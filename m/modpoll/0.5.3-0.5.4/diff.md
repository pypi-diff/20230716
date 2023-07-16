# Comparing `tmp/modpoll-0.5.3.tar.gz` & `tmp/modpoll-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modpoll-0.5.3.tar", max compression
+gzip compressed data, was "modpoll-0.5.4.tar", max compression
```

## Comparing `modpoll-0.5.3.tar` & `modpoll-0.5.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-03-27 15:28:13.637625 modpoll-0.5.3/LICENSE
--rw-r--r--   0        0        0     9516 2023-03-27 15:28:13.637625 modpoll-0.5.3/README.md
--rw-r--r--   0        0        0      214 2023-03-27 15:28:13.683628 modpoll-0.5.3/modpoll/__init__.py
--rw-r--r--   0        0        0       28 2023-03-27 15:28:13.684628 modpoll-0.5.3/modpoll/__main__.py
--rw-r--r--   0        0        0     4345 2023-03-27 15:28:13.684628 modpoll-0.5.3/modpoll/arg_parser.py
--rw-r--r--   0        0        0     3612 2023-03-27 15:28:13.684628 modpoll-0.5.3/modpoll/main.py
--rw-r--r--   0        0        0    19542 2023-03-27 15:28:13.684628 modpoll-0.5.3/modpoll/modbus_task.py
--rw-r--r--   0        0        0     4675 2023-03-27 15:28:13.684628 modpoll-0.5.3/modpoll/mqtt_task.py
--rw-r--r--   0        0        0      821 2023-03-27 15:28:13.685628 modpoll-0.5.3/pyproject.toml
--rw-r--r--   0        0        0    10757 1970-01-01 00:00:00.000000 modpoll-0.5.3/setup.py
--rw-r--r--   0        0        0    10401 1970-01-01 00:00:00.000000 modpoll-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-16 11:17:34.360655 modpoll-0.5.4/LICENSE
+-rw-r--r--   0        0        0     9516 2023-07-16 11:17:34.360655 modpoll-0.5.4/README.md
+-rw-r--r--   0        0        0      214 2023-07-16 11:17:34.393655 modpoll-0.5.4/modpoll/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-16 11:17:34.393655 modpoll-0.5.4/modpoll/__main__.py
+-rw-r--r--   0        0        0     4467 2023-07-16 11:17:34.393655 modpoll-0.5.4/modpoll/arg_parser.py
+-rw-r--r--   0        0        0     3617 2023-07-16 11:17:34.393655 modpoll-0.5.4/modpoll/main.py
+-rw-r--r--   0        0        0    19640 2023-07-16 11:17:34.394655 modpoll-0.5.4/modpoll/modbus_task.py
+-rw-r--r--   0        0        0     4675 2023-07-16 11:17:34.394655 modpoll-0.5.4/modpoll/mqtt_task.py
+-rw-r--r--   0        0        0      821 2023-07-16 11:17:34.394655 modpoll-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0    10757 1970-01-01 00:00:00.000000 modpoll-0.5.4/setup.py
+-rw-r--r--   0        0        0    10401 1970-01-01 00:00:00.000000 modpoll-0.5.4/PKG-INFO
```

### Comparing `modpoll-0.5.3/LICENSE` & `modpoll-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modpoll-0.5.3/README.md` & `modpoll-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `modpoll-0.5.3/modpoll/arg_parser.py` & `modpoll-0.5.4/modpoll/arg_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,16 @@
                         help='Baud rate for serial port. Defaults to 9600')
     parser.add_argument('--rtu-parity', default='none', choices=['none', 'odd', 'even'],
                         help='Parity for serial port. Defaults to none')
     parser.add_argument('--timeout', default=3.0, type=float,
                         help='Response time-out seconds for MODBUS devices, Defaults to 3.0')
     parser.add_argument('-o', '--export', default=None,
                         help='The file name to export references/registers')
+    parser.add_argument('-p', '--print-result', action='store_true',
+                        help='Print received data.')
     parser.add_argument('--mqtt-host', default=None,
                         help='MQTT server address. Skip MQTT setup if not specified')
     parser.add_argument('--mqtt-port', default=1883, type=int,
                         help='1883 for non-TLS or 8883 for TLS, Defaults to 1883')
     parser.add_argument('--mqtt-clientid', default=None,
                         help='MQTT client name, If qos > 0, set unique name for multiple clients')
     parser.add_argument('--mqtt-topic-prefix', default='modpoll/',
@@ -46,20 +48,20 @@
                         help='Use TLS')
     parser.add_argument('--mqtt-insecure', action='store_true',
                         help='Use TLS without providing certificates')
     parser.add_argument('--mqtt-cacerts', default=None,
                         help="Path to ca keychain")
     parser.add_argument('--mqtt-tls-version', default=None, choices=['tlsv1.2', 'tlsv1.1', 'tlsv1'],
                         help='TLS protocol version, can be one of tlsv1.2 tlsv1.1 or tlsv1')
+    parser.add_argument('--mqtt-single', action='store_true',
+                        help='Publish each value in a single topic. If not specified groups all values in a single topic.')
     parser.add_argument('--diagnostics-rate', default=0, type=float,
                         help='Time in seconds as publishing period for each device diagnostics')
     parser.add_argument('--autoremove', action='store_true',
                         help='Automatically remove poller if modbus communication has failed 3 times.')
     parser.add_argument('--loglevel', default='INFO', choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
                         help='Set log level, Defaults to INFO')
     parser.add_argument('--timestamp', action='store_true',
                         help='Add timestamp to the result')
     parser.add_argument('--delay', default=0, type=int,
                         help='Time to delay sending first request in seconds after connecting. Default to 0')
-    parser.add_argument('--mqtt-single', action='store_true',
-                        help='Publish each value in a single topic. If not specified groups all values in a single topic.')
     return parser
```

