# Comparing `tmp/terminal_manager-0.6.0.tar.gz` & `tmp/terminal_manager-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.6.0.tar", last modified: Sat Jul 15 08:24:50 2023, max compression
+gzip compressed data, was "terminal_manager-0.7.0.tar", last modified: Sun Jul 16 06:08:01 2023, max compression
```

## Comparing `terminal_manager-0.6.0.tar` & `terminal_manager-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.6.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.6.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-15 08:17:22.000000 terminal_manager-0.6.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.328201 terminal_manager-0.6.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.344201 terminal_manager-0.6.0/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     7058 2023-07-14 02:57:27.000000 terminal_manager-0.6.0/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5805 2023-07-15 07:05:41.000000 terminal_manager-0.6.0/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-13 07:25:10.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4074 2023-07-15 03:35:59.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-14 05:28:35.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-15 03:36:09.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8394 2023-07-14 07:44:55.000000 terminal_manager-0.6.0/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.348202 terminal_manager-0.6.0/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.7.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.7.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-16 06:02:52.000000 terminal_manager-0.7.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.426293 terminal_manager-0.7.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7058 2023-07-16 04:46:49.000000 terminal_manager-0.7.0/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5748 2023-07-16 04:40:07.000000 terminal_manager-0.7.0/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4312 2023-07-16 04:02:15.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-16 03:15:36.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-16 03:21:41.000000 terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8387 2023-07-16 04:39:12.000000 terminal_manager-0.7.0/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-15 08:37:34.000000 terminal_manager-0.7.0/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:08:01.430293 terminal_manager-0.7.0/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-16 06:08:01.000000 terminal_manager-0.7.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.6.0/LICENSE` & `terminal_manager-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/PKG-INFO` & `terminal_manager-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.6.0
+Version: 0.7.0
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.6.0/pyproject.toml` & `terminal_manager-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `terminal_manager-0.6.0/src/terminal_manager/__init__.py` & `terminal_manager-0.7.0/src/terminal_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/src/terminal_manager/collection.py` & `terminal_manager-0.7.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/src/terminal_manager/command.py` & `terminal_manager-0.7.0/src/terminal_manager/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,27 +101,25 @@
 
         Raises:
             CommandError
         """
         try:
             string = await self.async_generate_string(manager, variables)
         except CommandError as exc:
-            manager.logger.info(
-                "[%s] Command: %s => %s", manager.name, self.string, exc
-            )
+            manager.logger.debug("%s: %s => %s", manager.name, self.string, exc)
             raise
 
         try:
             output = await manager.async_execute_command_string(string, self.timeout)
         except CommandError as exc:
-            manager.logger.info("[%s] Command: %s => %s", manager.name, string, exc)
+            manager.logger.debug("%s: %s => %s", manager.name, string, exc)
             raise
 
-        manager.logger.info(
-            "[%s] Command: %s => %s, %s, %s",
+        manager.logger.debug(
+            "%s: %s => %s, %s, %s",
             manager.name,
             string,
             output.stdout,
             output.stderr,
             output.code,
         )
```

### Comparing `terminal_manager-0.6.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.7.0/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.7.0/src/terminal_manager/default_collections/linux.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,45 +34,59 @@
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 )
             ],
         ),
         SensorCommand(
-            "file=/sys/class/net/@sensor{network_interface}/device/power/wakeup; "
-            + "[[ ! -f $file ]] || cat $file",
+            "cat /sys/class/net/@sensor{network_interface}/device/power/wakeup 2>/dev/null",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
                 )
             ],
         ),
         SensorCommand(
-            "uname -a | awk '{print $1; print $2; print $3; print $(NF-1)}'",
+            "uname -n",
             sensors=[
                 TextSensor(
-                    SensorName.OS_NAME,
-                    SensorKey.OS_NAME,
-                ),
-                TextSensor(
                     SensorName.HOSTNAME,
                     SensorKey.HOSTNAME,
                 ),
-                TextSensor(
-                    SensorName.OS_VERSION,
-                    SensorKey.OS_VERSION,
-                ),
+            ],
+        ),
+        SensorCommand(
+            "uname -m",
+            sensors=[
                 TextSensor(
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
                 ),
             ],
         ),
         SensorCommand(
+            "uname -s",
+            sensors=[
+                TextSensor(
+                    SensorName.OS_NAME,
+                    SensorKey.OS_NAME,
+                ),
+            ],
+        ),
+        SensorCommand(
+            "uname -r",
+            sensors=[
+                TextSensor(
+                    SensorName.OS_VERSION,
+                    SensorKey.OS_VERSION,
+                ),
+            ],
+        ),
+        SensorCommand(
             "free -k | awk '/^Mem:/ {print $2}'",
             sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
                     unit="KiB",
                 )
