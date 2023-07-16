# Comparing `tmp/basictdf-0.1.8.tar.gz` & `tmp/basictdf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basictdf-0.1.8.tar", max compression
+gzip compressed data, was "basictdf-0.1.9.tar", max compression
```

## Comparing `basictdf-0.1.8.tar` & `basictdf-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      321 2023-07-10 17:26:48.883559 basictdf-0.1.8/README.md
--rw-r--r--   0        0        0      579 2023-07-10 17:26:48.887559 basictdf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2956 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/__init__.py
--rw-r--r--   0        0        0    17804 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/basictdf.py
--rw-r--r--   0        0        0     3824 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfBlock.py
--rw-r--r--   0        0        0    14252 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfCalibrationData.py
--rw-r--r--   0        0        0     5663 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfData2D.py
--rw-r--r--   0        0        0    12496 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfData3D.py
--rw-r--r--   0        0        0     7160 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfEMG.py
--rw-r--r--   0        0        0     4779 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfEvents.py
--rw-r--r--   0        0        0    10800 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfForce3D.py
--rw-r--r--   0        0        0     8432 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfForcePlatformsCalibration.py
--rw-r--r--   0        0        0     7410 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfForcePlatformsData.py
--rw-r--r--   0        0        0     5644 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfOpticalSystem.py
--rw-r--r--   0        0        0     6652 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfTypes.py
--rw-r--r--   0        0        0     1434 2023-07-10 17:26:48.887559 basictdf-0.1.8/src/basictdf/tdfUtils.py
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 basictdf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      952 2023-07-16 08:24:29.034191 basictdf-0.1.9/README.md
+-rw-r--r--   0        0        0      671 2023-07-16 08:24:29.034191 basictdf-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3012 2023-07-16 08:24:29.034191 basictdf-0.1.9/src/basictdf/__init__.py
+-rw-r--r--   0        0        0    18571 2023-07-16 08:24:29.034191 basictdf-0.1.9/src/basictdf/basictdf.py
+-rw-r--r--   0        0        0     4233 2023-07-16 08:24:29.034191 basictdf-0.1.9/src/basictdf/tdfBlock.py
+-rw-r--r--   0        0        0    15763 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfCalibrationData.py
+-rw-r--r--   0        0        0     5794 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfData2D.py
+-rw-r--r--   0        0        0    12542 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfData3D.py
+-rw-r--r--   0        0        0     7926 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfEMG.py
+-rw-r--r--   0        0        0     4730 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfEvents.py
+-rw-r--r--   0        0        0    10800 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfForce3D.py
+-rw-r--r--   0        0        0     8502 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfForcePlatformsCalibration.py
+-rw-r--r--   0        0        0     8410 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfForcePlatformsData.py
+-rw-r--r--   0        0        0     5670 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfOpticalSystem.py
+-rw-r--r--   0        0        0     6686 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfTypes.py
+-rw-r--r--   0        0        0     1434 2023-07-16 08:24:29.038191 basictdf-0.1.9/src/basictdf/tdfUtils.py
+-rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 basictdf-0.1.9/PKG-INFO
```

### Comparing `basictdf-0.1.8/src/basictdf/__init__.py` & `basictdf-0.1.9/src/basictdf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,16 @@
     "Data3D",
     "MarkerTrack",
     "TemporalEventsData",
     "Event",
     "EventsDataType",
     "EMG",
     "EMGTrack",
+    "ForcePlatformsDataBlock",
+    "ForcePlatformData",
 ]
 
 
 __pdoc__ = {}
 __pdoc__["basictdf.tdfUtils"] = False
 __pdoc__["basictdf.tdfTypes"] = False
 __pdoc__["collections.ABC"] = False
