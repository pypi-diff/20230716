# Comparing `tmp/logium-0.5.tar.gz` & `tmp/logium-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logium-0.5.tar", last modified: Sat Jul 15 22:49:29 2023, max compression
+gzip compressed data, was "logium-1.0.tar", last modified: Sat Jul 15 23:37:07 2023, max compression
```

## Comparing `logium-0.5.tar` & `logium-1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 22:49:29.163873 logium-0.5/
--rw-rw-rw-   0        0        0      157 2023-07-15 22:49:29.163873 logium-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 22:49:29.146231 logium-0.5/logium/
--rw-rw-rw-   0        0        0     6026 2023-07-15 22:48:39.000000 logium-0.5/logium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 22:49:29.162856 logium-0.5/logium.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-15 22:49:29.000000 logium-0.5/logium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-15 22:49:29.000000 logium-0.5/logium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 22:49:29.000000 logium-0.5/logium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 22:49:29.000000 logium-0.5/logium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 22:49:29.165871 logium-0.5/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-15 22:48:50.000000 logium-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:37:07.688676 logium-1.0/
+-rw-rw-rw-   0        0        0      157 2023-07-15 23:37:07.688676 logium-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 23:37:07.668450 logium-1.0/logium/
+-rw-rw-rw-   0        0        0     6067 2023-07-15 23:35:48.000000 logium-1.0/logium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:37:07.688676 logium-1.0/logium.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 23:37:07.000000 logium-1.0/logium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 23:37:07.688676 logium-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-07-15 23:35:35.000000 logium-1.0/setup.py
```

### Comparing `logium-0.5/logium/__init__.py` & `logium-1.0/logium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A simple logging library for recording and displaying log messages.
 
 Author: N0rmalUser
-Version: 0.5
+Version: 1.0
 
 This library provides a Logger class that allows you to log messages with various severity levels. The log messages can be output to the console and/or saved to a log file with timestamps.
 
 Usage:
 1. Create an instance of the Logger class by providing the log file name and optional settings.
 2. Use the logger instance to call different logging methods based on the severity level.
 3. The log messages will be printed to the console and/or appended to the log file.
@@ -67,16 +67,17 @@
 def _printer(self):
     """
     The inner function for printing the message to the console and/or file
     """
     if self.console_enabled:
         print(f'{self.time} {self.message}' if self.console_enabled and self.date_in_console else self.message)
     if self.file_enable:
+        file_output = f'{self.time} {self.message}' if self.file_enable and self.date_in_file else self.message
         with open(self.file[0], "a", encoding='utf-8') as f:
-            f.write(f'{self.time} {self.message}\n' if self.file_enable and self.date_in_file else self.message)
+            f.write(f'{file_output}\n')
 
 
 def _tagger(func):
     """
     The inner decorator function tagger takes a function and adds a tag to the message.
     """
     def wrapper(self, *args):
@@ -120,15 +121,15 @@
         self.message = ''
 
     @_tagger  # debug
     def d(self) -> None:
         """
         Decorator method for debug messages
         """
-        self.message = '-DEBUG-' + self.message
+        self.message = '-DEBUG- ' + self.message
         _printer(self)
 
     @_tagger  # error
     def e(self) -> None:
         """
         Decorator method for error messages
         """
```

