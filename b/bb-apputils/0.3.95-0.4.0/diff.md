# Comparing `tmp/bb_apputils-0.3.95.tar.gz` & `tmp/bb_apputils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_apputils-0.3.95.tar", max compression
+gzip compressed data, was "bb_apputils-0.4.0.tar", max compression
```

## Comparing `bb_apputils-0.3.95.tar` & `bb_apputils-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    12923 2023-07-16 06:50:44.394357 bb_apputils-0.3.95/README.md
--rw-r--r--   0        0        0       50 2023-07-16 06:50:31.087690 bb_apputils-0.3.95/bbargparser/__init__.py
--rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.3.95/bbargparser/argparser.py
--rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.3.95/bblogger/__init__.py
--rw-r--r--   0        0        0    19517 2023-07-16 06:50:25.614356 bb_apputils-0.3.95/bblogger/logger.py
--rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.3.95/bblogger/texttools.py
--rw-r--r--   0        0        0      424 2023-07-16 06:50:39.134356 bb_apputils-0.3.95/pyproject.toml
--rw-r--r--   0        0        0    13284 1970-01-01 00:00:00.000000 bb_apputils-0.3.95/PKG-INFO
+-rw-r--r--   0        0        0    12989 2023-07-16 07:21:56.691059 bb_apputils-0.4.0/README.md
+-rw-r--r--   0        0        0       49 2023-07-16 07:22:04.837725 bb_apputils-0.4.0/bbargparser/__init__.py
+-rw-r--r--   0        0        0    11659 2023-02-18 23:07:14.840343 bb_apputils-0.4.0/bbargparser/argparser.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:14:48.427104 bb_apputils-0.4.0/bblogger/__init__.py
+-rw-r--r--   0        0        0    19605 2023-07-16 07:20:06.824390 bb_apputils-0.4.0/bblogger/logger.py
+-rw-r--r--   0        0        0    11757 2022-11-06 23:50:55.000000 bb_apputils-0.4.0/bblogger/texttools.py
+-rw-r--r--   0        0        0      423 2023-07-16 07:22:14.131059 bb_apputils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13349 1970-01-01 00:00:00.000000 bb_apputils-0.4.0/PKG-INFO
```

### Comparing `bb_apputils-0.3.95/README.md` & `bb_apputils-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
 
     """
         Options would be set as '-i', '--input-file' and '-o', '--output-file'. The '-i'
       option will only accept an existing file as an argument and the '-o' option will
       accept an argument that matches a path format, regardless of whether it exists. opts(...)
       will return a key, item list from the provided user arguments. The '.items()' function
       should not be used when calling the class with user arguments. If no arguments are given,
-      self (dict) is returned. The default is to clear self every time it is called inless 'clear'
+      self (dict) is returned. The default is to clear self every time it is called unless 'clear'
       is set to False.
 
     """
 
 ```
 
 ## Changelog
@@ -333,15 +333,18 @@
 - 0.3.91
     - fixed typo in basic logging.... maybe
 
 - 0.3.92
     - 2nd attempt at fixing basic logging
 
 - 0.3.95
-    - rewrote the basic logging formatter
+    - yet another attempt to get basic log formatting right
+
+- 0.4.0
+    - re-wrote the basic log formatter
 
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
```

### Comparing `bb_apputils-0.3.95/bbargparser/argparser.py` & `bb_apputils-0.4.0/bbargparser/argparser.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.95/bblogger/logger.py` & `bb_apputils-0.4.0/bblogger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,50 +149,52 @@
         log_fmt = self.FORMAT.get(record.levelno)
         if self.mode == 'basic':
             try:
                 width = os.get_terminal_size().columns
             except:
                 width = 200
             msg = record.getMessage()