```

### Comparing `basictdf-0.1.8/src/basictdf/basictdf.py` & `basictdf-0.1.9/src/basictdf/basictdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,43 +123,57 @@
             size,
             creation_date,
             last_modification_date,
             last_access_date,
             comment,
         )
 
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, TdfEntry):
+            return False
+        return (
+            self.type == o.type
+            and self.format == o.format
+            and self.offset == o.offset
+            and self.size == o.size
+            and self.creation_date == o.creation_date
+            and self.last_modification_date == o.last_modification_date
+            and self.last_access_date == o.last_access_date
+            and self.comment == o.comment
+        )
+
     def __repr__(self) -> str:
         return (
             f"TdfEntry(type={self.type}, format={self.format}, offset={self.offset}, "
             f"size={self.size}, creation_date={self.creation_date}, "
             f"last_modification_date={self.last_modification_date}, "
             f"last_access_date={self.last_access_date}, comment={self.comment})"
         )
 
 
 class Tdf:
     SIGNATURE = b"\x82K`A\xd3\x11\x84\xca`\x00\xb6\xac\x16h\x0c\x08"
 
     def __init__(self, filename: Union[Path, str]) -> None:
-        self.filePath = Path(filename)
+        self.file_path = Path(filename)
 
-        if not self.filePath.exists():
-            raise FileNotFoundError(f"File {self.filePath} not found")
+        if not self.file_path.exists():
+            raise FileNotFoundError(f"File {self.file_path} not found")
 
         self._mode = "rb"
         self._inside_context = False
 
     def allow_write(self) -> "Tdf":
         """Allow writing to the file."""
         self._mode = "r+b"
         return self
 
     def __enter__(self) -> "Tdf":
         self._inside_context = True
-        self.handler: IO[bytes] = self.filePath.open(self._mode)
+        self.handler: IO[bytes] = self.file_path.open(self._mode)
 
         self.signature = self.handler.read(len(self.SIGNATURE))
 
         if self.signature != self.SIGNATURE:
             raise Exception("Invalid TDF file")
 
         self.version = u32.bread(self.handler)
@@ -505,18 +519,27 @@
 
         self.remove_block(newBlock.type)
         self.add_block(newBlock, comment)
 
     @property
     def nBytes(self) -> int:
         """Return the size of the TDF file in bytes"""
-        return self.filePath.stat().st_size
+        return self.file_path.stat().st_size
 
     def __len__(self) -> int:
         """Return the number of blocks in the TDF file
         that are not of type unusedSlot
         """
         return sum(1 for i in self.entries if i.type != BlockType.unusedSlot)
 
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, Tdf):
+            return False
+        return (
+            self.version == o.version
+            and self.nEntries == o.nEntries
+            and self.blocks == o.blocks
+        )
+
     @provide_context_if_needed
     def __repr__(self) -> str:
-        return f"Tdf({self.filePath}, nEntries={self.nEntries}, nBytes={self.nBytes}"
+        return f"Tdf({self.file_path}, nEntries={self.nEntries}, nBytes={self.nBytes}"
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfBlock.py` & `basictdf-0.1.9/src/basictdf/tdfBlock.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import IO, Optional
 
 __all__ = ["Block", "BlockType"]
 __doc__ = "Block and block type classes."
 
 
 class BlockType(Enum):
+    "All posible block types"
     unusedSlot = 0  # TDF_DATABLOCK_NOBLOCK
     notDefined = 1  # TDF_DATABLOCK_NOTYPE
     calibrationData = 2  # TDF_DATABLOCK_CALIB
     calibrationData2D = 3  # TDF_DATABLOCK_DATA2D4C
     data2D = 4  # TDF_DATABLOCK_DATA2D
     data3D = 5  # TDF_DATABLOCK_DATA3D
     opticalSystemConfiguration = 6  # TDF_DATABLOCK_OPTISETUP
@@ -23,15 +24,34 @@
     forceAndTorqueData = 12  # TDF_DATABLOCK_FORCE3D
     volumetricData = 13  # TDF_DATABLOCK_VOLUME
     analogData = 14  # TDF_DATABLOCK_GENPURPOSE
     generalCalibrationData = 15  # TDF_DATABLOCK_CALGENPURP
     temporalEventsData = 16  # TDF_DATABLOCK_EVENTS
 
 
