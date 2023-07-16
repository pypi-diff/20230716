# Comparing `tmp/bb_apputils-0.3.9.tar.gz` & `tmp/bb_apputils-0.3.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_apputils-0.3.9.tar", max compression
+gzip compressed data, was "bb_apputils-0.3.91.tar", max compression
```

## Comparing `bb_apputils-0.3.9.tar` & `bb_apputils-0.3.91.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12765 2023-07-15 23:38:35.760533 bb_apputils-0.3.9/README.md
--rw-r--r--   0        0        0       49 2023-07-15 23:38:43.147200 bb_apputils-0.3.9/bbargparser/__init__.py
--rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.9/bbargparser/argparser.py
--rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.9/bblogger/__init__.py
--rw-r--r--   0        0        0    19080 2023-07-15 23:37:30.143865 bb_apputils-0.3.9/bblogger/logger.py
--rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.9/bblogger/texttools.py
--rw-r--r--   0        0        0      423 2023-07-15 23:38:02.503866 bb_apputils-0.3.9/pyproject.toml
--rw-r--r--   0        0        0    13125 1970-01-01 00:00:00.000000 bb_apputils-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    12819 2023-07-16 05:55:34.037628 bb_apputils-0.3.91/README.md
+-rw-r--r--   0        0        0       50 2023-07-16 05:55:44.624294 bb_apputils-0.3.91/bbargparser/__init__.py
+-rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.91/bbargparser/argparser.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.91/bblogger/__init__.py
+-rw-r--r--   0        0        0    19084 2023-07-16 05:54:02.824292 bb_apputils-0.3.91/bblogger/logger.py
+-rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.91/bblogger/texttools.py
+-rw-r--r--   0        0        0      424 2023-07-16 05:55:45.620961 bb_apputils-0.3.91/pyproject.toml
+-rw-r--r--   0        0        0    13180 1970-01-01 00:00:00.000000 bb_apputils-0.3.91/PKG-INFO
```

### Comparing `bb_apputils-0.3.9/README.md` & `bb_apputils-0.3.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -326,14 +326,17 @@
 
 - 0.3.8
     - changed formatter to include filename instead of logger name
 
 - 0.3.9
     - fixed logging error when not in terminal
 
+- 0.3.91
+    - fixed typo in basic logging.... maybe
+
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
 
 <p>Adapted from <a href="https://stackoverflow.com/a/56944256/3638629">original code</a> by user's at Stack Overflow</p>
```

### Comparing `bb_apputils-0.3.9/bbargparser/argparser.py` & `bb_apputils-0.3.91/bbargparser/argparser.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.9/bblogger/logger.py` & `bb_apputils-0.3.91/bblogger/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                     words += [i]
 
                 if words:
                     msg_lines.append( ' '.join(words) )
 
                 space = width - 11 - len(record.levelname) - ( len(msg_lines[-1]) - ( int(len(msg_lines[-1]) / width) * width ))
                 if space < 0:
-                    msg_lines[-1] += f"{' ':.<{-i - 1}}"
+                    msg_lines[-1] += f"{' ':.<{-space - 1}}"
                     msg_lines += [ "          " ]
                     space = width - 16
 
                 record.msg = '\n'.join(msg_lines)
 
             else:
                 space = width - 21 - len(record.levelname) - ( len(msg) - ( int(len(msg) / width) * width ))
```

### Comparing `bb_apputils-0.3.9/bblogger/texttools.py` & `bb_apputils-0.3.91/bblogger/texttools.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.9/PKG-INFO` & `bb_apputils-0.3.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-apputils
-Version: 0.3.9
+Version: 0.3.91
 Summary: App utilities
 Author: Erik Beebe
 Author-email: beebeapps_debugging@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -338,14 +338,17 @@
 
 - 0.3.8
     - changed formatter to include filename instead of logger name
 
 - 0.3.9
     - fixed logging error when not in terminal
 
+- 0.3.91
+    - fixed typo in basic logging.... maybe
+
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
 
 <p>Adapted from <a href="https://stackoverflow.com/a/56944256/3638629">original code</a> by user's at Stack Overflow</p>
```

