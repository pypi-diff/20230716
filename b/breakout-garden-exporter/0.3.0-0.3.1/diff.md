# Comparing `tmp/breakout-garden-exporter-0.3.0.tar.gz` & `tmp/breakout-garden-exporter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breakout-garden-exporter-0.3.0.tar", last modified: Thu Jul 13 17:30:52 2023, max compression
+gzip compressed data, was "breakout-garden-exporter-0.3.1.tar", last modified: Sun Jul 16 20:48:09 2023, max compression
```

## Comparing `breakout-garden-exporter-0.3.0.tar` & `breakout-garden-exporter-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.691657 breakout-garden-exporter-0.3.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/bin/breakout-garden-exporter
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.691657 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 17:30:52.000000 breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/breakoutgardenexporter/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-13 17:30:47.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/icp10125.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/breakoutgardenexporter/sgp30.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:30:52.695657 breakout-garden-exporter-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_icp10125.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_sensor_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-13 17:30:24.000000 breakout-garden-exporter-0.3.0/tests/test_sgp30.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/bin/breakout-garden-exporter
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-16 20:48:09.000000 breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-16 20:48:09.000000 breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:48:09.000000 breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 20:48:09.000000 breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-16 20:48:09.000000 breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/breakoutgardenexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-16 20:48:06.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/icp10125.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/sensor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/breakoutgardenexporter/sgp30.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:48:09.117070 breakout-garden-exporter-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/tests/test_icp10125.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/tests/test_sensor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-16 20:47:47.000000 breakout-garden-exporter-0.3.1/tests/test_sgp30.py
```

### Comparing `breakout-garden-exporter-0.3.0/LICENSE` & `breakout-garden-exporter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/PKG-INFO` & `breakout-garden-exporter-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breakout-garden-exporter
-Version: 0.3.0
+Version: 0.3.1
 Summary: Exposes Prometheus metrics based on data collected from Pimoroni Breakout Garden sensors
 Home-page: https://github.com/andrewjw/breakout-garden-exporter
 Author: Andrew Wilkinson
 Author-email: andrewjwilkinson@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `breakout-garden-exporter-0.3.0/README.md` & `breakout-garden-exporter-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/bin/breakout-garden-exporter` & `breakout-garden-exporter-0.3.1/bin/breakout-garden-exporter`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/PKG-INFO` & `breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: breakout-garden-exporter
-Version: 0.3.0
+Version: 0.3.1
 Summary: Exposes Prometheus metrics based on data collected from Pimoroni Breakout Garden sensors
 Home-page: https://github.com/andrewjw/breakout-garden-exporter
 Author: Andrew Wilkinson
 Author-email: andrewjwilkinson@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `breakout-garden-exporter-0.3.0/breakout_garden_exporter.egg-info/SOURCES.txt` & `breakout-garden-exporter-0.3.1/breakout_garden_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/__init__.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 from .arguments import get_arguments
 from .icp10125 import ICP10125Sensor
 from .metrics import Metrics, MetricType, COUNTER, GAUGE
 from .sensor_manager import SensorManager
 from .server import serve
 from .sgp30 import SGP30Sensor
```

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/arguments.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/arguments.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/icp10125.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/icp10125.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class ICP10125Sensor(Sensor):
     def __init__(self) -> None:
         self.sensor: Optional[ICP10125] = None
 
     def initialise(self, metrics: Metrics) -> bool:
         try:
             self.sensor = ICP10125()
-        except RuntimeError:
+        except (RuntimeError, FileNotFoundError):
             return False
         else:
             metrics.add_metric("bge_pressure", GAUGE, "The air pressure")
             metrics.add_metric("bge_temperature", GAUGE, "The temperature")
 
             return True
```

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/metrics.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/metrics.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/sensor.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/sensor_manager.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/sensor_manager.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/server.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/server.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/breakoutgardenexporter/sgp30.py` & `breakout-garden-exporter-0.3.1/breakoutgardenexporter/sgp30.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.sensor: Optional[SGP30] = None
         self.warmed_up: bool = False
         self.initial_readings: int = 0
 
     def initialise(self, metrics: Metrics) -> bool:
         try:
             self.sensor = SGP30()
-        except RuntimeError:
+        except (RuntimeError, FileNotFoundError):
             return False
         else:
             self.sensor.command('init_air_quality')
             metrics.add_metric("bge_equivalent_co2",
                                GAUGE,
                                "The equivalent co2 (ppm)")
             metrics.add_metric("bge_voc",
```

### Comparing `breakout-garden-exporter-0.3.0/setup.py` & `breakout-garden-exporter-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/tests/__init__.py` & `breakout-garden-exporter-0.3.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/tests/test_arguments.py` & `breakout-garden-exporter-0.3.1/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/tests/test_icp10125.py` & `breakout-garden-exporter-0.3.1/tests/test_icp10125.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/tests/test_metrics.py` & `breakout-garden-exporter-0.3.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/tests/test_sensor_manager.py` & `breakout-garden-exporter-0.3.1/tests/test_sensor_manager.py`

 * *Files identical despite different names*

### Comparing `breakout-garden-exporter-0.3.0/tests/test_sgp30.py` & `breakout-garden-exporter-0.3.1/tests/test_sgp30.py`

 * *Files identical despite different names*