@@ -86,28 +100,28 @@
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            "df -k | awk '/^\\/dev\\// {print $6 \"|\" $4}'",
+            'df -k | awk \'/^\\/dev\\// {x=$0; sub(/^[^ ]+( +[^ ]+){4} /,"",x); print x "|" $4}\'',
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            "top -bn1 | awk 'NR<4 && tolower($0)~/cpu/ {print 100-$8}'",
+            "top -bn1 | awk 'NR<4 && tolower($0) ~ /cpu/ {print 100-$8}'",
             interval=30,
             sensors=[
                 NumberSensor(
                     SensorName.CPU_LOAD,
                     SensorKey.CPU_LOAD,
                     unit="%",
                 )
@@ -121,15 +135,15 @@
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
                 )
             ],
         ),
         SensorCommand(
-            "ps -e --no-headers | wc -l",
+            "ps -e | awk 'END {print NR-1}'",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.PROCESSES,
                     SensorKey.PROCESSES,
                 )
             ],
```

### Comparing `terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -36,34 +36,34 @@
                 TextSensor(
                     SensorName.NETWORK_INTERFACE,
                     SensorKey.NETWORK_INTERFACE,
                 ),
             ],
         ),
         SensorCommand(
+            "hostname",
+            sensors=[
+                TextSensor(
+                    SensorName.HOSTNAME,
+                    SensorKey.HOSTNAME,
+                )
+            ],
+        ),
+        SensorCommand(
             'for /f "skip=1 tokens=*" %i in (\'wmic ComputerSystem '
             + "get SystemType') do "
             + "@echo %i",
             sensors=[
                 TextSensor(
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
                 ),
             ],
         ),
         SensorCommand(
-            "hostname",
-            sensors=[
-                TextSensor(
-                    SensorName.HOSTNAME,
-                    SensorKey.HOSTNAME,
-                )
-            ],
-        ),
-        SensorCommand(
             "for /f \"skip=1 tokens=*\" %i in ('wmic OS get Caption') do @echo %i",
             sensors=[
                 TextSensor(
                     SensorName.OS_NAME,
                     SensorKey.OS_NAME,
                 ),
             ],
```

### Comparing `terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.7.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/src/terminal_manager/event.py` & `terminal_manager-0.7.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/src/terminal_manager/sensor.py` & `terminal_manager-0.7.0/src/terminal_manager/sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,30 +69,30 @@
 
     def _validate(self, value: Any) -> None:
         ...
 
     def _update_value(self, manager: Manager, data: str | None) -> None:
         if data is None:
             self.value = None
-            manager.logger.info(
-                "[%s] Sensor: %s => %s", manager.name, self.key, self.value
-            )
+            manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
             return
 
         try:
             value_string = self._render(data)
             value = self._convert(value_string)
             self._validate(value)
         except Exception as exc:  # pylint: disable=broad-except
             self.value = None
-            manager.logger.info("[%s] Sensor: %s => %s", manager.name, self.key, exc)
+            manager.logger.debug(
+                "%s: %s => %s (%s)", manager.name, self.key, self.value, exc
+            )
             return
 
         self.value = self.last_known_value = value
-        manager.logger.info("[%s] Sensor: %s => %s", manager.name, self.key, self.value)
+        manager.logger.debug("%s: %s => %s", manager.name, self.key, self.value)
 
     def _update_child_sensors(self, manager: Manager, data: list[str] | None) -> None:
         if data is None:
             for child in self.child_sensors:
                 child.update(manager, None)
             return
```

### Comparing `terminal_manager-0.6.0/src/terminal_manager/synchronizer.py` & `terminal_manager-0.7.0/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.6.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.7.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.6.0
+Version: 0.7.0
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `terminal_manager-0.6.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.7.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

