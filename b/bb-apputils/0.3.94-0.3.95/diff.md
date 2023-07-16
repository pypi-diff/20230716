# Comparing `tmp/bb_apputils-0.3.94.tar.gz` & `tmp/bb_apputils-0.3.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_apputils-0.3.94.tar", max compression
+gzip compressed data, was "bb_apputils-0.3.95.tar", max compression
```

## Comparing `bb_apputils-0.3.94.tar` & `bb_apputils-0.3.95.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12923 2023-07-16 06:44:06.337682 bb_apputils-0.3.94/README.md
--rw-r--r--   0        0        0       50 2023-07-16 06:44:10.984349 bb_apputils-0.3.94/bbargparser/__init__.py
--rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.94/bbargparser/argparser.py
--rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.94/bblogger/__init__.py
--rw-r--r--   0        0        0    19540 2023-07-16 06:44:55.951017 bb_apputils-0.3.94/bblogger/logger.py
--rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.94/bblogger/texttools.py
--rw-r--r--   0        0        0      424 2023-07-16 06:44:14.237683 bb_apputils-0.3.94/pyproject.toml
--rw-r--r--   0        0        0    13284 1970-01-01 00:00:00.000000 bb_apputils-0.3.94/PKG-INFO
+-rw-r--r--   0        0        0    12923 2023-07-16 06:50:44.394357 bb_apputils-0.3.95/README.md
+-rw-r--r--   0        0        0       50 2023-07-16 06:50:31.087690 bb_apputils-0.3.95/bbargparser/__init__.py
+-rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.95/bbargparser/argparser.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.95/bblogger/__init__.py
+-rw-r--r--   0        0        0    19517 2023-07-16 06:50:25.614356 bb_apputils-0.3.95/bblogger/logger.py
+-rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.95/bblogger/texttools.py
+-rw-r--r--   0        0        0      424 2023-07-16 06:50:39.134356 bb_apputils-0.3.95/pyproject.toml
+-rw-r--r--   0        0        0    13284 1970-01-01 00:00:00.000000 bb_apputils-0.3.95/PKG-INFO
```

### Comparing `bb_apputils-0.3.94/README.md` & `bb_apputils-0.3.95/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
 - 0.3.91
     - fixed typo in basic logging.... maybe
 
 - 0.3.92
     - 2nd attempt at fixing basic logging
 
-- 0.3.94
+- 0.3.95
     - rewrote the basic logging formatter
 
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
```

### Comparing `bb_apputils-0.3.94/bbargparser/argparser.py` & `bb_apputils-0.3.95/bbargparser/argparser.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.94/bblogger/logger.py` & `bb_apputils-0.3.95/bblogger/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         if self.mode == 'basic':
             try:
                 width = os.get_terminal_size().columns
             except:
                 width = 200
             msg = record.getMessage()
             if len(msg) + len(record.levelname) + 21 > width:
-                length = len(record.levelname) + 5
+                length = 13
                 words, msg_lines, indent = msg.split(), [''], f"{'    ':.<{length - 4}}"
                 while words:
                     if len(words[0]) + length + 2 > width:
                         if len(msg_lines[-1]) < int(width*.7):
                             left = width - len(msg_lines[-1]) - 2
                             split_word = words.pop(0)
                             word = split_word[:left]
```

### Comparing `bb_apputils-0.3.94/bblogger/texttools.py` & `bb_apputils-0.3.95/bblogger/texttools.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.94/PKG-INFO` & `bb_apputils-0.3.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-apputils
-Version: 0.3.94
+Version: 0.3.95
 Summary: App utilities
 Author: Erik Beebe
 Author-email: beebeapps_debugging@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -344,15 +344,15 @@
 
 - 0.3.91
     - fixed typo in basic logging.... maybe
 
 - 0.3.92
     - 2nd attempt at fixing basic logging
 
-- 0.3.94
+- 0.3.95
     - rewrote the basic logging formatter
 
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
```

