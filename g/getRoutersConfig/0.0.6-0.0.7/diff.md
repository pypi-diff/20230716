# Comparing `tmp/getRoutersConfig-0.0.6.tar.gz` & `tmp/getRoutersConfig-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getRoutersConfig-0.0.6.tar", last modified: Mon Jun 12 18:56:37 2023, max compression
+gzip compressed data, was "getRoutersConfig-0.0.7.tar", last modified: Sun Jul 16 15:34:31 2023, max compression
```

## Comparing `getRoutersConfig-0.0.6.tar` & `getRoutersConfig-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.292899 getRoutersConfig-0.0.6/
--rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5294 2023-06-12 18:56:37.291898 getRoutersConfig-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.250900 getRoutersConfig-0.0.6/app/
-drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.259898 getRoutersConfig-0.0.6/app/getRoutersConfig/
--rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.289900 getRoutersConfig-0.0.6/app/getRoutersConfig/src/
--rw-rw-rw-   0        0        0    11727 2023-06-12 16:51:26.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/CiscoClass.py
--rw-rw-rw-   0        0        0     9156 2023-06-12 18:56:34.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/HuaweiClass.py
--rw-rw-rw-   0        0        0     1216 2023-06-10 12:08:16.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/RouterClass.py
--rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/__init__.py
--rw-rw-rw-   0        0        0     2449 2023-05-30 15:46:22.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/main.py
--rw-rw-rw-   0        0        0      601 2023-06-10 12:42:51.000000 getRoutersConfig-0.0.6/app/getRoutersConfig/src/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-12 18:56:37.272900 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/
--rw-rw-rw-   0        0        0     5294 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 18:56:37.000000 getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 18:56:37.292899 getRoutersConfig-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-06-10 14:20:15.000000 getRoutersConfig-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:34:31.332884 getRoutersConfig-0.0.7/
+-rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5271 2023-07-16 15:34:31.330886 getRoutersConfig-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 15:34:31.257884 getRoutersConfig-0.0.7/app/
+drwxrwxrwx   0        0        0        0 2023-07-16 15:34:31.282886 getRoutersConfig-0.0.7/app/getRoutersConfig/
+-rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:34:31.323889 getRoutersConfig-0.0.7/app/getRoutersConfig/src/
+-rw-rw-rw-   0        0        0    11727 2023-07-16 15:24:43.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/src/CiscoClass.py
+-rw-rw-rw-   0        0        0     9043 2023-07-16 15:24:51.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/src/HuaweiClass.py
+-rw-rw-rw-   0        0        0     1216 2023-06-10 12:08:16.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/src/RouterClass.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/src/__init__.py
+-rw-rw-rw-   0        0        0     2462 2023-07-16 14:53:25.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/src/main.py
+-rw-rw-rw-   0        0        0      601 2023-06-10 12:42:51.000000 getRoutersConfig-0.0.7/app/getRoutersConfig/src/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-16 15:34:31.301886 getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/
+-rw-rw-rw-   0        0        0     5271 2023-07-16 15:34:31.000000 getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-07-16 15:34:31.000000 getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 15:34:31.000000 getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-16 15:34:31.000000 getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-16 15:34:31.000000 getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 15:34:31.333887 getRoutersConfig-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-07-16 15:26:36.000000 getRoutersConfig-0.0.7/setup.py
```

### Comparing `getRoutersConfig-0.0.6/LICENSE` & `getRoutersConfig-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.6/PKG-INFO` & `getRoutersConfig-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.6
-Summary: get Cisco routers configuration as Json
+Version: 0.0.7
+Summary: get Cisco and Huawei routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -49,16 +49,15 @@
         "years": 0,
         "weeks": 1,
         "days": 1,
         "hours": 11,
         "minutes": 25
     },
     "system_image": "c800-universalk9-mz.SPA.154-3.M6.bin",
-    "serial_number": "FCZ1234A5BC",
-    "config_register": "0x2102"
+    "serial_number": "FCZ1234A5BC"
 }
 ```
 
 # Get Ipv4 static routes
 ```python
 from getRoutersConfig import setInformations
```

### Comparing `getRoutersConfig-0.0.6/app/getRoutersConfig/src/CiscoClass.py` & `getRoutersConfig-0.0.7/app/getRoutersConfig/src/CiscoClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.6/app/getRoutersConfig/src/HuaweiClass.py` & `getRoutersConfig-0.0.7/app/getRoutersConfig/src/HuaweiClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,14 @@
         re_serial_number = r'ESN of device: (?P<serial_number>\S+)'
 
         match_serie_version_image = re.search(re_serie_version_image, output, flags=re.M)
         match_hostname = re.search(re_hostname, hostname, flags=re.M)
         match_model_uptime = re.search(re_model_uptime, output, flags=re.M)
         match_serial_number = re.search(re_serial_number, serial_number, flags=re.M)
 
-        print(match_serie_version_image)
-        print(match_hostname)
-        print(match_serial_number)
-
-
         return {
             "serie": match_serie_version_image.group('serie'),
             "model": match_model_uptime.group('model'),
             "version": match_serie_version_image.group('version'),
             "hostname": match_hostname.group('hostname'),
             "uptime": {
                 "years": int(match_model_uptime.group('years')) if match_model_uptime.group('years') else 0,
```

### Comparing `getRoutersConfig-0.0.6/app/getRoutersConfig/src/RouterClass.py` & `getRoutersConfig-0.0.7/app/getRoutersConfig/src/RouterClass.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.6/app/getRoutersConfig/src/main.py` & `getRoutersConfig-0.0.7/app/getRoutersConfig/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     net_connect = ConnectHandler(**host)
 
     time.sleep(3)
 
     if bastion_ip:
 
-        net_connect.write_channel(f"snmpwalk -v2c -c covareck {host_ip} SNMPv2-MIB::sysDescr\n")
+        net_connect.write_channel(f"snmpwalk -v2c -c {host_snmp_community} {host_ip} SNMPv2-MIB::sysDescr\n")
         net_connect.write_channel(f"ssh {host_ip}\r\n")
 
         time.sleep(2)
         output = net_connect.read_channel()
         if "huawei" in output.lower():
             device_type = "huawei"
         elif "cisco" in output.lower():
```

### Comparing `getRoutersConfig-0.0.6/app/getRoutersConfig/src/tools.py` & `getRoutersConfig-0.0.7/app/getRoutersConfig/src/tools.py`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.6/app/getRoutersConfig.egg-info/PKG-INFO` & `getRoutersConfig-0.0.7/app/getRoutersConfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.6
-Summary: get Cisco routers configuration as Json
+Version: 0.0.7
+Summary: get Cisco and Huawei routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
@@ -49,16 +49,15 @@
         "years": 0,
         "weeks": 1,
         "days": 1,
         "hours": 11,
         "minutes": 25
     },
     "system_image": "c800-universalk9-mz.SPA.154-3.M6.bin",
-    "serial_number": "FCZ1234A5BC",
-    "config_register": "0x2102"
+    "serial_number": "FCZ1234A5BC"
 }
 ```
 
 # Get Ipv4 static routes
 ```python
 from getRoutersConfig import setInformations
```

### Comparing `getRoutersConfig-0.0.6/setup.py` & `getRoutersConfig-0.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="getRoutersConfig",
-    version="0.0.6",
-    description="get Cisco routers configuration as Json",
+    version="0.0.7",
+    description="get Cisco and Huawei routers configuration as Json",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanielRicklin/getRoutersConfig",
     author="DanielRicklin",
     author_email="ricklin.daniel@outlook.fr",
```

