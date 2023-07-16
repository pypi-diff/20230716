# Comparing `tmp/ciscopykit-1.5.2.tar.gz` & `tmp/ciscopykit-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscopykit-1.5.2.tar", last modified: Wed Jul 12 20:31:08 2023, max compression
+gzip compressed data, was "ciscopykit-1.5.3.tar", last modified: Sun Jul 16 17:07:34 2023, max compression
```

## Comparing `ciscopykit-1.5.2.tar` & `ciscopykit-1.5.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.535171 ciscopykit-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-12 20:31:08.535171 ciscopykit-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.527171 ciscopykit-1.5.2/ciscopykit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.531171 ciscopykit-1.5.2/ciscopykit/help/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/help/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.531171 ciscopykit-1.5.2/ciscopykit/lan_security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/dhcp_snooping.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/dynamic_arp_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/stp_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/switchport_security.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/lan_security/vlan_security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.531171 ciscopykit-1.5.2/ciscopykit/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/services/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/services/dhcp_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/services/pat_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.535171 ciscopykit-1.5.2/ciscopykit/switch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/switch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/switch/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/switch/l2_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/switch/l3_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/switch/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.535171 ciscopykit-1.5.2/ciscopykit/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/templates/generate_router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/templates/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.535171 ciscopykit-1.5.2/ciscopykit/vlan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/vlan/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/ciscopykit/vlan/vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:31:08.527171 ciscopykit-1.5.2/ciscopykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-12 20:31:08.000000 ciscopykit-1.5.2/ciscopykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-12 20:31:08.000000 ciscopykit-1.5.2/ciscopykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:31:08.000000 ciscopykit-1.5.2/ciscopykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-12 20:31:08.000000 ciscopykit-1.5.2/ciscopykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 20:31:08.000000 ciscopykit-1.5.2/ciscopykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 20:31:08.000000 ciscopykit-1.5.2/ciscopykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:31:08.535171 ciscopykit-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-12 20:30:50.000000 ciscopykit-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.584844 ciscopykit-1.5.3/ciscopykit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.584844 ciscopykit-1.5.3/ciscopykit/help/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/help/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/lan_security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/dhcp_snooping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/dynamic_arp_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/stp_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/switchport_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/lan_security/vlan_security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/dhcp_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/services/pat_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/switch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/l2_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/l3_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/switch/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/templates/generate_router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/templates/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/ciscopykit/vlan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/vlan/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/ciscopykit/vlan/vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:07:34.584844 ciscopykit-1.5.3/ciscopykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 17:07:34.000000 ciscopykit-1.5.3/ciscopykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:07:34.588844 ciscopykit-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-16 17:07:18.000000 ciscopykit-1.5.3/setup.py
```

### Comparing `ciscopykit-1.5.2/LICENSE.md` & `ciscopykit-1.5.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/PKG-INFO` & `ciscopykit-1.5.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.5.2
+Version: 1.5.3
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.5.2/README.md` & `ciscopykit-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/app.py` & `ciscopykit-1.5.3/ciscopykit/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/device.py` & `ciscopykit-1.5.3/ciscopykit/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         """
         Returns the list of active interfaces.
 
         Returns:
             list: The list of active interfaces.
         """
         return self.active_interfaces
-        @staticmethod
+    @staticmethod
     def generate_init_config(hostname, site, interface_range="GigabitEthernet0/0-10", static_pass="cisco", motd="Welcome to the Cisco network!"):
         """
         Generates the initial configuration for the device.
 
         Args:
             hostname (str): The hostname to be set in the configuration.
             site (str): The site name to be used in the configuration.
```

### Comparing `ciscopykit-1.5.2/ciscopykit/entry_point.py` & `ciscopykit-1.5.3/ciscopykit/entry_point.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/interface.py` & `ciscopykit-1.5.3/ciscopykit/interface.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/lan_security/switchport_security.py` & `ciscopykit-1.5.3/ciscopykit/lan_security/switchport_security.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def configure_switchport_security(interface, max_mac, violation_action='restrict', aging_time=None, sticky_mac=True):
+def generate_switchport_security_config(interface, max_mac, violation_action='restrict', aging_time=None, sticky_mac=True):
     """
     Generate the configuration command for switchport security.
 
     Args:
         interface (str): Interface name.
         max_mac (int): Maximum number of MAC addresses to be learned.
         violation_action (str, optional): Violation action. Can be 'restrict', 'protect', or 'shutdown'. (default: 'restrict')
```

### Comparing `ciscopykit-1.5.2/ciscopykit/services/app.py` & `ciscopykit-1.5.3/ciscopykit/services/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/services/dhcp_service.py` & `ciscopykit-1.5.3/ciscopykit/services/dhcp_service.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/services/pat_service.py` & `ciscopykit-1.5.3/ciscopykit/services/pat_service.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/switch/app.py` & `ciscopykit-1.5.3/ciscopykit/switch/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/switch/l3_switch.py` & `ciscopykit-1.5.3/ciscopykit/switch/l3_switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/switch/switch.py` & `ciscopykit-1.5.3/ciscopykit/switch/switch.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/templates/generate_router_config.py` & `ciscopykit-1.5.3/ciscopykit/templates/generate_router_config.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/vlan/app.py` & `ciscopykit-1.5.3/ciscopykit/vlan/app.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit/vlan/vlan.py` & `ciscopykit-1.5.3/ciscopykit/vlan/vlan.py`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/ciscopykit.egg-info/PKG-INFO` & `ciscopykit-1.5.3/ciscopykit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscopykit
-Version: 1.5.2
+Version: 1.5.3
 Summary: A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer
 Home-page: https://github.com/Vincent-de-Torres-Portfolio/ciscopykit
 Author: devinci-it
 Author-email: vince.dev@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ciscopykit-1.5.2/ciscopykit.egg-info/SOURCES.txt` & `ciscopykit-1.5.3/ciscopykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ciscopykit-1.5.2/setup.py` & `ciscopykit-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ciscopykit',
-    version='1.5.2',
+    version='1.5.3',
     author='devinci-it',
     author_email='vince.dev@icloud.com',
     description='A network management toolkit for Cisco devices keeping track of devices when using GNS3 / Cisco Packet Tracer',
     long_description='''A network management toolkit for Cisco devices. It provides classes and methods to manage network devices, interfaces, and configurations.''',
     url='https://github.com/Vincent-de-Torres-Portfolio/ciscopykit',
     packages=find_packages(),
     classifiers=[
```

