# Comparing `tmp/homeconnect_webthing-0.3.9.tar.gz` & `tmp/homeconnect_webthing-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeconnect_webthing-0.3.9.tar", last modified: Sat Feb 25 09:25:36 2023, max compression
+gzip compressed data, was "homeconnect_webthing-1.0.0.tar", last modified: Sun Jul 16 09:10:21 2023, max compression
```

## Comparing `homeconnect_webthing-0.3.9.tar` & `homeconnect_webthing-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:25:36.769319 homeconnect_webthing-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-25 09:25:36.769319 homeconnect_webthing-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:25:36.769319 homeconnect_webthing-0.3.9/homeconnect_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    33554 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/appliances.py
--rw-r--r--   0 runner    (1001) docker     (123)    27284 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/appliances_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/homeconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/homeconnect_webthing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 09:25:36.769319 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-25 09:25:36.000000 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-25 09:25:36.000000 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 09:25:36.000000 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-25 09:25:36.000000 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-25 09:25:36.000000 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-25 09:25:36.000000 homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-25 09:25:27.000000 homeconnect_webthing-0.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-25 09:25:36.769319 homeconnect_webthing-0.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/homeconnect_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/appliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26282 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/appliances_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/homeconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/homeconnect_webthing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 09:10:21.000000 homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-16 09:10:05.000000 homeconnect_webthing-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-16 09:10:21.329148 homeconnect_webthing-1.0.0/setup.cfg
```

### Comparing `homeconnect_webthing-0.3.9/LICENSE` & `homeconnect_webthing-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-0.3.9/PKG-INFO` & `homeconnect_webthing-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeconnect_webthing
-Version: 0.3.9
+Version: 1.0.0
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `homeconnect_webthing-0.3.9/README.md` & `homeconnect_webthing-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/__init__.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/app.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/app.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/appliances.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/appliances.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 import logging
 import requests
 import json
 from time import sleep
 from typing import List, Dict, Any
 from datetime import datetime, timedelta
-from os.path import exists, join
-from os import makedirs
-from appdirs import site_data_dir
+from redzoo.database.simple import SimpleDB
 from homeconnect_webthing.auth import Auth
 from homeconnect_webthing.eventstream import EventListener
 from homeconnect_webthing.utils import print_duration, is_success
 
 
 
 class OfflineException(Exception):
     pass
 
 
 class Appliance(EventListener):
 
+    ON = "On"
+    OFF = "Off"
+
+    STATE_READY = "READY"
+    STATE_STARTABLE = "STARTABLE"
+    STATE_DELAYED_STARTED = "DELAYED_STARTED"
+    STATE_RUNNING = "RUNNING"
+    STATE_FINISHED = "FINISHED"
+    STATE_OFF = "OFF"
+    VALID_STATES = [STATE_READY, STATE_STARTABLE, STATE_DELAYED_STARTED, STATE_RUNNING, STATE_FINISHED, STATE_OFF]
+
     def __init__(self, device_uri: str, auth: Auth, name: str, device_type: str, haid: str, brand: str, vib: str, enumber: str):
         self._device_uri = device_uri
         self._auth = auth
         self.name = name
         self.device_type = device_type
         self.haid = haid
         self.brand = brand
         self.vib = vib
         self.enumber = enumber
         self.__value_changed_listeners = set()
         self.last_refresh = datetime.now() - timedelta(hours=9)
         self.remote_start_allowed = False
-        self.startable = False
-        self.started = False
         self.program_remote_control_active = False
         self._program_selected = ""
         self.program_remaining_time_sec = 0
         self.__program_progress = 0
         self.__program_local_control_active = ""
         self._power = ""
         self._door = ""
         self._operation = ""
-        self.completed = True
-        self.status = "INACTIVE"
         self.__program_active = ""
         self.child_lock = False
+        self.__db = SimpleDB(haid + '_db')
         self._reload_status_and_settings()
         self._reload_selected_program(ignore_error=True)
 
     def id(self) -> str:
         return self.haid
 
     @property
     def power(self):
         if len(self._power) > 0:
             return self._power[self._power.rindex('.')+1:]
         else:
-            return "Off"
+            return self.OFF
 
     @property
     def door(self):
         if len(self._door) > 0:
             return self._door[self._door.rindex('.')+1:]
         else:
             return ""
 
     @property
     def operation(self):
-        if len(self._operation)> 0:
+        if len(self._operation) > 0:
             return self._operation[self._operation.rindex('.')+1:]
         else:
             return ""
 
     @property
     def program_selected(self):
         if len(self._program_selected) > 0:
@@ -86,65 +92,74 @@
         else:
             return 0
 
     def register_value_changed_listener(self, value_changed_listener):
         self.__value_changed_listeners.add(value_changed_listener)
         self._notify_listeners()
 
-    def __update_state(self):
-        if self.power.lower() == "on" and self.operation.lower() == 'delayedstart':
-            new_status = "DELAYED_STARTED"
+    @property
+    def state(self) -> str:
+        return self.__db.get("state", self.STATE_READY)
 
-        elif self.power.lower() == "on" and self.operation.lower() == 'run':
-            new_status = "STARTED"
-            self.completed = False
-
-        elif self.power.lower() == "on" and \
-             not self.completed and \
-             self.door.lower() == "closed" and \
-             self.remote_start_allowed and \
-             self.operation.lower() not in ['delayedstart', 'run', 'finished', 'inactive']:
-            new_status = "REMOTE_STARTABLE"
-
-        elif self.power.lower() != "on":
-            new_status = "INACTIVE"
-            self.completed = True
-
-        else:
-            new_status = "INACTIVE"
-
-        if self.status != new_status:
-            logging.info("new status: " + new_status + " (previous: " + self.status + ")")
-            self.status = new_status
+    @state.setter
+    def state(self, new_state: str):
+        if self.state != new_state:
+            logging.info(self.name + " new state: " + new_state + " (previous: " + self.state + ")")
+            self.__db.put("state", new_state)
 
+    @property
+    def __previous_run_completed(self) -> bool:
+        return self.__db.get("previous_program_completed", True)
 
-    def _notify_listeners(self):
-        self.__update_state()
+    @__previous_run_completed.setter
+    def __previous_run_completed(self, completed: bool):
+        self.__db.put("previous_program_completed", completed)
+
+    def __update_state(self):
+        power = self.power.lower() == self.ON.lower()
+        operation = self.operation.lower()
 
-        # will be removed
-        self.startable = self.door.lower() == "closed" and \
-                         self.power.lower() == "on" and \
-                         self.remote_start_allowed and \
-                         self.operation.lower() not in ['delayedstart', 'run', 'finished', 'inactive']
-        self.started = self.power.lower() == "on" and \
-                       self.door.lower() == "closed" and \
-                       self.operation.lower() in ['delayedstart', 'run']
+        if power and operation == 'delayedstart':
+            self.state = self.STATE_DELAYED_STARTED
+        elif power and operation == 'run':
+            self.state = self.STATE_RUNNING
+            self.__previous_run_completed = False
+        elif power and operation == 'ready' and self.door.lower() == "closed" and self.__previous_run_completed and self.remote_start_allowed and self.program_remote_control_active:
+            self.state = self.STATE_STARTABLE
+        elif power and operation == 'finished':
+            self.state = self.STATE_FINISHED
+        else:
+            if self.door.lower() == 'open' or not power:
+                self.__previous_run_completed = True
+            if power and self.door.lower() == 'closed':
+                self.state = self.STATE_READY
+            elif power:
+                self.state = self.STATE_FINISHED
+            else:
+                self.state = self.OFF
 
+    def _notify_listeners(self):
+        self.__update_state()
         for value_changed_listener in self.__value_changed_listeners:
             value_changed_listener()
 
     def on_connected(self, event):
         logging.info(self.name + " has been connected (event stream). Reloading status/settings")
         self._reload_status_and_settings()
 
     def on_disconnected(self, event):
         logging.info(self.name + " has been disconnected (event stream)")
 
     def on_keep_alive_event(self, event):
-        self._notify_listeners()
+        try:
+            if (self.last_refresh + timedelta(minutes=30)) < datetime.now():
+                self._reload_status_and_settings()
+            self._notify_listeners()
+        except Exception as e:
+            logging.warning("error occurred processing keep alive event "+  str(e))
 
     def on_notify_event(self, event):
         self._on_value_changed_event(event)
 
     def on_status_event(self, event):
         self._on_value_changed_event(event)
 
@@ -165,14 +180,15 @@
             status = self._perform_get('/status').get('data', {}).get('status', {})
             self._on_values_changed(status, "reload status", notify_listeners=False)
 
             settings = self._perform_get('/settings').get('data', {}).get('settings', {})
             self._on_values_changed(settings, "reload settings")
         except Exception as e:
             if isinstance(e, OfflineException):
+                self._power = ""
                 logging.info(self.name + " is offline. Could not query current status/settings")
             else:
                 logging.warning(self.name + " error occurred on refreshing" + str(e))
 
     def _on_values_changed(self, changes: List[Dict[str, Any]], source: str, notify_listeners: bool = True):
         if len(changes) > 0:
             for change in changes:
@@ -203,15 +219,14 @@
             self._program_selected = change.get('value', None)
             logging.info(self.name + " field 'selected program': " + str(self._program_selected) + " (" + source + ")")
         elif key == 'BSH.Common.Option.ProgramProgress':
             self.__program_progress = change.get('value', None)
             logging.info(self.name + " field 'program progress': " + str(self.__program_progress) + " (" + source + ")")
         elif key == 'BSH.Common.Status.LocalControlActive':
             self.__program_local_control_active = change.get('value', None)
-            logging.info(self.name + " field 'local control active': " + str(self.__program_local_control_active) + " (" + source + ")")
         elif key == 'BSH.Common.Status.RemoteControlActive':
             self.program_remote_control_active = change.get('value', False)
             logging.info(self.name + " field 'remote control active': " + str(self.program_remote_control_active) + " (" + source + ")")
         elif key == 'BSH.Common.Setting.ChildLock': # supported by dishwasher, washer, dryer, ..
             self.child_lock = change.get('value', False)
             logging.info(self.name + " field 'child lock': " + str(self.child_lock) + " (" + source + ")")
         elif key == 'BSH.Common.Root.ActiveProgram':
@@ -258,17 +273,21 @@
         else:
             if response.status_code == 409:
                 msg = response.json()
                 if msg.get("error", {}).get('key', "") == "SDK.Error.HomeAppliance.Connection.Initialization.Failed":
                     raise OfflineException()
             raise Exception("error occurred by calling GET " + uri + " Got " + str(response.status_code) + " " + response.text)
 
-    def _perform_put(self, path:str, data: str, max_trials: int = 3, current_trial: int = 1):
+    def _perform_put(self, path:str, data: str, max_trials: int = 3, current_trial: int = 1, verbose: bool = False):
         uri = self._device_uri + path
+        if verbose:
+            logging.info("PUT " + uri + "\r\n" + json.dumps(data, indent=2))
         response = requests.put(uri, data=data, headers={"Content-Type": "application/json", "Authorization": "Bearer " + self._auth.access_token}, timeout=5000)
+        if verbose:
+            logging.info(str(response.status_code) + "\r\n" + response.text)
         if not is_success(response.status_code):
             logging.warning("error occurred by calling PUT (" + str(current_trial) + ". trial) " + uri + " " + data)
             logging.warning("got " + str(response.status_code) + " " + str(response.text))
             if current_trial <= max_trials:
                 delay = 1 + current_trial
                 logging.warning("waiting " + str(delay) + " sec for retry")
                 sleep(delay)
@@ -309,15 +328,14 @@
         self.program_water_forecast_percent = 0
         super().__init__(device_uri, auth, name, device_type, haid, brand, vib, enumber)
 
     def _on_value_changed(self, key: str, change: Dict[str, Any], source: str) -> bool:
         if key == 'BSH.Common.Option.StartInRelative':
             if 'value' in change.keys():
                 self.__program_start_in_relative_sec = change['value']
-                logging.info(self.name + " field 'start in relative': " + str(self.__program_start_in_relative_sec) + " (" + source + ")")
             if 'constraints' in change.keys():
                 constraints = change['constraints']
                 if 'max' in constraints.keys():
                     self.__program_start_in_relative_sec_max = constraints['max']
                     logging.info(self.name + " field 'start in relative max value': " + str(self.__program_start_in_relative_sec_max) + " (" + source + ")")
         elif key == 'Dishcare.Dishwasher.Option.ExtraDry':
             self.program_extra_try = change.get('value', False)
@@ -349,100 +367,112 @@
     def write_start_date(self, start_date: str):
         self._reload_status_and_settings()
         self._reload_selected_program()  # ensure that selected program is loaded
 
         if len(self._program_selected) == 0:
             logging.warning("ignoring start command. No program selected")
 
-        elif self.startable:
+        else:
             remaining_secs_to_wait = int((datetime.fromisoformat(start_date) - datetime.now()).total_seconds())
             if remaining_secs_to_wait < 0:
                 remaining_secs_to_wait = 0
-            if remaining_secs_to_wait > self.__program_start_in_relative_sec_max:
-                remaining_secs_to_wait = self.__program_start_in_relative_sec_max
+            if remaining_secs_to_wait >= self.__program_start_in_relative_sec_max:
+                logging.warning("remaining seconds to wait " + print_duration(remaining_secs_to_wait) + " is larger than max supported value of " + print_duration(self.__program_start_in_relative_sec_max) + ". Ignore setting start date")
 
-            # update starttime (already started in a delayed manner
-            if self.operation.lower() in ['delayedstart']:
+            # start in a delayed manner
+            if self.state == self.STATE_STARTABLE:
                 try:
                     data = {
                         "data": {
-                            "key": "BSH.Common.Option.StartInRelative",
-                            "value": remaining_secs_to_wait,
-                            "unit": "seconds"
+                            "key": self._program_selected,
+                            "options": [{
+                                "key": "BSH.Common.Option.StartInRelative",
+                                "value": remaining_secs_to_wait,
+                                "unit": "seconds"
+                            }]
                         }
                     }
 
-                    self._perform_put("/programs/active/options/BSH.Common.Option.StartInRelative", json.dumps(data, indent=2), max_trials=3)
-                    logging.info(self.name + " update start time: " + self.program_selected +
+                    self._perform_put("/programs/active", json.dumps(data, indent=2), max_trials=3)
+                    logging.info(self.name + " PROGRAMSTRART - program " + self.program_selected +
                                  " starts in " + print_duration(remaining_secs_to_wait) +
                                  " (duration " + print_duration(self.program_remaining_time_sec) + ")")
                 except Exception as e:
                     logging.warning("error occurred by starting " + self.name + " " + str(e))
 
-            # start in a delayed manner
-            else:
+            # update start time (already started in a delayed manner)
+            elif self.state == self.STATE_DELAYED_STARTED:
                 try:
                     data = {
                         "data": {
-                            "key": self._program_selected,
-                            "options": [{
-                                "key": "BSH.Common.Option.StartInRelative",
-                                "value": remaining_secs_to_wait,
-                                "unit": "seconds"
-                            }]
+                            "key": "BSH.Common.Option.StartInRelative",
+                            "value": remaining_secs_to_wait,
+                            "unit": "seconds"
                         }
                     }
 
-                    self._perform_put("/programs/active", json.dumps(data, indent=2), max_trials=3)
-                    logging.info(self.name + " PROGRAMSTRART - program " + self.program_selected +
+                    self._perform_put("/programs/active/options/BSH.Common.Option.StartInRelative", json.dumps(data, indent=2), max_trials=3)
+                    logging.info(self.name + " update start time: " + self.program_selected +
                                  " starts in " + print_duration(remaining_secs_to_wait) +
                                  " (duration " + print_duration(self.program_remaining_time_sec) + ")")
                 except Exception as e:
-                    logging.warning("error occurred by starting " + self.name + " " + str(e))
-        else:
-            logging.warning("ignoring start command. " + self.name + " is in state " + self._operation)
-        self._notify_listeners()
+                    logging.warning("error occurred by updating start time " + self.name + " " + str(e))
+
+            else:
+                logging.warning("ignoring start command. " + self.name + " is in state " + str(self.state))
+            self._notify_listeners()
+
+
+class FinishDate:
+
+    def __init__(self, start_date: str, program_duration_sec: int, remaining_secs_to_finish: int):
+        self.start_date = start_date
+        self.program_duration_sec = program_duration_sec
+        self.remaining_secs_to_finish = remaining_secs_to_finish
+
+    @staticmethod
+    def __compute_remaining_secs_to_finish(start_date: str, duration_sec: int, program_finish_in_relative_stepsize_sec: int) -> int:
+        remaining_secs_to_finish = int((datetime.fromisoformat(start_date) - datetime.now()).total_seconds()) + duration_sec
+        if remaining_secs_to_finish < 0:
+            logging.info("remaining_secs_to_finish is < 0. set it with 0")
+            remaining_secs_to_finish = 0
+        if remaining_secs_to_finish > 0 and program_finish_in_relative_stepsize_sec > 0:
+            remaining_secs_to_finish = int(remaining_secs_to_finish / program_finish_in_relative_stepsize_sec) * program_finish_in_relative_stepsize_sec
+        return remaining_secs_to_finish
+
+    @staticmethod
+    def create(start_date: str, program_duration_sec: int, program_finish_in_relative_stepsize_sec: int, program_finish_in_relative_max_sec: int):
+        remaining_secs_to_finish = FinishDate.__compute_remaining_secs_to_finish(start_date, program_duration_sec, program_finish_in_relative_stepsize_sec)
+        return FinishDate(start_date, program_duration_sec, remaining_secs_to_finish)
+
+    def __str__(self):
+        return "remaining seconds to finished " + str(self.remaining_secs_to_finish) + " (" + print_duration(self.remaining_secs_to_finish) + "). End time " + (datetime.fromisoformat(self.start_date) + timedelta(seconds=self.program_duration_sec)).strftime("%H:%M") + " (= start time " + datetime.fromisoformat(self.start_date).strftime("%H:%M") + " + " + print_duration(self.program_duration_sec) + " program duration)"
+
+    def __repr__(self):
+        return self.__str__()
 
 
 class FinishInAppliance(Appliance):
 
     def __init__(self, device_uri: str, auth: Auth, name: str, device_type: str, haid: str, brand: str, vib: str, enumber: str):
         self._program_finish_in_relative_sec = 0
         self.__program_finish_in_relative_max_sec = 86000
         self.__program_finish_in_relative_stepsize_sec = 60
+        self._durations = SimpleDB(haid + '_durations')
         super().__init__(device_uri, auth, name, device_type, haid, brand, vib, enumber)
-        self.__durations = self.__load_durations()
-
-    def __load_durations(self):
-        durations = {}
-        try:
-            with open(self.__file(), 'r') as file:
-                durations = json.load(file)
-                logging.info("config " + str(durations) + " loaded (" + self.__file() + ")")
-        except Exception as e:
-            logging.info("error reading " + self.__file() + " " + str(e))
-        return durations
-
-    def __file(self) -> str:
-        dir = site_data_dir("HomeConnect", appauthor=False)
-        if not exists(dir):
-            makedirs(dir)
-        file = join(dir, self.haid + '_config.json')
-        return file
 
     def _on_value_changed(self, key: str, change: Dict[str, Any], source: str) -> bool:
         if key == 'BSH.Common.Status.OperationState':
             operation = change.get('value', "undefined")
             if operation != self._operation:
                 logging.info(self.name + " field 'operation state': " + str(operation) + ". previous state = " + str(self._operation) + " (" + source + ")")
                 self._operation = operation
         elif key == 'BSH.Common.Option.FinishInRelative':  # supported by dryer & washer only
             if 'value' in change.keys():
                 self._program_finish_in_relative_sec = int(change['value'])
-                logging.info(self.name + " field 'finish in relative': " + str(self._program_finish_in_relative_sec) + " (" + source + ")")
             if 'constraints' in change.keys():
                 constraints = change['constraints']
                 if 'max' in constraints.keys():
                     self.__program_finish_in_relative_max_sec = constraints['max']
                     logging.info(self.name + " field 'program_finish_in_relative_max_sec: " + str(self.__program_finish_in_relative_max_sec) + " (" + source + ")")
                 if 'stepsize' in constraints.keys():
                     self.__program_finish_in_relative_stepsize_sec = constraints['stepsize']
@@ -456,79 +486,80 @@
             # unhandled
             return super()._on_value_changed(key, change, source)
         return True
 
     def read_start_date(self) -> str:
         if self.operation.lower() == 'delayedstart' and self._program_finish_in_relative_sec > 0:
             start_date = datetime.now() + timedelta(seconds=self._program_finish_in_relative_sec) - timedelta(seconds=self.__program_duration_sec())
-            return start_date.strftime("%Y-%m-%d %H:%M")
+            return start_date.strftime("%Y-%m-%dT%H:%M")
         else:
             return ""
 
     def _program_fingerprint(self) -> str:
         return self._program_selected
 
     @property
     def program_duration_hours(self) -> float:
         return round(self.__program_duration_sec() / (60*60), 1)
 
     def __program_duration_sec(self):
         # will update props, if duration is available
         program_fingerprint = self._program_fingerprint()
-        if len(self.program_selected) > 0 and self._program_finish_in_relative_sec > 0 and self.operation.lower() not in ['delayedstart', 'run', 'finished', 'inactive']:
-            if self.__durations.get(program_fingerprint, "?") != self._program_finish_in_relative_sec:   # duration changed?
-                self.__durations[program_fingerprint] = self._program_finish_in_relative_sec
-                logging.info("duration update for " + program_fingerprint + " with " + str(self._program_finish_in_relative_sec))
-                with open(self.__file(), 'w') as file:
-                    json.dump(self.__durations, file)
+        if len(self.program_selected) > 0 and self._program_finish_in_relative_sec > 0 and self.state == self.STATE_READY:
+            if self._durations.get(program_fingerprint, -1) != self._program_finish_in_relative_sec:   # duration changed?
+                if self._program_finish_in_relative_sec < 5 * 60 * 60:
+                    self._durations.put(program_fingerprint, self._program_finish_in_relative_sec)
+                    logging.info("duration update for " + program_fingerprint + " with " + str(self._program_finish_in_relative_sec))
+                else:
+                    logging.info("duration update for " + program_fingerprint + " with " + str(self._program_finish_in_relative_sec) + " ignored. Value seems to high")
 
         # get duration
-        duration_sec = self.__durations.get(program_fingerprint, None)
+        duration_sec = self._durations.get(program_fingerprint, None)
         if duration_sec is None:
-            logging.warning("no duration stored. Using default (key: " + program_fingerprint + " available values: " + str(self.__durations) + ")")
+            logging.warning("no duration stored. Using default (key: " + program_fingerprint + " available values: " + ", ".join([key + ": " + str(self._durations.get(key)) for key in self._durations.keys()]) + ")")
             return 7222  # 2h
         else:
             return duration_sec
 
-    def __compute_remaining_secs_to_finish(self, start_date: str, duration_sec: int) -> int:
-        remaining_secs_to_finish = int((datetime.fromisoformat(start_date) - datetime.now()).total_seconds()) + duration_sec
-        if remaining_secs_to_finish < 0:
-            logging.info("remaining_secs_to_finish is < 0. set it with 0")
-            remaining_secs_to_finish = 0
-        if remaining_secs_to_finish > 0 and self.__program_finish_in_relative_stepsize_sec > 0:
-            remaining_secs_to_finish = int(remaining_secs_to_finish / self.__program_finish_in_relative_stepsize_sec) * self.__program_finish_in_relative_stepsize_sec
-        return remaining_secs_to_finish
-
     def write_start_date(self, start_date: str):
         logging.info("starting device at " + start_date)
 
         # ensure that current settings and selected program is loaded
         self._reload_status_and_settings()
         self._reload_selected_program()
 
         # when startable
-        if self.startable:
+        if self.state == self.STATE_STARTABLE:
             program_duration_sec = self.__program_duration_sec()
-            data = {
-                "data": {
-                    "key": self._program_selected,
-                    "options": [{
-                        "key": "BSH.Common.Option.FinishInRelative",
-                        "value": self.__compute_remaining_secs_to_finish(start_date, program_duration_sec),
-                        "unit": "seconds"
-                    }]
-                }
-            }
-            try:
-                self._perform_put("/programs/active", json.dumps(data, indent=2), max_trials=3)
-                logging.info(self.name + " program " + self.program_selected + " starts at " + start_date + " (duration " + str(round(program_duration_sec/(60*60), 1)) + " h)")
-            except Exception as e:
-                logging.warning("error occurred by starting " + self.name + " with program " + self.program_selected + " at " + start_date + " (duration: " + str(round(program_duration_sec/(60*60), 1)) + " h) " + str(e))
+            finish_date = FinishDate.create(start_date, program_duration_sec, self.__program_finish_in_relative_stepsize_sec, self.__program_finish_in_relative_max_sec)
+            if finish_date.remaining_secs_to_finish >= self.__program_finish_in_relative_max_sec:
+                logging.warning("remaining seconds to finished " + print_duration(finish_date.remaining_secs_to_finish) + " is larger than max supported value of " + print_duration(self.__program_finish_in_relative_max_sec) + ". Ignore setting start date")
+            else:
+                try:
+                    data = {
+                        "data": {
+                            "key": self._program_selected,
+                            "options": [{
+                                "key": "BSH.Common.Option.FinishInRelative",
+                                "value": finish_date.remaining_secs_to_finish,
+                                "unit": "seconds"
+                            }]
+                        }
+                    }
+                    self._perform_put("/programs/active", json.dumps(data, indent=2), max_trials=3, verbose=True)
+                    logging.info(self.name + " program " + self.program_selected + " starts at " + start_date + " -> " + str(finish_date))
+                except Exception as e:
+                    logging.warning("error occurred by starting " + self.name + " with program " + self.program_selected + " at " + start_date + " (duration: " + str(round(program_duration_sec/(60*60), 1)) + " h) " + str(e))
+
+        # update end time
+        elif self.state == self.STATE_DELAYED_STARTED:
+            logging.warning("updating start time currently not supported")
         else:
-            logging.warning(self.name + " not startable. Ignoring start command.")
+            logging.warning(self.name + " is in state " + str(self.state) + " Ignoring start command.")
+
 
 
 class Washer(FinishInAppliance):
     DeviceType = 'washer'
 
     def __init__(self, device_uri: str, auth: Auth, name: str, device_type: str, haid: str, brand: str, vib: str, enumber: str):
         self.idos1_baselevel = 0
```

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/appliances_webthing.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/appliances_webthing.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,23 +114,23 @@
                      metadata={
                          'title': 'Door State',
                          "type": "string",
                          'description': 'Door State. See https://api-docs.home-connect.com/states?#door-state',
                          'readOnly': True,
                      }))
 
