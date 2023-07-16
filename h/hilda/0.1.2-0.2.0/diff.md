# Comparing `tmp/hilda-0.1.2.tar.gz` & `tmp/hilda-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-0.1.2.tar", last modified: Mon Jul  3 14:30:55 2023, max compression
+gzip compressed data, was "hilda-0.2.0.tar", last modified: Sun Jul 16 15:28:25 2023, max compression
```

## Comparing `hilda-0.1.2.tar` & `hilda-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-07-03 14:30:55.881790 hilda-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18368 2023-07-03 14:30:43.000000 hilda-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.877790 hilda-0.1.2/hilda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (123)    40937 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/lldb_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/lsof.m
--rw-r--r--   0 runner    (1001) docker     (123)    11366 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/remotepairingd.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-03 14:30:43.000000 hilda-0.1.2/hilda/to_ns_from_json.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.877790 hilda-0.1.2/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18903 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 14:30:55.000000 hilda-0.1.2/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 14:30:55.885790 hilda-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:30:43.000000 hilda-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:55.881790 hilda-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/hilda_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 14:30:43.000000 hilda-0.1.2/tests/lldb_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-16 15:28:08.000000 hilda-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-16 15:28:25.774668 hilda-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-07-16 15:28:08.000000 hilda-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.770668 hilda-0.2.0/hilda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (123)   120119 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (123)    41527 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/lldb_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/boringssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.774668 hilda-0.2.0/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-16 15:28:08.000000 hilda-0.2.0/hilda/to_ns_from_json.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:28:25.770668 hilda-0.2.0/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20787 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 15:28:25.000000 hilda-0.2.0/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-16 15:28:08.000000 hilda-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 15:28:08.000000 hilda-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:28:25.774668 hilda-0.2.0/setup.cfg
```

### Comparing `hilda-0.1.2/PKG-INFO` & `hilda-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,48 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.1.2
+Version: 0.2.0
 Summary: LLDB wrapped and empowered by iPython's features
