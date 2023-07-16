# Comparing `tmp/coffeepy-0.1.6.tar.gz` & `tmp/coffeepy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeepy-0.1.6.tar", last modified: Fri Jul 14 19:33:01 2023, max compression
+gzip compressed data, was "coffeepy-0.1.7.tar", last modified: Sun Jul 16 11:17:43 2023, max compression
```

## Comparing `coffeepy-0.1.6.tar` & `coffeepy-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 19:32:51.000000 coffeepy-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-14 19:33:01.968010 coffeepy-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-14 19:32:51.000000 coffeepy-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 19:32:51.000000 coffeepy-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:33:01.968010 coffeepy-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.964010 coffeepy-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/src/coffeepy/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 19:32:51.000000 coffeepy-0.1.6/src/coffeepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-14 19:32:51.000000 coffeepy-0.1.6/src/coffeepy/coffeepy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/src/coffeepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 19:33:01.000000 coffeepy-0.1.6/src/coffeepy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:33:01.968010 coffeepy-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-14 19:32:51.000000 coffeepy-0.1.6/tests/test_coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-16 11:17:32.000000 coffeepy-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 11:17:43.625823 coffeepy-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-16 11:17:32.000000 coffeepy-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-16 11:17:32.000000 coffeepy-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:17:43.625823 coffeepy-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/src/coffeepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 11:17:32.000000 coffeepy-0.1.7/src/coffeepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-16 11:17:32.000000 coffeepy-0.1.7/src/coffeepy/coffeepy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/src/coffeepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 11:17:43.000000 coffeepy-0.1.7/src/coffeepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:17:43.625823 coffeepy-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-16 11:17:32.000000 coffeepy-0.1.7/tests/test_coffeepy.py
```

### Comparing `coffeepy-0.1.6/LICENSE` & `coffeepy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.6/PKG-INFO` & `coffeepy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `coffeepy-0.1.6/README.md` & `coffeepy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `coffeepy-0.1.6/pyproject.toml` & `coffeepy-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coffeepy"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="kuvaus", email="coffeepy@kuvaus.org" },
 ]
 description = "Coffeepy prevents the system from sleeping"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `coffeepy-0.1.6/src/coffeepy/coffeepy.py` & `coffeepy-0.1.7/src/coffeepy/coffeepy.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
                 if 'win32' in sys.platform:
                     if check_windows_terminal() == True:
                         display_animation()
                     else:
                         display_animation(ascii_animation)
                 else:
                     display_animation()
+            else:
+                time.sleep(1)
 
     except KeyboardInterrupt:
         print('\nExiting')
 
     finally:
         if proc:
             proc.terminate()
```

### Comparing `coffeepy-0.1.6/src/coffeepy.egg-info/PKG-INFO` & `coffeepy-0.1.7/src/coffeepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coffeepy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Coffeepy prevents the system from sleeping
 Author-email: kuvaus <coffeepy@kuvaus.org>
 Project-URL: Homepage, https://github.com/kuvaus/coffeepy
 Project-URL: Bug Tracker, https://github.com/kuvaus/coffeepy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `coffeepy-0.1.6/tests/test_coffeepy.py` & `coffeepy-0.1.7/tests/test_coffeepy.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,53 +126,52 @@
         run(runtime)
 
     def test_timed_run():
         runtime = 0.01
         run(runtime)
 
 #
-# Test the run function
-# Then test run with macos, linux and windows
+# Test run on macos, linux and windows
 #
 
 # macOS
 # Use mock to simulate 'check_caffeinate'
 #
 @patch('sys.platform', new='darwin')
 @patch('subprocess.Popen')
 @patch('subprocess.check_output')
-def test_run_on_linux_with_caffeinate(mock_subproc, mock_popen):
+def test_platform_macos(mock_subproc, mock_popen):
     mock_subproc.return_value = '/usr/bin/caffeinate'
     mock_popen.return_value.returncode = 0
     runtime = 0.01
     run(runtime)
     mock_popen.assert_called_once_with(['caffeinate', '-dims'])
 
 #
 # Linux and caffeinate
 # Use mock to simulate 'check_caffeinate'
 #
 @patch('sys.platform', new='linux')
 @patch('subprocess.Popen')
 @patch('subprocess.check_output')
-def test_run_on_linux_with_caffeinate(mock_subproc, mock_popen):
+def test_platform_linux_with_caffeinate(mock_subproc, mock_popen):
     mock_subproc.return_value = '/usr/bin/caffeinate'
     mock_popen.return_value.returncode = 0
     runtime = 0.01
     run(runtime)
     mock_popen.assert_called_once_with(['caffeinate', '-dims'])
 
 #
 # Linux
 # Use mock to simulate 'subprocess.Popen'
 #
 @patch('sys.platform', new='linux')
 @patch('subprocess.Popen')
 @patch('subprocess.check_output')
-def test_run_on_linux_without_caffeinate(mock_subproc, mock_popen):
+def test_plaform_linux_without_caffeinate(mock_subproc, mock_popen):
     mock_subproc.side_effect = subprocess.CalledProcessError(1, 'which')
     mock_popen.return_value.returncode = 0
     runtime = 0.01
     run(runtime)
     calls = [call(['xset', 's', 'off']), call(['xset', '-dpms'])]
     mock_popen.assert_has_calls(calls, any_order=True)
 
@@ -182,7 +181,8 @@
 #
 @patch('sys.platform', new='win32')
 @patch('ctypes.windll', create=True)
 def test_platform_windows(self):
     runtime = 0.01
     run(runtime)
 
+
```