-class Block(ABC):
+class Sized(ABC):
+    @property
+    @abstractmethod
+    def nBytes(self) -> int:
+        "Size in bytes"
+        pass
+
+
+class BuildWriteable(ABC):
+    @classmethod
+    @abstractmethod
+    def _build(cls, file: IO[bytes], format: int):
+        pass
+
+    @abstractmethod
+    def _write(self, file: IO[bytes]):
+        pass
+
+
+class Block(Sized, BuildWriteable, ABC):
     """
     A class to represent a TDF block.
     """
 
     type = BlockType.notDefined
 
     def __init__(
@@ -49,23 +69,15 @@
             else datetime.now()
         )
         self.last_access_date = (
             last_access_date if last_access_date is not None else datetime.now()
         )
 
     @abstractmethod
-    def nBytes(self) -> int:
-        pass
-
-    @abstractmethod
-    def _build(self, file: IO[bytes], format: int):
-        pass
-
-    @abstractmethod
-    def _write(self, file: IO[bytes]):
+    def __iter__(self):
         pass
 
     def __repr__(self):
         return f"<{self.__class__.__name__} type={self.type}>"
 
 
 class NotImplementedBlock(Block):
@@ -115,28 +127,38 @@
     type = BlockType.analogData
 
 
 class GeneralCalibrationData(NotImplementedBlock):
     type = BlockType.generalCalibrationData
 
 
+class UnusedFormat(Enum):
+    unusedFormat = 0
+
+
 class UnusedBlock(Block):
     type = BlockType.unusedSlot
     nBytes = 0
-    format = None
+    format = UnusedFormat.unusedFormat
+
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
 
     @staticmethod
     def _build(*args, **kwargs) -> "UnusedBlock":
         return UnusedBlock()
 
     def _write(self, *args, **kwargs) -> None:
         pass
 
     def __repr__(self) -> str:
         return "<UnusedBlock>"
 
+    def __iter__(self):
+        return iter([])
+
     def __eq__(self, other: "UnusedBlock") -> bool:
         return isinstance(other, UnusedBlock)
 
 
 class NotDefinedBlock(NotImplementedBlock):
     type = BlockType.notDefined
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfCalibrationData.py` & `basictdf-0.1.9/src/basictdf/tdfCalibrationData.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import IntEnum
 from typing import List, Union
 
 import numpy as np
 