### Comparing `modpoll-0.5.3/modpoll/main.py` & `modpoll-0.5.4/modpoll/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from datetime import timezone
 import sys
 import signal
 import json
 
 from modpoll.arg_parser import get_parser
 from modpoll.mqtt_task import mqttc_setup, mqttc_close, mqttc_receive
-from modpoll.modbus_task import modbus_setup, modbus_poll, modbus_publish, modbus_publish_diagnostics, modbus_export, modbus_close, modbus_write_coil, modbus_write_register
+from modpoll.modbus_task import modbus_setup, modbus_poll, modbus_publish, modbus_publish_diagnostics, modbus_export, \
+    modbus_close, modbus_write_coil, modbus_write_register
 
 LOG_SIMPLE = "%(asctime)s | %(levelname).1s | %(name)s | %(message)s"
 log = None
 event_exit = threading.Event()
 
 
 def _signal_handler(signal, frame):
@@ -94,15 +95,15 @@
         if topic and payload:
             device_name = re.search(f"^{args.mqtt_topic_prefix}([^/\n]*)/set", topic).group(1)
             if device_name:
                 try:
                     reg = json.loads(payload)
                     if "coil" == reg["object_type"]:
                         if modbus_write_coil(device_name, reg["address"], reg["value"]):
-                            log.info(f"")
+                            log.info("")
                     elif "holding_register" == reg["object_type"]:
                         modbus_write_register(device_name, reg["address"], reg["value"])
                 except json.decoder.JSONDecodeError:
                     log.warning(f"Fail to parse json message: {payload}")
         if args.once:
             event_exit.set()
             break
```

### Comparing `modpoll-0.5.3/modpoll/modbus_task.py` & `modpoll-0.5.4/modpoll/modbus_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,28 +274,28 @@
                 log.error("No device to add poller.")
                 continue
             if "coil" == fc:
                 function_code = 1
                 if size > 2000:  # some implementations don't seem to support 2008 coils/inputs
                     log.error("Too many coils (max. 2000). Ignoring poller.")
                     continue
-            elif "input_status" == fc:
+            elif "discrete_input" == fc:
                 function_code = 2
                 if size > 2000:
-                    log.error("Too many inputs (max. 2000). Ignoring poller.")
+                    log.error("Too many discrete inputs (max. 2000). Ignoring poller.")
                     continue
             elif "holding_register" == fc:
                 function_code = 3
                 if size > 123:  # applies to TCP, RTU should support 125 registers. But let's be safe.
-                    log.error("Too many registers (max. 123). Ignoring poller.")
+                    log.error("Too many holding registers (max. 123). Ignoring poller.")
                     continue
             elif "input_register" == fc:
                 function_code = 4
                 if size > 123:
-                    log.error(f"Too many registers (max. 123). Ignoring poller.")
+                    log.error(f"Too many input registers (max. 123): {size}. Ignoring poller.")
                     continue
             else:
                 log.warning(f"Unknown function code ({fc}) ignoring poller.")
                 continue
             current_poller = Poller(current_device, function_code, start_address, size, endian)
             current_device.pollerList.append(current_poller)
             log.info(f"Add poller (start_address={current_poller.start_address}, size={current_poller.size}) "
@@ -332,15 +332,15 @@
 def load_config(file):
     try:
         with requests.Session() as s:
             response = s.get(file)
             decoded_content = response.content.decode('utf-8')
             csv_reader = csv.reader(decoded_content.splitlines(), delimiter=',')
             parse_config(csv_reader)
-    except requests.RequestException as exception:
+    except requests.RequestException:
         with open(file, "r") as f:
             f.seek(0)
             csv_reader = csv.reader(f)
             parse_config(csv_reader)
 
 
 def modbus_setup(config, event):
@@ -358,15 +358,15 @@
         if args.rtu_parity == "odd":
             parity = "O"
         elif args.rtu_parity == "even":
             parity = "E"
         else:
             parity = "N"
         master = ModbusSerialClient(method="rtu", port=args.rtu, stopbits=1, bytesize=8, parity=parity,
-                                    baudrate=int(args.rtu_baud), reset_socket=True)
+                                    baudrate=int(args.rtu_baud), timeout=args.timeout, reset_socket=True)
     elif args.tcp:
         master = ModbusTcpClient(args.tcp, args.tcp_port, timeout=args.timeout, reset_socket=True)
     else:
         log.error("You must specify a modbus access method, either --rtu or --tcp")
         return False
     return True
 
@@ -383,16 +383,17 @@
             if not p.disabled:
                 p.poll()
                 if event_exit.is_set():
                     master.close()
                     return
                 event_exit.wait(timeout=args.interval)
     master.close()
-    # Always printout result
-    modbus_print()
+    # printout result, if -p or --print-result are set
+    if args.print_result:
+        modbus_print()
 
 
 def modbus_write_coil(device_name, address: int, value):
     if not master:
         return False
     master.connect()
     time.sleep(args.delay)
