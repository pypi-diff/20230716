# Comparing `tmp/bb_apputils-0.3.8.tar.gz` & `tmp/bb_apputils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_apputils-0.3.8.tar", max compression
+gzip compressed data, was "bb_apputils-0.3.9.tar", max compression
```

## Comparing `bb_apputils-0.3.8.tar` & `bb_apputils-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12709 2023-03-25 12:54:21.563375 bb_apputils-0.3.8/README.md
--rw-r--r--   0        0        0       49 2023-02-23 07:57:08.944094 bb_apputils-0.3.8/bbargparser/__init__.py
--rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.8/bbargparser/argparser.py
--rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.8/bblogger/__init__.py
--rw-r--r--   0        0        0    19011 2023-03-25 12:52:54.363373 bb_apputils-0.3.8/bblogger/logger.py
--rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.8/bblogger/texttools.py
--rw-r--r--   0        0        0      423 2023-03-25 12:53:34.253374 bb_apputils-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    13069 1970-01-01 00:00:00.000000 bb_apputils-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    12765 2023-07-15 23:38:35.760533 bb_apputils-0.3.9/README.md
+-rw-r--r--   0        0        0       49 2023-07-15 23:38:43.147200 bb_apputils-0.3.9/bbargparser/__init__.py
+-rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.9/bbargparser/argparser.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.9/bblogger/__init__.py
+-rw-r--r--   0        0        0    19080 2023-07-15 23:37:30.143865 bb_apputils-0.3.9/bblogger/logger.py
+-rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.9/bblogger/texttools.py
+-rw-r--r--   0        0        0      423 2023-07-15 23:38:02.503866 bb_apputils-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    13125 1970-01-01 00:00:00.000000 bb_apputils-0.3.9/PKG-INFO
```

### Comparing `bb_apputils-0.3.8/README.md` & `bb_apputils-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,17 @@
 - 0.3.5
     - modified BBLogger and getLogger to hopefully maintain the right level across modules
     - added 'rootlogger' level option
 
 - 0.3.8
     - changed formatter to include filename instead of logger name
 
+- 0.3.9
+    - fixed logging error when not in terminal
+
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
 
 <p>Adapted from <a href="https://stackoverflow.com/a/56944256/3638629">original code</a> by user's at Stack Overflow</p>
```

### Comparing `bb_apputils-0.3.8/bbargparser/argparser.py` & `bb_apputils-0.3.9/bbargparser/argparser.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.8/bblogger/logger.py` & `bb_apputils-0.3.9/bblogger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,18 @@
                              "<span style=\"color: #fc0202;\"> %(name)s>%(module)s.%(funcName)s </span>",
                              "<b>[ %(lineno)d ]</b>", "<span style=\"color: #fc0202;\"> %(levelname)s: </span>",
                              "<code>%(message)s</code></p>" ])
 
     def format(self, record):
         log_fmt = self.FORMAT.get(record.levelno)
         if self.mode == 'basic':
-            width = os.get_terminal_size().columns
+            try:
+                width = os.get_terminal_size().columns
+            except:
+                width = 200
             msg = record.getMessage()
             if len(msg) + len(record.levelname) + 21 > width:
                 words, msg_lines, first = [], [], len(record.levelname) + 5
                 for i in msg.split():
                     if len(' '.join( words )) + first + len(i) + 1 > width:
                         first = 0
                         msg_lines.append( ' '.join( words ))
```

### Comparing `bb_apputils-0.3.8/bblogger/texttools.py` & `bb_apputils-0.3.9/bblogger/texttools.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.8/PKG-INFO` & `bb_apputils-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-apputils
-Version: 0.3.8
+Version: 0.3.9
 Summary: App utilities
 Author: Erik Beebe
 Author-email: beebeapps_debugging@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -335,14 +335,17 @@
 - 0.3.5
     - modified BBLogger and getLogger to hopefully maintain the right level across modules
     - added 'rootlogger' level option
 
 - 0.3.8
     - changed formatter to include filename instead of logger name
 
+- 0.3.9
+    - fixed logging error when not in terminal
+
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
 
 <p>Adapted from <a href="https://stackoverflow.com/a/56944256/3638629">original code</a> by user's at Stack Overflow</p>
```