-from basictdf.tdfBlock import Block, BlockType
+from basictdf.tdfBlock import Block, BlockType, BuildWriteable, Sized
 from basictdf.tdfTypes import (
     MAT3X3D,
     MAT3X3F,
     VEC2D,
     VEC3D,
     VEC3F,
     CameraViewPort,
@@ -29,44 +29,72 @@
     "Kali distorsion (from BTS) type"
     AmassDistorsion = 2
     "Amass distorsion (from BTS) type"
     Seelab1Distorsion = 3
     "Radial distorsion up to 2nd order"
 
 
-class SeelabCameraData:
+class SeelabCameraData(Sized, BuildWriteable):
     def __init__(
         self,
         rotation_matrix,
         translation_vector,
         focus,
         optical_center,
         radial_distortion,
         decentering,
         thin_prism,
         view_port: Union[CameraViewPort, np.ndarray],
     ) -> None:
+        if not isinstance(rotation_matrix, np.ndarray) or rotation_matrix.shape != (
+            3,
+            3,
+        ):
+            raise TypeError("rotation_matrix must be a (3,3) shape numpy array")
+
         self.rotation_matrix = rotation_matrix
         "Rotation matrix of the camera"
 
+        if not isinstance(
+            translation_vector, np.ndarray
+        ) or translation_vector.shape != (3,):
+            raise TypeError("translation_vector must be a (3,) shape numpy array")
+
         self.translation_vector = translation_vector
         "Translation vector of the camera"
 
+        if not isinstance(focus, np.ndarray) or focus.shape != (2,):
+            raise TypeError("focus must be a (2,) shape numpy array")
+
         self.focus = focus
         "Focal length of the camera"
 
+        if not isinstance(optical_center, np.ndarray) or optical_center.shape != (2,):
+            raise TypeError("optical_center must be a (2,) shape numpy array")
+
         self.optical_center = optical_center
         "Optical center of the camera"
 
+        if not isinstance(radial_distortion, np.ndarray) or radial_distortion.shape != (
+            2,
+        ):
+            raise TypeError("radial_distortion must be a (2,) shape numpy array")
+
         self.radial_distortion = radial_distortion
         "Radial distortion of the camera"
 
+        if not isinstance(decentering, np.ndarray) or decentering.shape != (2,):
+            raise TypeError("decentering must be a (2,) shape numpy array")
+
         self.decentering = decentering
         "Decentering of the camera"
 
+        if not isinstance(thin_prism, np.ndarray) or thin_prism.shape != (2,):
+            raise TypeError("thin_prism must be a (2,) shape numpy array")
+
         self.thin_prism = thin_prism
         "Thin prism of the camera"
 
         if isinstance(view_port, CameraViewPort):
             view_port = view_port
         elif isinstance(view_port, np.ndarray) and view_port.shape == (
             2,
@@ -273,16 +301,17 @@
         distorsion_model: DistorsionModel,
         calibration_volume_size: np.ndarray,
         calibration_volume_rotation_matrix: np.ndarray,
         calibration_volume_translation_vector: np.ndarray,
         cameras_calibration_map: np.ndarray,
         cam_data: Union[List[BTSCameraData], List[SeelabCameraData]],
         format: CalibrationDataBlockFormat = CalibrationDataBlockFormat.Seelab1,
+        **kwargs,
     ) -> None:
-        super().__init__()
+        super().__init__(**kwargs)
 
         self.distorsion_model = distorsion_model
         "Distorsion model of the calibration"
 
         if calibration_volume_size.shape != VEC3F.btype.shape:
             raise ValueError(
                 (
@@ -390,14 +419,21 @@
             + VEC3F.btype.itemsize  # calibration_volume
             + MAT3X3F.btype.itemsize  # rotation matrix
             + VEC3F.btype.itemsize  # translation_vector
             + i16.btype.itemsize * len(self.cam_data)  # calibration map
             + sum(cam.nBytes for cam in self.cam_data)  # calibration data
         )
 
+    def __iter__(self):
+        """
+        Iterates over the cameras in the block.
+        Returns a tuple of (channel, camera)
+        """
+        return iter(zip(self.cameras_calibration_map, self.cam_data))
+
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, CalibrationDataBlock):
             return False
 
         return (
             self.distorsion_model == o.distorsion_model
             and np.array_equal(self.calibration_volume_size, o.calibration_volume_size)
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfData2D.py` & `basictdf-0.1.9/src/basictdf/tdfData2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 __doc__ = """
 Data2D module
 """
 from enum import Enum
 
 import numpy as np
 
-from basictdf.tdfBlock import Block, BlockType
+from basictdf.tdfBlock import Block, BlockType, Sized, BuildWriteable
 from basictdf.tdfTypes import VEC2F, i32, i16, u32, u16, f32
 
 
 class Data2DFlags(Enum):
     with_distortion = 0
     without_distortion = 1
 
 
-class Data2DPCK:
+class Data2DPCK(Sized, BuildWriteable):
     def __init__(self, data) -> None:
         self.data = data
 
     @staticmethod
-    def _build(stream, nFrames, nCameras):
+    def _build(stream, nFrames, nCameras) -> "Data2DPCK":
         nPointsCaptured = u16.bread(stream, nCameras * nFrames).reshape(
             [nCameras, nFrames]
         )
         data = np.empty((nFrames, nCameras), dtype=object)
 
         for frame in range(nFrames):
             for camera in range(nCameras):
@@ -100,20 +100,23 @@
         the corresponding frame.
         """
         self.format = format
 
         self._camMap = []
         self._data = None
 
+    def __iter__(self):
+        return iter(self._data.data)
+
     @property
     def data(self):
         return self._data.data
 
     @data.setter
-    def data(self, value):
+    def data(self, value) -> None:
         self._data = Data2DPCK(value)
 
     @staticmethod
     def _build(stream, format) -> "Data2D":
         format = Data2DBlockFormat(format)
         if format != Data2DBlockFormat.PCKFormat:
             raise NotImplementedError(f"Data2D format {format} is not implemented yet.")
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfData3D.py` & `basictdf-0.1.9/src/basictdf/tdfData3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from enum import Enum
 from io import BytesIO
 from typing import BinaryIO, Iterable, Iterator, List, Union
 
 import numpy as np
 
-from basictdf.tdfBlock import Block, BlockType
+from basictdf.tdfBlock import Block, BlockType, BuildWriteable, Sized
 from basictdf.tdfTypes import (
     MAT3X3F,
     VEC3F,
     BTSString,
     TdfType,
     Volume,
     f32,
@@ -43,15 +43,15 @@
 
 
 LinkType = TdfType(np.dtype([("Track1", "<u4"), ("Track2", "<u4")]))
 
 TrackType = TdfType(np.dtype("<3f4"))
 
 
-class MarkerTrack:
+class MarkerTrack(Sized, BuildWriteable):
     """
     A track that collects all the data of a physical marker, such as name and position.
     """
 
     def __init__(self, label: str, track_data: np.ndarray) -> None:
         self.label = label
         "The name of the marker"
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfEMG.py` & `basictdf-0.1.9/src/basictdf/tdfEMG.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,60 @@
-__doc__ = "Electromyography data module."
+__doc__ = """
+
+EMG data module.
+
+This module contains the classes to represent EMG data in a TDF file.
+
+Example:
+
+```python
+from basictdf import Tdf, EMG, EMGTrack
+import numpy as np
+
+# Create an empty EMG block
+emg = EMG(frequency=1000, nSamples=1000)
+
+# Create a bogus EMG track with random data
+emgTrack = EMGTrack("emg", np.random.rand(1000))
+
+# Add it to the EMG block
+emg.addSignal(emgTrack)
+
+# Write it to a new TDF file
+with Tdf.new("my_file.tdf").allow_write() as tdf:
+    tdf.emg = emg
+
+# This works too
+tdf = Tdf.new("my_file.tdf")
+with tdf.allow_write() as tdf:
+    tdf.emg = emg
+
+```
+
+"""
+
 
 from enum import Enum
 from typing import Iterator, Union
 
 import numpy as np
 
-from basictdf.tdfBlock import Block, BlockType
+from basictdf.tdfBlock import Block, BlockType, Sized, BuildWriteable
 from basictdf.tdfTypes import BTSString, TdfType, f32, i16, i32
 
 SegmentData = TdfType(np.dtype([("startFrame", "<i4"), ("nFrames", "<i4")]))
 
 
 class EMGBlockFormat(Enum):
     unknownFormat = 0
     byTrack = 1
     byFrame = 2
 
 
-class EMGTrack:
+class EMGTrack(Sized, BuildWriteable):
     def __init__(self, label: str, trackData: np.ndarray) -> None:
         self.label = label
         self.data = trackData
 
     @property
     def nSamples(self) -> int:
         """
@@ -32,26 +65,26 @@
 
     @property
     def _segments(self):
         maskedTrackData = np.ma.masked_invalid(self.data)
         return np.ma.clump_unmasked(maskedTrackData.T)
 
     @staticmethod
-    def build(stream, nSamples) -> "EMGTrack":
+    def _build(stream, nSamples) -> "EMGTrack":
         label = BTSString.bread(stream, 256)
         nSegments = i32.bread(stream)
         i32.skip(stream)  # padding
         segmentData = SegmentData.bread(stream, nSegments)
         trackData = np.empty(nSamples, dtype="<f4")
         trackData[:] = np.nan
         for startFrame, nFrames in segmentData:
             trackData[startFrame : startFrame + nFrames] = f32.bread(stream, nFrames)
         return EMGTrack(label, trackData)
 
-    def write(self, file) -> None:
+    def _write(self, file) -> None:
         # label
         BTSString.bwrite(file, 256, self.label)
 
         segments = self._segments
 
         # nSegments
         i32.bwrite(file, len(segments))
@@ -110,15 +143,15 @@
         startTime = f32.bread(stream)
         nSamples = i32.bread(stream) + 49  # Why 49??? Whyyyy????
         emgMap = i16.bread(stream, n=nSignals)
 
         d = EMG(frequency, nSamples, startTime, format)
         if format == EMGBlockFormat.byTrack:
             for n in range(nSignals):
-                emgSignal = EMGTrack.build(stream, nSamples)
+                emgSignal = EMGTrack._build(stream, nSamples)
                 d.addSignal(emgSignal, channel=emgMap[n])
         else:
             raise NotImplementedError(f"EMG format {format} not implemented yet")
         return d
 
     def _write(self, file) -> None:
         if self.format != EMGBlockFormat.byTrack:
@@ -137,15 +170,15 @@
         i32.bwrite(file, self.nSamples - 49)  # That 49 again
 
         # emgMap
         i16.bwrite(file, self._emgMap)
 
         # signals
         for signal in self._signals:
-            signal.write(file)
+            signal._write(file)
 
     def __getitem__(self, key) -> EMGTrack:
         if isinstance(key, int):
             return self._signals[key]
         elif isinstance(key, str):
             try:
                 return next(signal for signal in self._signals if signal.label == key)
@@ -163,24 +196,26 @@
     def __iter__(self) -> Iterator[EMGTrack]:
         return iter(self._signals)
 
     def __len__(self) -> int:
         return len(self._signals)
 
     def __eq__(self, other) -> bool:
+        if not isinstance(other, EMG):
+            return False
         return (
             self.frequency == other.frequency
             and self.startTime == other.startTime
             and self.nSamples == other.nSamples
             and all(s1 == s2 for s1, s2 in zip(self._signals, other._signals))
         )
 
     def addSignal(self, signal: EMGTrack, channel=None) -> None:
         """
-        adds a signal to the EMG block. If the channel is not specified,
+        Adds a signal to the EMG block. If the channel is not specified,
         it is set to the next one  available
         """
         if not isinstance(signal, EMGTrack):
             raise TypeError(f"Can only add EMGTrack objects, got {type(signal)}")
         if signal.nSamples != self.nSamples:
             raise ValueError(
                 (
@@ -198,14 +233,17 @@
         else:
             if channel in self._emgMap:
                 raise ValueError(f"Channel {channel} already in use")
             self._emgMap.append(channel)
         self._signals.append(signal)
 
     def removeSignal(self, label: str) -> None:
+        """
+        Removes a signal specified by its label from the EMG block
+        """
         try:
             pos = next(i for i, v in enumerate(self._signals) if v == label)
         except StopIteration:
             raise KeyError(f"EMG signal with label {label} not found")
 
         del self._signals[pos]
         del self._emgMap[pos]
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfEvents.py` & `basictdf-0.1.9/src/basictdf/tdfEvents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 __doc__ = "Events data module."
 
 from enum import Enum
 from typing import Iterator, Union
 
 import numpy as np
 
-from basictdf.tdfBlock import Block, BlockType
+from basictdf.tdfBlock import Block, BlockType, BuildWriteable, Sized
 from basictdf.tdfTypes import BTSString, f32, i32, u32
 from basictdf.tdfUtils import is_iterable
 
 
 class TemporalEventsDataFormat(Enum):
     unknown = 0
     standard = 1
 
 
 class EventsDataType(Enum):
     singleEvent = 0
     eventSequence = 1
 
 
-class Event:
+class Event(Sized, BuildWriteable):
     """
     A class representing a single event or a sequence of events.
     """
 
     def __init__(self, label, values=[], type=EventsDataType.singleEvent) -> None:
         self.label = label
         self.type = type
@@ -76,15 +76,15 @@
             f"nItems={len(self.values)} "
             f"values={self.values}>"
         )
 
 
 class TemporalEventsData(Block):
     """
-    A class to represent a TDF temporal events data block.
+    The Events data block. Stores the temporal events data.
     """
 
     type = BlockType.temporalEventsData
 
     def __init__(self, format=TemporalEventsDataFormat.standard, start_time=0.0):
         super().__init__()
         self.format = format
@@ -133,17 +133,15 @@
             return value in self.events
         elif isinstance(value, str):
             return any(value == event.label for event in self.events)
         raise TypeError(f"Invalid key type: {type(value)}")
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, TemporalEventsData):
-            raise TypeError(
-                "Can only compare TemporalEventsData with TemporalEventsData"
-            )
+            return False
         return (
             self.format == other.format
             and self.start_time == other.start_time
             and all(e1 == e2 for e1, e2 in zip(self.events, other.events))
         )
 
     def __repr__(self) -> str:
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfForce3D.py` & `basictdf-0.1.9/src/basictdf/tdfForce3D.py`

 * *Files identical despite different names*

### Comparing `basictdf-0.1.8/src/basictdf/tdfForcePlatformsCalibration.py` & `basictdf-0.1.9/src/basictdf/tdfForcePlatformsCalibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,20 @@
     number. The channel number links the logical channel of the platform to the
     physical channel of the data acquisition system.
     """
 
     type = BlockType.forcePlatformsCalibrationData
 
     def __init__(
-        self, platforms=None, format=ForcePlatformCalibrationBlockFormat.GRPFormat
+        self,
+        platforms=None,
+        format=ForcePlatformCalibrationBlockFormat.GRPFormat,
+        **kwargs,
     ) -> None:
+        super().__init__(**kwargs)
         self._platforms: List[ForcePlatformInfo] = platforms or []
         self._platformMap = []
         self.format = format
 
     @staticmethod
     def _build(stream, format) -> "ForcePlatformsCalibrationDataBlock":
         format = ForcePlatformCalibrationBlockFormat(format)
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfForcePlatformsData.py` & `basictdf-0.1.9/src/basictdf/tdfForcePlatformsData.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+__doc__ = """
+Force platform data module.
+"""
+
 from enum import Enum
-from basictdf.tdfBlock import Block, BlockType
+from basictdf.tdfBlock import Block, BlockType, Sized, BuildWriteable
 from basictdf.tdfTypes import i32, u16, SegmentData, TdfType, f32
 
 import numpy as np
 
 PlatDataType = TdfType(
     np.dtype([("application_point", "2<f4"), ("force", "3<f4"), ("torque", "<f4")])
 )
@@ -23,21 +27,27 @@
     byFrameISSWithVelocityFormat = 10  # TDF_DATAPLAT_FORMAT_BYFRAME_ISS_VEL
     byTrackISSWithLabelsAndVelocityFormat = 11  # TDF_DATAPLAT_FORMAT_BYTRACK_WL_ISS_VEL
     byFrameISSWithLabelsAndVelocityFormat = 12  # TDF_DATAPLAT_FORMAT_BYFRAME_WL_ISS_VEL
     byTrackDoubleWithVelocityFormat = 13  # TDF_DATAPLAT_FORMAT_BYTRACK_DBL_VEL
     byFrameDoubleWithVelocityFormat = 14  # TDF_DATAPLAT_FORMAT_BYFRAME_DBL_VEL
 
 
-class ForcePlatformData:
+class ForcePlatformData(Sized, BuildWriteable):
     """
     Class that stores the data of a force platform,
     such as force, torque and application point.
     """
 
-    def __init__(self, label, application_point, force, torque) -> None:
+    def __init__(
+        self,
+        label: str,
+        application_point: np.array,
+        force: np.array,
+        torque: np.array,
+    ) -> None:
         self.label = label
         "Force platform label"
         self.application_point = application_point
         "Position of the application point in x,y coordinates"
         self.force = force
         "Force in x,y,z coordinates"
         self.torque = torque
@@ -87,14 +97,15 @@
             i32.bwrite(stream, np.array(segment.stop - segment.start))
 
         for segment in segments:
             PlatDataType.bwrite(stream, self._get_segment_data(segment))
 
     @property
     def nBytes(self) -> int:
+        "Size in bytes of the platform data"
         nSegments = len(self._segments)
 
         base = 4 + 4 + (4 + 4) * nSegments
 
         for segment in self._segments:
             base += PlatDataType.btype.itemsize * (segment.stop - segment.start)
 
@@ -170,14 +181,34 @@
         i32.bwrite(stream, self.frequency)
         f32.bwrite(stream, self.start_time)
         i32.bwrite(stream, self.n_frames)
         u16.bwrite(stream, self._plat_map)
         for plat in self._platforms:
             plat._write(stream, self.format)
 
+    def __iter__(self):
+        """
+        Iterates over the platforms in the block.
+        Returns a tuple of (channel, platform)
+        """
+        return iter(zip(self._plat_map, self._platforms))
+
+    def add_platform(self, platform: ForcePlatformData, channel: int = None) -> None:
+        """
+        Adds a platform to the block. If channel is specified and it's not already
+        in use, the platform is added to that channel. Otherwise, the platform is
+        added to the next available channel.
+        """
+        if channel is None:
+            channel = len(self._platforms)
+        if channel in self._plat_map:
+            raise ValueError(f"Channel {channel} already in use")
+        self._plat_map.append(channel)
+        self._platforms.append(platform)
+
     @property
     def nBytes(self) -> int:
         return (
             4  # nPlatforms
             + 4  # frequency
             + 4  # startTime
             + 4  # nFrames
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfOpticalSystem.py` & `basictdf-0.1.9/src/basictdf/tdfOpticalSystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,20 +120,21 @@
 class OpticalSetupBlock(Block):
     type = BlockType.opticalSystemConfiguration
 
     def __init__(
         self,
         format: OpticalSetupBlockFormat = OpticalSetupBlockFormat.basicFormat,
         channels: List[OpticalChannelData] = [],
+        **kwargs,
     ) -> None:
         """A data block containing information about the physical setup of
         motion capture.
         """
 
-        super().__init__()
+        super().__init__(**kwargs)
         self.format = format
         self.channels = channels
 
     @staticmethod
     def _build(stream, format) -> "OpticalSetupBlock":
         format = OpticalSetupBlockFormat(format)
         nChannels = i32.bread(stream)
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfTypes.py` & `basictdf-0.1.9/src/basictdf/tdfTypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,11 +204,13 @@
 
     def __repr__(self) -> str:
         return f"CameraViewPort(origin={self.origin}, size={self.size})"
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, CameraViewPort):
             raise TypeError("Can only compare CameraViewPort with CameraViewPort")
-        return np.all(self.origin == other.origin) and np.all(self.size == other.size)
+        return np.array_equal(self.origin, other.origin) and np.array_equal(
+            self.size, other.size
+        )
 
 
 SegmentData = TdfType(np.dtype([("startFrame", "<i4"), ("nFrames", "<i4")]))
```

### Comparing `basictdf-0.1.8/src/basictdf/tdfUtils.py` & `basictdf-0.1.9/src/basictdf/tdfUtils.py`

 * *Files identical despite different names*