-Home-page: https://github.com/doronz88/hilda
-Author: DoronZ
-Project-URL: hilda, https://github.com/doronz88/hilda
-Classifier: Programming Language :: Python :: 3.7
+Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
+Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
+License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
+        
+        Permission is hereby granted, free of charge, to any person obtaining
+        a copy of this software and associated documentation files (the
+        "Software"), to deal in the Software without restriction, including
+        without limitation the rights to use, copy, modify, merge, publish,
+        distribute, sublicense, and/or sell copies of the Software, and to
+        permit persons to whom the Software is furnished to do so, subject to
+        the following conditions:
+        
+        The above copyright notice and this permission notice shall be
+        included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+        NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+        LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+        WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://github.com/doronz88/hilda
+Project-URL: Bug Reports, https://github.com/doronz88/hilda/issues
+Keywords: python,debugger,lldb,ipython,ios,debug
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
 - [Description](#description)
 - [Example](#example)
 - [Installation](#installation)
 - [How to use](#how-to-use)
     * [Starting a Hilda shell](#starting-a-hilda-shell)
         + [Bare mode](#bare-mode)
@@ -76,14 +103,24 @@
 
 *⚠️ Please note that Hilda is installed on top of XCode's python so LLDB will be able to use its features.*
 
 # How to use
 
 ## Starting a Hilda shell
 
+### Attach mode
+
+Use the attach sub-command in order to start an LLDB shell attached to given process.
+
+```shell
+hilda attach [-p pid] [-n process-name]
+```
+
+After attaching, simply execute `hilda` command to enter the hilda shell.
+
 ### Bare mode
 
 Use "Bare mode" to get a "bare-bones" lldb shell, whereas hilda plugin is already loaded and ready to start. This mode
 is useful when you need to have custom commands for attaching to the target process (for example when debugging OSX
 processes).
 
 To start this mode simply use:
@@ -113,33 +150,38 @@
 
 ### Remote mode
 
 This mode will auto-connect to the remote device and attach to your target process assuming you are trying to debug a
 remote jailbroken iOS device.
 
 Please note the following:
-* script assumes the connected device already **has a running ssh server**, which doesn't require a password (you can use
-`ssh-copy-id` to achieve this).
+
+* script assumes the connected device already **has a running ssh server**, which doesn't require a password (you can
+  use
+  `ssh-copy-id` to achieve this).
 
 From this point the flow diverges into 2 flows:
 
 ### The connected device is connected to the network via `internet sharing` with your computer
+
 Run the following command:
+
 ```shell
 hilda remote PROCESS_NAME SSH_PORT
 ``` 
 
 ### The connected device is connected via Wi-Fi
 
 For this to work, you will need to make sure of the following:
-  * Find your cellphone IP address (Settings -> Wi-Fi -> network info -> IP Address).
-  * Once you found it, run the following command:
-      ```shell
-      hilda remote PROCESS_NAME SSH_PORT --hostname <DEVICE_IP_ADDRESS>
-      ```
+
+* Find your cellphone IP address (Settings -> Wi-Fi -> network info -> IP Address).
+* Once you found it, run the following command:
+    ```shell
+    hilda remote PROCESS_NAME SSH_PORT --hostname <DEVICE_IP_ADDRESS>
+    ```
 
 ## Commands
 
 Commands are just global python functions you can access any time. It's really advised to first get a good overview over
 them before start using, so you take full advantage of everything Hilda has to offer.
 
 Given below is a list of them:
```

### Comparing `hilda-0.1.2/README.md` & `hilda-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,24 @@
 
 *⚠️ Please note that Hilda is installed on top of XCode's python so LLDB will be able to use its features.*
 
 # How to use
 
 ## Starting a Hilda shell
 
+### Attach mode
+
+Use the attach sub-command in order to start an LLDB shell attached to given process.
+
+```shell
+hilda attach [-p pid] [-n process-name]
+```
+
+After attaching, simply execute `hilda` command to enter the hilda shell.
+
 ### Bare mode
 
 Use "Bare mode" to get a "bare-bones" lldb shell, whereas hilda plugin is already loaded and ready to start. This mode
 is useful when you need to have custom commands for attaching to the target process (for example when debugging OSX
 processes).
 
 To start this mode simply use:
@@ -98,33 +108,38 @@
 
 ### Remote mode
 
 This mode will auto-connect to the remote device and attach to your target process assuming you are trying to debug a
 remote jailbroken iOS device.
 
 Please note the following:
-* script assumes the connected device already **has a running ssh server**, which doesn't require a password (you can use
-`ssh-copy-id` to achieve this).
+
+* script assumes the connected device already **has a running ssh server**, which doesn't require a password (you can
+  use
+  `ssh-copy-id` to achieve this).
 
 From this point the flow diverges into 2 flows:
 
 ### The connected device is connected to the network via `internet sharing` with your computer
+
 Run the following command:
+
 ```shell
 hilda remote PROCESS_NAME SSH_PORT
 ``` 
 
 ### The connected device is connected via Wi-Fi
 
 For this to work, you will need to make sure of the following:
-  * Find your cellphone IP address (Settings -> Wi-Fi -> network info -> IP Address).
-  * Once you found it, run the following command:
-      ```shell
-      hilda remote PROCESS_NAME SSH_PORT --hostname <DEVICE_IP_ADDRESS>
-      ```
+
+* Find your cellphone IP address (Settings -> Wi-Fi -> network info -> IP Address).
+* Once you found it, run the following command:
+    ```shell
+    hilda remote PROCESS_NAME SSH_PORT --hostname <DEVICE_IP_ADDRESS>
+    ```
 
 ## Commands
 
 Commands are just global python functions you can access any time. It's really advised to first get a good overview over
 them before start using, so you take full advantage of everything Hilda has to offer.
 
 Given below is a list of them:
```

### Comparing `hilda-0.1.2/hilda/command.py` & `hilda-0.2.0/hilda/command.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/exceptions.py` & `hilda-0.2.0/hilda/exceptions.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/from_ns_to_json.m` & `hilda-0.2.0/hilda/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/get_objectivec_class_description.m` & `hilda-0.2.0/hilda/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/get_objectivec_symbol_data.m` & `hilda-0.2.0/hilda/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/hilda_ascii_art.html` & `hilda-0.2.0/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/hilda_client.py` & `hilda-0.2.0/hilda/hilda_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,39 +8,42 @@
 import os
 import pickle
 import textwrap
 import time
 from collections import namedtuple
 from contextlib import contextmanager, suppress
 from datetime import datetime, timezone
-from functools import partial
+from functools import cached_property, partial
 from pathlib import Path
 from typing import Union
 
-import IPython
 import docstring_parser
 import hexdump
+import IPython
 import lldb
 from humanfriendly import prompts
 from humanfriendly.terminal.html import html_to_ansi
+from keystone import KS_ARCH_ARM64, KS_ARCH_X86, KS_MODE_64, KS_MODE_LITTLE_ENDIAN, Ks
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import XmlLexer
 from tqdm import tqdm
 from traitlets.config import Config
 
 from hilda import objective_c_class
-from hilda.command import command, CommandsMeta
-from hilda.exceptions import *
+from hilda.command import CommandsMeta, command
+from hilda.exceptions import AccessingMemoryError, AccessingRegisterError, AddingLldbSymbolError, \
+    BrokenLocalSymbolsJarError, ConvertingFromNSObjectError, ConvertingToNsObjectError, CreatingObjectiveCSymbolError, \
+    DisableJetsamMemoryChecksError, EvaluatingExpressionError, HildaException, SymbolAbsentError
+from hilda.launch_lldb import disable_logs  # noqa: F401
 from hilda.objective_c_symbol import ObjectiveCSymbol
 from hilda.registers import Registers
 from hilda.snippets.mach import CFRunLoopServiceMachPort_hooks
 from hilda.symbol import Symbol
 from hilda.symbols_jar import SymbolsJar
-from hilda.launch_lldb import disable_logs
 
 IsaMagic = namedtuple('IsaMagic', 'mask value')
 ISA_MAGICS = [
     # ARM64
     IsaMagic(mask=0x000003f000000001, value=0x000001a000000001),
     # X86_64
     IsaMagic(mask=0x001f800000000001, value=0x001d800000000001),
@@ -73,15 +76,15 @@
         self.debugger = debugger
         self.target = debugger.GetSelectedTarget()
         self.process = self.target.GetProcess()
         self.symbols = SymbolsJar.create(self)
         self.breakpoints = {}
         self.captured_objects = {}
         self.registers = Registers(self)
-
+        self.arch = self.target.GetTriple().split('-')[0]
         # should unwind the stack on errors. change this to False in order to debug self-made calls
         # within hilda
         self._evaluation_unwind_on_error = True
 
         # should ignore breakpoints while evaluation
         self._evaluation_ignore_breakpoints = True
 
@@ -235,14 +238,24 @@
 
         if not err.Success():
             raise AccessingMemoryError()
 
         return retval
 
     @command()
+    def poke_text(self, address: int, code: str) -> int:
+        """
+        Write instructions to address.
+        :param address:
+        :param code:
+        """
+        bytecode, count = self._ks.asm(code, as_bytes=True)
+        return self.poke(address, bytecode)
+
+    @command()
     def peek(self, address, size: int) -> bytes:
         """
         Read data at given address
         :param address:
         :param size:
         :return:
         """
@@ -254,36 +267,21 @@
 
         if not err.Success():
             raise AccessingMemoryError()
 
         return retval
 
     @command()
-    def peek_str(self, address, encoding=None):
+    def peek_str(self, address: Symbol) -> str:
         """
         Peek a buffer till null termination
         :param address:
-        :param encoding: character encoding. if None, bytes is returned
         :return:
         """
-        if hasattr(self.symbols, 'strlen'):
-            # always prefer using native strlen
-            buf = self.peek(address, self.symbols.strlen(address))
-        else:
-            buf = self.peek(address, 1)
-            while buf[-1] != 0:
-                buf += self.peek(address + len(buf), 1)
-
-            # remove null terminator
-            buf = buf[:-1]
-
-        if encoding is not None:
-            buf = str(buf, encoding)
-
-        return buf
+        return address.po('char *')[1:-1]  # strip the ""
 
     @command()
     def stop(self):
         """ Stop process. """
         self.debugger.SetAsync(False)
 
         is_running = self.process.GetState() == lldb.eStateRunning
@@ -318,23 +316,24 @@
         Useful in order to exit gracefully so process doesn't get killed
         while you exit
         """
         if not self.process.Detach().Success():
             self.log_critical('failed to detach')
 
     @command()
-    def disass(self, address, buf, should_print=True) -> lldb.SBInstructionList:
+    def disass(self, address, buf, flavor='intel', should_print=True) -> lldb.SBInstructionList:
         """
         Print disassembly from a given address
+        :param flavor:
         :param address:
         :param buf:
         :param should_print:
         :return:
         """
-        inst = self.target.GetInstructions(lldb.SBAddress(address, self.target), buf)
+        inst = self.target.GetInstructionsWithFlavor(lldb.SBAddress(address, self.target), flavor, buf)
         if should_print:
             print(inst)
         return inst
 
     @command()
     def file_symbol(self, address) -> Symbol:
         """
@@ -604,15 +603,15 @@
             bp.SetScriptCallbackFunction('lldb.hilda_client.bp_callback_router')
 
         self.log_info(f'Breakpoint #{bp.id} has been set')
         return bp
 
     def bp_callback_router(self, frame, bp_loc, *_):
         """
-        Route the breakpoint callback the the specific breakpoint callback.
+        Route the breakpoint callback the specific breakpoint callback.
         :param lldb.SBFrame frame: LLDB Frame object.
         :param lldb.SBBreakpointLocation bp_loc: LLDB Breakpoint location object.
         """
         bp_id = bp_loc.GetBreakpoint().GetID()
         self._bp_frame = frame
         try:
             self.breakpoints[bp_id].callback(self, frame, bp_loc, self.breakpoints[bp_id].options)
@@ -898,21 +897,21 @@
         If interval is supplied, then if the device is in running state, it will sleep for the interval
         given before and after execution.
         """
         is_running = self.process.GetState() == lldb.eStateRunning
 
         if is_running:
             self.stop()
-            time.sleep(1)
+            time.sleep(interval)
 
         try:
             yield
         finally:
             if is_running:
-                time.sleep(1)
+                time.sleep(interval)
                 self.cont()
 
     @contextmanager
     def safe_malloc(self, size):
         """
         Context-Manager for allocating a block of memory which is freed afterwards
         :param size:
@@ -1112,20 +1111,19 @@
             elif isinstance(arg, int) or isinstance(arg, Symbol):
                 arg = int(arg) & 0xffffffffffffffff
                 args_conv.append(f'0x{arg:x}')
             else:
                 raise NotImplementedError('cannot serialize argument')
         return args_conv
 
-    @staticmethod
-    def _generate_call_expression(address, params):
+    def _generate_call_expression(self, address, params):
         args_type = ','.join(['intptr_t'] * len(params))
         args_conv = ','.join(params)
 
-        if self.target.modules[0].triple.split('-')[0] == 'arm64e':
+        if self.arch == 'arm64e':
             address = f'ptrauth_sign_unauthenticated((void *){address}, ptrauth_key_asia, 0)'
 
         return f'((intptr_t(*)({args_type}))({address}))({args_conv})'
 
     def _globalize_commands(self):
         """ Make all command available in global scope. """
         reserved_names = list(globals().keys()) + dir(builtins)
@@ -1174,7 +1172,14 @@
             'cf': lambda val: val.cf_description,
             'po': lambda val: val.po(),
         }
         if fmt in formatters:
             return formatters[fmt](value)
         else:
             return f'{value:x} (unsupported format)'
+
+    @cached_property
+    def _ks(self) -> Ks:
+        platforms = {'arm64': Ks(KS_ARCH_ARM64, KS_MODE_LITTLE_ENDIAN),
+                     'arm64e': Ks(KS_ARCH_ARM64, KS_MODE_LITTLE_ENDIAN),
+                     'x86_64h': Ks(KS_ARCH_X86, KS_MODE_64)}
+        return platforms.get(self.arch)
```

### Comparing `hilda-0.1.2/hilda/launch_lldb.py` & `hilda-0.2.0/hilda/launch_lldb.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,10 +63,30 @@
     """ Just start an lldb shell """
     # connect local LLDB client
     commands = [f'command script import {os.path.join(Path(__file__).resolve().parent, "lldb_entrypoint.py")}']
     commands = '\n'.join(commands)
     execute(f'lldb --one-line "{commands}"')
 
 
+@cli.command('attach')
+@click.option('-n', '--name', help='process name to attach')
+@click.option('-p', '--pid', type=click.INT, help='pid to attach')
+def attach(name: str, pid: int):
+    """ Attach to given process and start an lldb shell """
+    # connect local LLDB client
+    commands = []
+    if name is not None:
+        commands.append(f'process attach -n {name}')
+    elif pid is not None:
+        commands.append(f'process attach -p {pid}')
+    else:
+        print('missing either process name or pid for attaching')
+        return
+
+    commands.append(f'command script import {os.path.join(Path(__file__).resolve().parent, "lldb_entrypoint.py")}')
+    commands = '\n'.join(commands)
+    execute(f'lldb --one-line "{commands}"')
+
+
 if __name__ == '__main__':
     disable_logs()
     cli()
```

### Comparing `hilda-0.1.2/hilda/lldb_entrypoint.py` & `hilda-0.2.0/hilda/lldb_entrypoint.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/lsof.m` & `hilda-0.2.0/hilda/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/objective_c_class.py` & `hilda-0.2.0/hilda/objective_c_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import time
 from collections import namedtuple
 from dataclasses import dataclass, field
 from functools import partial
 from pathlib import Path
 from uuid import uuid4
 
+from objc_types_decoder.decode import decode as decode_type
+from objc_types_decoder.decode import decode_with_tail
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import ObjectiveCLexer
-from objc_types_decoder.decode import decode as decode_type, decode_with_tail
 
-from hilda.symbols_jar import SymbolsJar
 from hilda.exceptions import GettingObjectiveCClassError
+from hilda.symbols_jar import SymbolsJar
 
 Ivar = namedtuple('Ivar', 'name type_ offset')
 Property = namedtuple('Property', 'name attributes')
 PropertyAttributes = namedtuple('PropertyAttributes', 'synthesize type_ list')
 
 
 def convert_encoded_property_attributes(encoded):
```

### Comparing `hilda-0.1.2/hilda/objective_c_symbol.py` & `hilda-0.2.0/hilda/objective_c_symbol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 import os
 from contextlib import suppress
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 
+from objc_types_decoder.decode import decode as decode_type
 from pygments import highlight
 from pygments.formatters import TerminalTrueColorFormatter
 from pygments.lexers import ObjectiveCLexer
-from objc_types_decoder.decode import decode as decode_type
 
 from hilda.exceptions import HildaException
-from hilda.objective_c_class import Class, convert_encoded_property_attributes, Method, Property
-from hilda.symbols_jar import SymbolsJar
+from hilda.objective_c_class import Class, Method, Property, convert_encoded_property_attributes
 from hilda.symbol import Symbol
+from hilda.symbols_jar import SymbolsJar
 
 
 class SettingIvarError(HildaException):
     """ Raise when trying to set an Ivar too early or when the Ivar doesn't exist. """
     pass
```

### Comparing `hilda-0.1.2/hilda/registers.py` & `hilda-0.2.0/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/snippets/dyld.py` & `hilda-0.2.0/hilda/snippets/dyld.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from cached_property import cached_property
-
 import lldb
+from cached_property import cached_property
 
 from hilda.snippets.macho.all_image_infos import AllImageInfos
 from hilda.snippets.syslog import open_syslog_socket
 
 
 def all_image_infos():
     return AllImageInfos()
```

### Comparing `hilda-0.1.2/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py` & `hilda-0.2.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,57 @@
 import lldb
-from keystone import Ks, KS_ARCH_ARM64, KS_MODE_LITTLE_ENDIAN
 
+from hilda.exceptions import SymbolAbsentError
 
-def disable_mach_msg_errors():
+
+def _CFRunLoopServiceMachPort_hook(hilda, *args):
+    """
+    :param hilda.hilda_client.HildaClient hilda:
+     """
+    hilda.jump(hilda.CFRunLoopServiceMachPort_while_ea)
+    hilda.cont()
+
+
+def _disable_internal_error_handling() -> None:
+    hilda = lldb.hilda_client
+    with hilda.stopped():
+        instructions = hilda.symbols.__CFRunLoopServiceMachPort.disass(2000, should_print=False)
+        while_ea = None
+        for instruction in instructions:
+            if (while_ea is None) and instruction.DoesBranch():
+                # Beginning of the `while(true) { ... }`
+                while_ea = instruction.GetOperands(hilda.target)
+                hilda.CFRunLoopServiceMachPort_while_ea = int(hilda.file_symbol(eval(while_ea)))
+            elif instruction.GetMnemonic(hilda.target) in ('brk', 'ud2'):
+                symbol = hilda.symbol(instruction.addr.GetLoadAddress(hilda.target))
+                symbol.bp(
+                    _CFRunLoopServiceMachPort_hook,
+                    forced=True,
+                    name=f'__CFRunLoopServiceMachPort-brk-{int(symbol - hilda.symbols.__CFRunLoopServiceMachPort)}'
+                )
+
+    if hilda.arch == 'x86_64h':
+        return
+
+    # on iOS 16.x, will need to also patch this one
+    try:
+        handle_error = hilda.symbols['__CFRunLoopServiceMachPort.cold.1']
+    except SymbolAbsentError:
+        return
+
+    for instruction in handle_error.disass(2000, should_print=False):
+        if instruction.GetMnemonic(hilda.target) in ('brk', 'ud2'):
+            # mov x0, x0
+            hilda.symbol(instruction.addr.GetLoadAddress(hilda.target)).poke(b'\xe0\x03\x00\xaa')
+
+
+def _disable_mach_msg_timeout() -> None:
     """
-    Disable mach_msg syscall timeout CFRunLoopServiceMachPort. `__CFRunLoopServiceMachPort` receives
-    `mach_msg_timeout_t` parameter, the parameter passes on `x3` register. We set timeout = MACH_MSG_TIMEOUT_NONE.
+    Remove the timeout validation from __CFRunLoopServiceMachPort. This is done by patching the mach_msg_timeout_t
+    parameter (4rd one) to MACH_MSG_TIMEOUT_NONE. On arm the parameter passes on `x3` register.
 
         __int64 __fastcall __CFRunLoopServiceMachPort(
             mach_port_name_t a1,
             mach_msg_header_t **a2,
             mach_port_t *a3,
             mach_msg_timeout_t a4,
             voucher_mach_msg_state_t *a5,
@@ -25,19 +67,26 @@
         CoreFoundation:__text:0000000186E50144                 STP             X29, X30, [SP,#0x60+var_s0]
         CoreFoundation:__text:0000000186E50148                 ADD             X29, SP, #0x60
         CoreFoundation:__text:0000000186E5014C                 MOV             X21, X5
         CoreFoundation:__text:0000000186E50150                 MOV             X22, X4
         CoreFoundation:__text:0000000186E50154                 MOV             X23, X3       <-------- Timeout parameter
     """
     hilda = lldb.hilda_client
-    ks = Ks(KS_ARCH_ARM64, KS_MODE_LITTLE_ENDIAN)
+    if hilda.arch == 'x86_64h':
+        return
+
     with hilda.stopped():
         for inst in hilda.symbols.__CFRunLoopServiceMachPort.disass(200, should_print=False):
             mnemonic = inst.GetMnemonic(hilda.target)
-            operands = inst.GetOperands(hilda.target).replace(' ', '')
-            if mnemonic != 'mov' or ',x3' not in operands:
+            operands = inst.GetOperands(hilda.target)
+            if mnemonic != 'mov' or not operands.endswith('x3'):
                 continue
             addr = inst.GetAddress()
             file_addr = addr.GetFileAddress()
-            encoding, _ = ks.asm(f'{mnemonic} {operands.replace("x3", "0")}')
-            hilda.file_symbol(file_addr).poke(bytearray(encoding))
+            new_inst = f'{mnemonic} {operands.replace("x3", "0")}'
+            hilda.file_symbol(file_addr).poke_text(new_inst)
             break
+
+
+def disable_mach_msg_errors() -> None:
+    _disable_mach_msg_timeout()
+    _disable_internal_error_handling()
```

### Comparing `hilda-0.1.2/hilda/snippets/macho/all_image_infos.py` & `hilda-0.2.0/hilda/snippets/macho/all_image_infos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import lldb
-from construct import Struct, Tell, Int32ul, Pointer, this, Array, Int32ub, CString, If, Int64ul, Hex
+from construct import Array, CString, Hex, If, Int32ub, Int32ul, Int64ul, Pointer, Struct, Tell, this
 from humanfriendly import prompts
 
-from hilda.snippets.macho.image_info import dyld_image_info_t, ImageInfo
+from hilda.snippets.macho.image_info import ImageInfo, dyld_image_info_t
 from hilda.snippets.macho.macho import mach_header_t
 from hilda.snippets.uuid import uuid_t
 from hilda.symbol import SymbolFormatField
 
 all_image_infos_t = Struct(
     'address' / Tell,
     'version' / Int32ul,
```

### Comparing `hilda-0.1.2/hilda/snippets/macho/image_info.py` & `hilda-0.2.0/hilda/snippets/macho/image_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import lldb
-from construct import Pointer, this, CString, Int64ul, Struct, If
+from construct import CString, If, Int64ul, Pointer, Struct, this
 
 from hilda.snippets.macho.macho import mach_header_t
 from hilda.snippets.macho.macho_load_commands import LoadCommands
 from hilda.snippets.uuid import uuid_t
 from hilda.symbol import SymbolFormatField
 
 dyld_image_info_t = Struct(
```

### Comparing `hilda-0.1.2/hilda/snippets/macho/macho.py` & `hilda-0.2.0/hilda/snippets/macho/macho.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from construct import Int32ul, Struct, Hex, this, Tell, LazyArray, Computed
+from construct import Computed, Hex, Int32ul, LazyArray, Struct, Tell, this
+
 from hilda.snippets.macho.macho_load_commands import LOAD_COMMAND_TYPE, load_command_t
 
 
 def __calculate_aslr(ctx):
     loaded_address = ctx.load_address
     for load_command in ctx.load_commands:
         if load_command.cmd == LOAD_COMMAND_TYPE.LC_SEGMENT_64 and load_command.data.segname == '__TEXT':
```

### Comparing `hilda-0.1.2/hilda/snippets/macho/macho_load_commands.py` & `hilda-0.2.0/hilda/snippets/macho/macho_load_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import lldb
-
-from construct import Hex, Int32ul, Pointer, PaddedString, Int64ul, this, Enum, Struct, Tell, Switch, Bytes, Seek, \
-    Array, Int8ul
+from construct import Array, Bytes, Enum, Hex, Int8ul, Int32ul, Int64ul, PaddedString, Pointer, Seek, Struct, Switch, \
+    Tell, this
 
 from hilda.snippets.macho.apple_version import version_t
 from hilda.symbol import SymbolFormatField
 
 # See: https://opensource.apple.com/source/xnu/xnu-7195.81.3/EXTERNAL_HEADERS/mach-o/loader.h
 LC_REQ_DYLD = 0x80000000
```

### Comparing `hilda-0.1.2/hilda/snippets/remotepairingd.py` & `hilda-0.2.0/hilda/snippets/remotepairingd.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,15 @@
     0x1b: 'SETUP_CODE_TYPE',
     0x1c: 'PRODUCTION_DATA',
     0x1d: 'APP_INFO',
     0xff: 'SEPARATOR'
 }
 
 
-def TLV8CopyCoalesced_bp(hilda, *args):
-    src = hilda.registers.x0
-    end = hilda.registers.x1
+def _TLV8CopyCoalesced_bp(hilda, *args):
     type_ = hilda.registers.x2
     out_len = hilda.registers.x3
     out_len.item_size = 4
     hilda.finish()
 
     if hilda.registers.x0 == 0:
         print(f'TLV8CopyCoalesced\n'
@@ -52,29 +50,27 @@
         print(f'TLV8CopyCoalesced\n'
               f'    type_: {TLV_MAP[type_]}\n'
               f'    buffer: {hilda.registers.x0.peek(out_len[0])}\n'
               f'---\n')
     hilda.cont()
 
 
-def TLV8BufferAppend_bp(hilda, *args):
+def _TLV8BufferAppend_bp(hilda, *args):
     buffer = hilda.registers.x0
     type_ = hilda.registers.x1
     buffer = hilda.registers.x2
     buffer_len = hilda.registers.x3
     print(f'TLV8BufferAppend\n'
           f'    type_: {TLV_MAP[type_]}\n'
           f'    buffer: {buffer.peek(buffer_len)}\n'
           f'---\n')
     hilda.cont()
 
 
-def SRPClientStart_libsrp_bp(hilda, *args):
-    client = hilda.registers.x0
-    params = hilda.registers.x1
+def _SRPClientStart_libsrp_bp(hilda, *args):
     username = hilda.registers.x2
     username_len = hilda.registers.x3
     password = hilda.registers.x4
     password_len = hilda.registers.x5
     salt = hilda.registers.x6
     salt_len = hilda.registers.x7
     server_public_key = hilda.registers.sp[0]
@@ -87,16 +83,15 @@
           f'    salt: {salt.peek(salt_len)}\n'
           f'    server_public_key: {server_public_key.peek(server_public_key_len)}\n'
           f'    client_public_key: {client_public_key.peek(client_public_key_len)}\n'
           f'---\n')
     hilda.cont()
 
 
-def cced25519_sign_bp(hilda, *args):
-    digest_info = hilda.registers.x0
+def _cced25519_sign_bp(hilda, *args):
     sig = hilda.registers.x1
     len = hilda.registers.x2
     msg = hilda.registers.x3
     msg = msg.peek(len)
     public_key = hilda.registers.x4.peek(32)
     private_key = hilda.registers.x5.peek(32)
     hilda.finish()
@@ -105,31 +100,30 @@
           f'    private_key: {private_key}\n'
           f'    msg: {msg}\n'
           f'    sig: {sig.peek(64)}\n'
           f'---\n')
     hilda.cont()
 
 
-def cced25519_verify_bp(hilda, *args):
-    digest_info = hilda.registers.x0
+def _cced25519_verify_bp(hilda, *args):
     sig = hilda.registers.x3
     len = hilda.registers.x1
     msg = hilda.registers.x2
     msg = msg.peek(len)
     public_key = hilda.registers.x4.peek(32)
     hilda.finish()
     print(f'cced25519_verify\n'
           f'    public_key: {public_key}\n'
           f'    msg: {msg}\n'
           f'    sig: {sig.peek(64)}\n'
           f'---\n')
     hilda.cont()
 
 
-def CryptoHKDF_bp(hilda, *args):
+def _CryptoHKDF_bp(hilda, *args):
     descriptor = hilda.registers.x0
     key = hilda.registers.x1.peek(hilda.registers.x2)
     salt = hilda.registers.x3
     salt_len = hilda.registers.x4
     info = hilda.registers.x5
     info_len = hilda.registers.x6
     out_key = hilda.registers.sp[0]
@@ -173,18 +167,18 @@
           f'---\n')
     hilda.cont()
 
 
 def monitor_crypto_functions() -> None:
     hilda_client = lldb.hilda_client
 
-    hilda_client.symbols.TLV8CopyCoalesced.bp(TLV8CopyCoalesced_bp)
-    hilda_client.symbols.TLV8BufferAppend.bp(TLV8BufferAppend_bp)
-    hilda_client.symbols.SRPClientStart_libsrp.bp(SRPClientStart_libsrp_bp)
+    hilda_client.symbols.TLV8CopyCoalesced.bp(_TLV8CopyCoalesced_bp)
+    hilda_client.symbols.TLV8BufferAppend.bp(_TLV8BufferAppend_bp)
+    hilda_client.symbols.SRPClientStart_libsrp.bp(_SRPClientStart_libsrp_bp)
     hilda_client.symbols.SRPClientVerify_libsrp.monitor()
     hilda_client.symbols.SRPServerStart_libsrp.monitor()
     hilda_client.symbols.SRPServerVerify_libsrp.monitor()
-    hilda_client.symbols.cced25519_sign.bp(cced25519_sign_bp)
-    hilda_client.symbols.cced25519_verify.bp(cced25519_verify_bp)
-    hilda_client.symbols.CryptoHKDF.bp(CryptoHKDF_bp)
+    hilda_client.symbols.cced25519_sign.bp(_cced25519_sign_bp)
+    hilda_client.symbols.cced25519_verify.bp(_cced25519_verify_bp)
+    hilda_client.symbols.CryptoHKDF.bp(_CryptoHKDF_bp)
     hilda_client.symbols._chacha20_poly1305_encrypt_all.bp(_chacha20_poly1305_encrypt_all_bp)
     hilda_client.symbols._chacha20_poly1305_decrypt_all.bp(_chacha20_poly1305_decrypt_all_bp)
```

### Comparing `hilda-0.1.2/hilda/snippets/xpc.py` & `hilda-0.2.0/hilda/snippets/xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda/symbol.py` & `hilda-0.2.0/hilda/symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from construct import FormatField
-from contextlib import contextmanager
-import struct
 import os
+import struct
+from contextlib import contextmanager
+
+from construct import FormatField
 
 from hilda.objective_c_class import Class
 
 ADDRESS_SIZE_TO_STRUCT_FORMAT = {1: 'B', 2: 'H', 4: 'I', 8: 'Q'}
 
 
 class SymbolFormatField(FormatField):
@@ -115,16 +116,19 @@
 
     def peek(self, count):
         return self._client.peek(self, count)
 
     def poke(self, buf):
         return self._client.poke(self, buf)
 
-    def peek_str(self, encoding=None):
-        return self._client.peek_str(self, encoding)
+    def poke_text(self, code: str) -> int:
+        return self._client.poke_text(self, code)
+
+    def peek_str(self):
+        return self._client.peek_str(self)
 
     def monitor(self, **args):
         return self._client.monitor(self, **args)
 
     def bp(self, callback=None, **args):
         return self._client.bp(self, callback, **args)
```

### Comparing `hilda-0.1.2/hilda/symbols_jar.py` & `hilda-0.2.0/hilda/symbols_jar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from contextlib import suppress
 
 import lldb
 
-from hilda.exceptions import SymbolAbsentError, AddingLldbSymbolError
+from hilda.exceptions import AddingLldbSymbolError, SymbolAbsentError
 
 
 class SymbolsJar(dict):
     @staticmethod
     def create(client):
         """
         Factory method for creating symbols jars
```

### Comparing `hilda-0.1.2/hilda/to_ns_from_json.m` & `hilda-0.2.0/hilda/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-0.1.2/hilda.egg-info/PKG-INFO` & `hilda-0.2.0/hilda.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,48 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 0.1.2
+Version: 0.2.0
 Summary: LLDB wrapped and empowered by iPython's features
-Home-page: https://github.com/doronz88/hilda
-Author: DoronZ
-Project-URL: hilda, https://github.com/doronz88/hilda
-Classifier: Programming Language :: Python :: 3.7
+Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
+Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
+License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
+        
+        Permission is hereby granted, free of charge, to any person obtaining
+        a copy of this software and associated documentation files (the
+        "Software"), to deal in the Software without restriction, including
+        without limitation the rights to use, copy, modify, merge, publish,
+        distribute, sublicense, and/or sell copies of the Software, and to
+        permit persons to whom the Software is furnished to do so, subject to
+        the following conditions:
+        
+        The above copyright notice and this permission notice shall be
+        included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+        NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+        LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+        WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Project-URL: Homepage, https://github.com/doronz88/hilda
+Project-URL: Bug Reports, https://github.com/doronz88/hilda/issues
+Keywords: python,debugger,lldb,ipython,ios,debug
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
 - [Description](#description)
 - [Example](#example)
 - [Installation](#installation)
 - [How to use](#how-to-use)
     * [Starting a Hilda shell](#starting-a-hilda-shell)
         + [Bare mode](#bare-mode)
@@ -76,14 +103,24 @@
 
 *⚠️ Please note that Hilda is installed on top of XCode's python so LLDB will be able to use its features.*
 
 # How to use
 
 ## Starting a Hilda shell
 
+### Attach mode
+
+Use the attach sub-command in order to start an LLDB shell attached to given process.
+
+```shell
+hilda attach [-p pid] [-n process-name]
+```
+
+After attaching, simply execute `hilda` command to enter the hilda shell.
+
 ### Bare mode
 
 Use "Bare mode" to get a "bare-bones" lldb shell, whereas hilda plugin is already loaded and ready to start. This mode
 is useful when you need to have custom commands for attaching to the target process (for example when debugging OSX
 processes).
 
 To start this mode simply use:
@@ -113,33 +150,38 @@
 
 ### Remote mode
 
 This mode will auto-connect to the remote device and attach to your target process assuming you are trying to debug a
 remote jailbroken iOS device.
 
 Please note the following:
-* script assumes the connected device already **has a running ssh server**, which doesn't require a password (you can use
-`ssh-copy-id` to achieve this).
+
+* script assumes the connected device already **has a running ssh server**, which doesn't require a password (you can
+  use
+  `ssh-copy-id` to achieve this).
 
 From this point the flow diverges into 2 flows:
 
 ### The connected device is connected to the network via `internet sharing` with your computer
+
 Run the following command:
+
 ```shell
 hilda remote PROCESS_NAME SSH_PORT
 ``` 
 
 ### The connected device is connected via Wi-Fi
 
 For this to work, you will need to make sure of the following:
-  * Find your cellphone IP address (Settings -> Wi-Fi -> network info -> IP Address).
-  * Once you found it, run the following command:
-      ```shell
-      hilda remote PROCESS_NAME SSH_PORT --hostname <DEVICE_IP_ADDRESS>
-      ```
+
+* Find your cellphone IP address (Settings -> Wi-Fi -> network info -> IP Address).
+* Once you found it, run the following command:
+    ```shell
+    hilda remote PROCESS_NAME SSH_PORT --hostname <DEVICE_IP_ADDRESS>
+    ```
 
 ## Commands
 
 Commands are just global python functions you can access any time. It's really advised to first get a good overview over
 them before start using, so you take full advantage of everything Hilda has to offer.
 
 Given below is a list of them:
```

### Comparing `hilda-0.1.2/hilda.egg-info/SOURCES.txt` & `hilda-0.2.0/hilda.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+LICENSE
 README.md
-setup.cfg
-setup.py
+pyproject.toml
+requirements.txt
 hilda/__init__.py
 hilda/__main__.py
 hilda/command.py
 hilda/exceptions.py
 hilda/from_ns_to_json.m
 hilda/get_objectivec_class_description.m
 hilda/get_objectivec_symbol_data.m
@@ -22,27 +23,23 @@
 hilda.egg-info/PKG-INFO
 hilda.egg-info/SOURCES.txt
 hilda.egg-info/dependency_links.txt
 hilda.egg-info/entry_points.txt
 hilda.egg-info/requires.txt
 hilda.egg-info/top_level.txt
 hilda/snippets/__init__.py
+hilda/snippets/boringssl.py
 hilda/snippets/collections.py
 hilda/snippets/dyld.py
 hilda/snippets/fs_utils.py
 hilda/snippets/remotepairingd.py
 hilda/snippets/syslog.py
 hilda/snippets/uuid.py
 hilda/snippets/xpc.py
 hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
 hilda/snippets/mach/__init__.py
 hilda/snippets/macho/__init__.py
 hilda/snippets/macho/all_image_infos.py
 hilda/snippets/macho/apple_version.py
 hilda/snippets/macho/image_info.py
 hilda/snippets/macho/macho.py
-hilda/snippets/macho/macho_load_commands.py
-tests/__init__.py
-tests/__main__.py
-tests/conftest.py
-tests/hilda_tests.py
-tests/lldb_entrypoint.py
+hilda/snippets/macho/macho_load_commands.py
```