-            if len(msg) + len(record.levelname) + 21 > width:
-                length = 13
-                words, msg_lines, indent = msg.split(), [''], f"{'    ':.<{length - 4}}"
+            if len(msg) + len(record.levelname) + 19 > width:
+                length = len(record.levelname) + 6
+                words, msg_lines, indent = msg.split(), [''], f"{'':<{length}}"
                 while words:
                     if len(words[0]) + length + 2 > width:
                         if len(msg_lines[-1]) < int(width*.7):
-                            left = width - len(msg_lines[-1]) - 2
+                            left = width - len(msg_lines[-1]) - 1
                             split_word = words.pop(0)
                             word = split_word[:left]
                             msg_lines[-1] += f" {word}"
-                            msg_lines.append( f"{indent}" )
                             words.insert( 0, split_word[left:] )
+                            msg_lines.append( f"{indent}" )
                         else:
                             msg_lines.append( f"{indent}" )
 
                         length = len(msg_lines[-1])
 
                     else:
                         word = f" {words.pop(0)}"
                         length += len(word)
                         msg_lines[-1] += word
 
-                    if not words and length + 15 > width:
+                    if not words and length + 15 >= width:
                         msg_lines.append( f"{indent}" )
                         length = len(msg_lines[-1])
+                        break
 
-                space = width - length - 14
-                if space > 0:
-                    msg_lines[-1] += f"{'':.<{space}}"
-
+                space = width - length - 15
                 record.msg = '\n'.join(msg_lines)
 
             else:
-                space = width - 21 - len(record.levelname) - ( len(msg) - ( int(len(msg) / width) * width ))
+                space = width - 20 - len(record.levelname) - ( len(msg) - ( int(len(msg) / width) * width ))
+
+            if space > 0:
+                log_fmt = f"{log_fmt}  {' ':.>{space}}"+"-\x1b[1;37m"+" %(asctime)s"+"\x1b[0m"
+            else:
+                log_fmt = f"{log_fmt}  "+"-\x1b[1;37m"+" %(asctime)s"+"\x1b[0m"
 
-            log_fmt = f"{log_fmt}  {' ':.>{space}}"+"-\x1b[1;37m"+" %(asctime)s"+"\x1b[0m"
             formatter = logging.Formatter(log_fmt, '[%R:%S]')
 
         elif self.mode == 'debug':
             formatter = logging.Formatter(log_fmt, '[%R:%S]')
 
         elif self.mode == 'html' or self.mode == 'plaintext':
             formatter = logging.Formatter(log_fmt, '%a, %m/%d/%y [%R:%S]:')
```

### Comparing `bb_apputils-0.3.95/bblogger/texttools.py` & `bb_apputils-0.4.0/bblogger/texttools.py`

 * *Files identical despite different names*

### Comparing `bb_apputils-0.3.95/PKG-INFO` & `bb_apputils-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-apputils
-Version: 0.3.95
+Version: 0.4.0
 Summary: App utilities
 Author: Erik Beebe
 Author-email: beebeapps_debugging@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -319,15 +319,15 @@
 
     """
         Options would be set as '-i', '--input-file' and '-o', '--output-file'. The '-i'
       option will only accept an existing file as an argument and the '-o' option will
       accept an argument that matches a path format, regardless of whether it exists. opts(...)
       will return a key, item list from the provided user arguments. The '.items()' function
       should not be used when calling the class with user arguments. If no arguments are given,
-      self (dict) is returned. The default is to clear self every time it is called inless 'clear'
+      self (dict) is returned. The default is to clear self every time it is called unless 'clear'
       is set to False.
 
     """
 
 ```
 
 ## Changelog
@@ -345,15 +345,18 @@
 - 0.3.91
     - fixed typo in basic logging.... maybe
 
 - 0.3.92
     - 2nd attempt at fixing basic logging
 
 - 0.3.95
-    - rewrote the basic logging formatter
+    - yet another attempt to get basic log formatting right
+
+- 0.4.0
+    - re-wrote the basic log formatter
 
 ## Thanks To:
 
 ##### Colored logging with logging.Formatter()
 
 <p>Thread at <a href="https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output">Stack Overflow</a> on python log formatting</p>
```

