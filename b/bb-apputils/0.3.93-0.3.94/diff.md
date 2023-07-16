# Comparing `tmp/bb_apputils-0.3.93.tar.gz` & `tmp/bb_apputils-0.3.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_apputils-0.3.93.tar", max compression
+gzip compressed data, was "bb_apputils-0.3.94.tar", max compression
```

## Comparing `bb_apputils-0.3.93.tar` & `bb_apputils-0.3.94.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12923 2023-07-16 06:42:12.954347 bb_apputils-0.3.93/README.md
--rw-r--r--   0        0        0       50 2023-07-16 06:41:40.541013 bb_apputils-0.3.93/bbargparser/__init__.py
--rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.93/bbargparser/argparser.py
--rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.93/bblogger/__init__.py
--rw-r--r--   0        0        0    19538 2023-07-16 06:41:17.644346 bb_apputils-0.3.93/bblogger/logger.py
--rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.93/bblogger/texttools.py
--rw-r--r--   0        0        0      424 2023-07-16 06:41:34.894346 bb_apputils-0.3.93/pyproject.toml
--rw-r--r--   0        0        0    13284 1970-01-01 00:00:00.000000 bb_apputils-0.3.93/PKG-INFO
+-rw-r--r--   0        0        0    12923 2023-07-16 06:44:06.337682 bb_apputils-0.3.94/README.md
+-rw-r--r--   0        0        0       50 2023-07-16 06:44:10.984349 bb_apputils-0.3.94/bbargparser/__init__.py
+-rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.94/bbargparser/argparser.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.94/bblogger/__init__.py
+-rw-r--r--   0        0        0    19540 2023-07-16 06:44:55.951017 bb_apputils-0.3.94/bblogger/logger.py
+-rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.94/bblogger/texttools.py
+-rw-r--r--   0        0        0      424 2023-07-16 06:44:14.237683 bb_apputils-0.3.94/pyproject.toml
+-rw-r--r--   0        0        0    13284 1970-01-01 00:00:00.000000 bb_apputils-0.3.94/PKG-INFO
```

### Comparing `bb_apputils-0.3.93/README.md` & `bb_apputils-0.3.94/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 
 - 0.3.91
     - fixed typo in basic logging.... maybe
 
 - 0.3.92
     - 2nd attempt at fixing basic logging
 
-- 0.3.93
+- 0.3.94
     - rewrote the basic logging formatter
 
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
```

### Comparing `bb_apputils-0.3.93/bbargparser/argparser.py` & `bb_apputils-0.3.94/bbargparser/argparser.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.93/bblogger/logger.py` & `bb_apputils-0.3.94/bblogger/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                             left = width - len(msg_lines[-1]) - 2
                             split_word = words.pop(0)
                             word = split_word[:left]
                             msg_lines[-1] += f" {word}"
                             msg_lines.append( f"{indent}" )
                             words.insert( 0, split_word[left:] )
                         else:
-                            msg_lines.append( f"{indent}"
+                            msg_lines.append( f"{indent}" )
 
                         length = len(msg_lines[-1])
 
                     else:
                         word = f" {words.pop(0)}"
                         length += len(word)
                         msg_lines[-1] += word
```

### Comparing `bb_apputils-0.3.93/bblogger/texttools.py` & `bb_apputils-0.3.94/bblogger/texttools.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.93/PKG-INFO` & `bb_apputils-0.3.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-apputils
-Version: 0.3.93
+Version: 0.3.94
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
 
-- 0.3.93
+- 0.3.94
     - rewrote the basic logging formatter
 
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
```