-        self.status = Value(appliance.status)
+        self.state = Value(appliance.state)
         self.add_property(
             Property(self,
-                     'status',
-                     self.status,
+                     'state',
+                     self.state,
                      metadata={
-                         'title': 'status',
+                         'title': 'State',
                          "type": "string",
-                         'description': 'The status',
+                         'description': 'The state (valid values ' + ", ".join(appliance.VALID_STATES) + ')',
                          'readOnly': True,
                      }))
 
         self.operation = Value(appliance.operation)
         self.add_property(
             Property(self,
                      'operation',
@@ -150,38 +150,14 @@
                      metadata={
                          'title': 'Remote Start Allowed State',
                          "type": "boolean",
                          'description': 'Remote Start Allowance State. See https://api-docs.home-connect.com/states?#remote-start-allowance-state',
                          'readOnly': True,
                      }))
 
-        self.startable = Value(appliance.startable)
-        self.add_property(
-            Property(self,
-                     'startable',
-                     self.startable,
-                     metadata={
-                         'title': 'Startable',
-                         "type": "boolean",
-                         'description': 'True, if the appliance can be started remotely',
-                         'readOnly': True,
-                     }))
-
-        self.started = Value(appliance.started)
-        self.add_property(
-            Property(self,
-                     'started',
-                     self.started,
-                     metadata={
-                         'title': 'Started',
-                         "type": "boolean",
-                         'description': 'True, if the appliance is (delayed) started',
-                         'readOnly': True,
-                     }))
-
         self.remote_control_active = Value(appliance.program_remote_control_active)
         self.add_property(
             Property(self,
                      'remote_control_active',
                      self.remote_control_active,
                      metadata={
                          'title': 'Remote Control active',
@@ -223,17 +199,15 @@
         self.ioloop.add_callback(self._on_value_changed, self.appliance)
 
     def _on_value_changed(self, appliance):
         self.power.notify_of_external_update(self.appliance.power)
         self.door.notify_of_external_update(self.appliance.door)
         self.operation.notify_of_external_update(self.appliance.operation)
         self.remote_start_allowed.notify_of_external_update(self.appliance.remote_start_allowed)
-        self.status.notify_of_external_update(self.appliance.status)
-        self.startable.notify_of_external_update(self.appliance.startable)
-        self.started.notify_of_external_update(self.appliance.started)
+        self.state.notify_of_external_update(self.appliance.state)
         self.remote_control_active.notify_of_external_update(self.appliance.program_remote_control_active)
         self.enumber.notify_of_external_update(self.appliance.enumber)
         self.vib.notify_of_external_update(self.appliance.vib)
         self.brand.notify_of_external_update(self.appliance.brand)
         self.haid.notify_of_external_update(self.appliance.haid)
         self.name.notify_of_external_update(self.appliance.name)
         self.device_type.notify_of_external_update(self.appliance.device_type)
```

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/auth.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import requests
+import uuid
 import webbrowser
 from os import path
 from datetime import datetime, timedelta
 from urllib.parse import urlsplit, parse_qs
 from typing import Optional
 
 
@@ -31,21 +32,24 @@
 class Auth:
 
     URI = "https://api.home-connect.com/security"
     DEFAULT_FILENAME = "homeconnect_oauth.txt"
 
     @staticmethod
     def create(client_id: str, client_secret:str, scope: str = "IdentifyAppliance%20Dishwasher%20Dryer%20Washer"):
-        uri = Auth.URI + "/oauth/authorize?response_type=code&client_id=" + client_id + "&scope=" + scope
+        state = str(uuid.uuid4())
+        uri = Auth.URI + "/oauth/authorize?response_type=code&client_id=" + client_id + "&scope=" + scope + "&state=" + state
         webbrowser.open(uri)
 
         auth_result = input("Please enter the URL redirected to: ")
         query = urlsplit(auth_result).query
         params = parse_qs(query)
         authorization_code = params['code']
+        if params['state'][0] != state:
+            raise Exception("state mismatch")  # refer https://auth0.com/docs/secure/attack-protection/state-parameters
 
         data = {"client_id": client_id,
                 "client_secret": client_secret,
                 "grant_type": "authorization_code",
                 "code": authorization_code}
         response = requests.post(Auth.URI + '/oauth/token', data=data)
         data = response.json()
```

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/eventstream.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/eventstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
                         if remaining_secs_next_reconnect <= 0:
                             self.close("Max lifetime " + print_duration(self.max_lifetime_sec) + " reached (periodic reconnect)")
 
                         if self.stream is None:
                             return
                 except Exception as e:
+                    #traceback.print_exc()
                     if datetime.now() > (connect_time + timedelta(seconds=self.max_lifetime_sec)):
                         self.close("Max lifetime " + print_duration(self.max_lifetime_sec) + " reached (periodic reconnect)")
                     else:
                         raise e
             else:
                 if self.response.headers.get('Content-Type', 'text/event-stream').lower() == 'text/event-stream':
                     raise Exception("opening event stream returns " + str(self.response.status_code))
```

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing/homeconnect.py` & `homeconnect_webthing-1.0.0/homeconnect_webthing/homeconnect.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/PKG-INFO` & `homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homeconnect-webthing
-Version: 0.3.9
+Version: 1.0.0
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `homeconnect_webthing-0.3.9/homeconnect_webthing.egg-info/SOURCES.txt` & `homeconnect_webthing-1.0.0/homeconnect_webthing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