```

### Comparing `modpoll-0.5.3/modpoll/mqtt_task.py` & `modpoll-0.5.4/modpoll/mqtt_task.py`

 * *Files identical despite different names*

### Comparing `modpoll-0.5.3/pyproject.toml` & `modpoll-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modpoll"
-version = "0.5.3"
+version = "0.5.4"
 description = "A New Command Line Tool for Modbus"
 authors = ["Ying Shaodong <helloysd@foxmail.com>"]
 readme = "README.md"
 homepage = "https://helloysd.gitlab.io/modpoll"
 repository = "https://github.com/gavinying/modpoll"
 license = "MIT"
 include = [
```

### Comparing `modpoll-0.5.3/setup.py` & `modpoll-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0']}
 
 entry_points = \
 {'console_scripts': ['modpoll = modpoll:app']}
 
 setup_kwargs = {
     'name': 'modpoll',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'A New Command Line Tool for Modbus',
     'long_description': '# modpoll - A New Command Line Tool for Modbus\n\n[![pipeline status](https://gitlab.com/helloysd/modpoll/badges/master/pipeline.svg)](https://gitlab.com/helloysd/modpoll/-/commits/master)\n[![License](https://img.shields.io/pypi/l/modpoll)](https://gitlab.com/helloysd/modpoll/-/blob/master/LICENSE)\n[![Downloads](http://pepy.tech/badge/modpoll)](http://pepy.tech/project/modpoll)\n\n> Learn more about *modpoll* usage at [documentation](https://helloysd.gitlab.io/modpoll) site. \n\n\n\n## Motivation\n\nThe initial idea of creating this tool is to help myself debugging new devices during site survey. A site survey usually has limited time and space, working on-site also piles up some pressures. At that time, a portable swiss-knife toolkit is our best friend.\n\nThis program can be easily deployed to Raspberry Pi or similar embedded devices, polling data from modbus devices, users can choose to log data locally or publish to a MQTT broker for further debugging. \n\nThe MQTT broker can be setup on the same Raspberry Pi or on the cloud. Once data successfully published, users can subscribe to a specific MQTT topic to view the data via a smart phone at your fingertip. \n\n\n\n<p align="center">\n  <img src="docs/assets/modpoll-usage.png">\n</p>\n\n\n\nMoreover, you can also run this program continuously on a server as a Modbus-MQTT gateway, i.e. polling from local Modbus devices and forwarding data to a centralized cloud service. \n\nIn fact, *modpoll* helps to bridge between the traditional fieldbus world and the new IoT world. \n\n\n> This program is designed to be a standalone tool, it works out-of-the-box on Linux/macOS/Windows. \n\n> If you are looing for a modbus python library, please consider the following great open source projects, [pymodbus](https://github.com/riptideio/pymodbus) or [minimalmodbus](https://github.com/pyhys/minimalmodbus)\n\n\n\n## Feature\n\n- Support Modbus RTU/TCP/UDP devices\n- Show polling data for local debugging, like a typical modpoll tool\n- Publish polling data to MQTT broker for remote debugging, especially on smart phone\n- Export polling data to local storage for further investigation\n- Provide docker solution for continuous data polling use case\n\n\n\n## Installation\n\nThis program tested on python 3.8+, the package is available in the Python Package Index, users can easily install it using `pip` or `pipx`.\n\n### Using PIP\n\nPython3 is supported by most popular platforms, e.g. Linux/macOS/Windows, on which you can install *modpoll* using `pip` tool, \n\n```bash\npip install modpoll\n```\n\nUpgrade the tool via the following command,\n\n```bash\npip install -U modpoll\n```\n\n### On Windows\n\nIt is recommended to use `pipx` for installing *modpoll* on Windows, refer to [here](https://pypa.github.io/pipx/installation/) for more information about `pipx`. \n\nOnce `pipx` installed, you can run the following command in a Command Prompt termial. \n\n```PowerShell\npipx install modpoll\n```\n\nUpgrade the tool via the following command,\n\n```PowerShell\npipx upgrade modpoll\n```\n\n\n## Quickstart\n\nAs the name tells, *modpoll* is a tool for communicating with Modbus devices, so ideally it makes more sense if you have a real Modbus device on hand for the following test, but it is OK if you don\'t, we provide a virtual Modbus TCP device deployed at `modsim.topmaker.net:502` for your quick testing purpose. \n\nLet\'s start expoloring *modpoll* with *modsim* device, run the following command to get a first glimpse,\n\n```bash\nmodpoll --tcp modsim.topmaker.net --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv\n```\n\n<p align="center">\n  <img src="docs/assets/screenshot-modpoll.png">\n</p>\n\n\n> the modsim code is also available [here](https://github.com/gavinying/modsim)\n\n\n### Prepare Modbus configure file\n\nThe reason we can magically poll data from the online device *modsim* is because we have already provided the [Modbus configure file](https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv) for *modsim* device as following, \n\n```CSV\ndevice,modsim001,1,,\npoll,holding_register,40000,20,BE_BE\nref,value1,40000,uint16,rw\nref,value2,40001,uint16,rw\nref,value3,40002,uint16,rw\nref,value4,40003,uint16,rw\nref,value5,40004,int16,rw\nref,value6,40005,int16,rw\nref,value7,40006,int16,rw\nref,value8,40007,int16,rw\nref,value9,40008,uint32,rw\nref,value10,40010,uint32,rw\nref,value11,40012,int32,rw\nref,value12,40014,int32,rw\nref,value13,40016,float32,rw\nref,value14,40018,float32,rw\npoll,coil,0,24,BE_BE\nref,coil1-8,0,bool,rw\nref,coil9-16,8,bool,rw\n```\n\nThis configuration tells *modpoll* to do the following for each poll,\n\n- Read `20` holding registers (register address: `40000-40019`) and parse data accordingly; \n- Read `24` coils (coil address: `0-23`) and parse data accordingly; \n\n\nNormally, you need to customize a Modbus configuration file for your own device before running *modpoll* tool, which defines the optimal polling patterns and register mappings according to device vendor\'s documents. \n\nThe configuration can be either a local file or a remote public URL resource. \n\n> *Refer to the [documentation](https://helloysd.gitlab.io/modpoll/configure.html) site for more details.*\n\n### Poll local device (modsim)\n\nIf you are blocked by company firewall for online device or prefer a local test, you can launch your own device simulator by running *modsim* locally, \n\n```bash\ndocker run -p 5020:5020 helloysd/modsim\n```\n\nIt will create a virtual Modbus TCP device running at `localhost:5020`, and then you can poll it using *modpoll* tool, \n\n```bash\nmodpoll --tcp localhost --tcp-port 5020 --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv\n```\n\n> Use `sudo` before the docker command if you want to use the standard port `502`.\n\n```bash\nsudo docker run -p 502:5020 helloysd/modsim\nmodpoll --tcp localhost --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv\n```\n\n\n### Publish data to MQTT broker\n\nThis is a useful function of this new *modpoll* tool, which provides a simple way to publish collected modbus data to MQTT broker, so users can view data from a smart phone via a MQTT client. \n\nThe following example uses a public MQTT broker `mqtt.eclipseprojects.io` for test purpose. You can also setup your own MQTT broker locally using [mosquitto](https://mosquitto.org/download/).\n\n```bash\nmodpoll --tcp modsim.topmaker.net --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv --mqtt-host mqtt.eclipseprojects.io\n```\n\nWith successful data polling and publishing, you can subscribe the topic `modpoll/modsim` on the same MQTT broker `mqtt.eclipseprojects.io` to view the collected data. \n\n> The MQTT topic uses `<mqtt_topic_prefix>/<deviceid>` pattern, <mqtt_topic_prefix> is provided by `--mqtt-topic-prefix` argument, the default value is `modpoll/`  and <deviceid> is provided by the Modbus configure file. \n\n\n\n<p align="center">\n  <img src="docs/assets/screencast-modpoll-mqtt.gif">\n</p>\n\n\n\n### Write registers via MQTT publish\n\nThe *modpoll* tool will subscribe to the topic `<mqtt_topic_prefix>/<deviceid>/set` once it successfully connected to MQTT broker, user can write device register(s) via MQTT publish, \n\n- To write a single holding register (address at `40001`)\n\n  ```json\n  {\n    "object_type": "holding_register",\n    "address": 40001,\n    "value": 12\n  }\n  ```\n\n- To write multiple holding registers (address starting from `40001`)\n\n  ```json\n  {\n    "object_type": "holding_register",\n    "address": 40001,\n    "value": [12, 13, 14, 15]\n  }\n  ```\n\n\n\n## Run in docker\n\nA docker image has been provided for user to directly run the program without local installation, \n\n  ```bash\n  docker run helloysd/modpoll\n  ```\n\nIt shows the version of the program by default.\n\nSimilar to the above *modsim* test, we can poll the first 5 holding registers with `docker run`,\n\n  ```bash\n  docker run helloysd/modpoll modpoll --tcp modsim.topmaker.net --config https://raw.githubusercontent.com/gavinying/modpoll/master/examples/modsim.csv\n  ```\n\nIf you want to load a local configure file, you need to mount a local folder onto container volume, \nfor example, if the child folder `examples` contains the config file `modsim.csv`, we can use it via the following command, \n\n  ```bash\n  docker run -v $(pwd)/examples:/app/examples helloysd/modpoll modpoll --tcp modsim.topmaker.net --config /app/examples/modsim.csv\n  ```\n\n\n\n## Basic Usage\n\n- Connect to Modbus TCP device\n\n  ```bash\n  modpoll --tcp 192.168.1.10 --config examples/modsim.csv\n  ```\n\n- Connect to Modbus RTU device \n\n  ```bash\n  modpoll --rtu /dev/ttyUSB0 --rtu-baud 9600 --config contrib/eniwise/scpms6.csv\n  ```\n\n- Connect to Modbus TCP device and publish data to MQTT broker \n\n  ```bash\n  modpoll --tcp modsim.topmaker.net --tcp-port 5020 --config examples/modsim.csv --mqtt-host mqtt.eclipseprojects.io\n  ```\n\n- Connect to Modbus TCP device and export data to local csv file\n\n  ```bash\n  modpoll --tcp modsim.topmaker.net --tcp-port 5020 --config examples/modsim.csv --export data.csv\n  ```\n\n\n\n> *Refer to the [documentation](https://helloysd.gitlab.io/modpoll) site for more details about the configuration and examples.*\n\n\n\n## Credits\n\nThe implementation of this project is heavily inspired by the following two projects:\n- https://github.com/owagner/modbus2mqtt (MIT license)\n- https://github.com/mbs38/spicierModbus2mqtt (MIT license)\n\nThanks to Max Brueggemann and Oliver Wagner for their great work. \n\n\n\n## License\n\nMIT © [helloysd](helloysd@foxmail.com)\n',
     'author': 'Ying Shaodong',
     'author_email': 'helloysd@foxmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://helloysd.gitlab.io/modpoll',
```

### Comparing `modpoll-0.5.3/PKG-INFO` & `modpoll-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modpoll
-Version: 0.5.3
+Version: 0.5.4
 Summary: A New Command Line Tool for Modbus
 Home-page: https://helloysd.gitlab.io/modpoll
 License: MIT
 Author: Ying Shaodong
 Author-email: helloysd@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

