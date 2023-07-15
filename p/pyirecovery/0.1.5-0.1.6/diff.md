# Comparing `tmp/pyirecovery-0.1.5.tar.gz` & `tmp/pyirecovery-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirecovery-0.1.5.tar", max compression
+gzip compressed data, was "pyirecovery-0.1.6.tar", max compression
```

## Comparing `pyirecovery-0.1.5.tar` & `pyirecovery-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-06-16 17:10:08.642664 pyirecovery-0.1.5/LICENSE
--rw-r--r--   0        0        0      451 2023-06-16 17:10:08.642921 pyirecovery-0.1.5/README.md
--rw-r--r--   0        0        0      233 2023-06-16 17:10:08.644459 pyirecovery-0.1.5/pyirecovery/__init__.py
--rw-r--r--   0        0        0     7870 2023-06-18 14:11:29.167114 pyirecovery-0.1.5/pyirecovery/__main__.py
--rw-r--r--   0        0        0     2927 2023-07-01 23:47:57.391127 pyirecovery-0.1.5/pyirecovery/no_backend_fix.py
--rw-r--r--   0        0        0      470 2023-07-05 22:06:24.669999 pyirecovery-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 pyirecovery-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-16 17:10:08.642664 pyirecovery-0.1.6/LICENSE
+-rw-r--r--   0        0        0      451 2023-06-16 17:10:08.642921 pyirecovery-0.1.6/README.md
+-rw-r--r--   0        0        0      233 2023-06-16 17:10:08.644459 pyirecovery-0.1.6/pyirecovery/__init__.py
+-rw-r--r--   0        0        0     7926 2023-07-15 22:57:22.272878 pyirecovery-0.1.6/pyirecovery/__main__.py
+-rw-r--r--   0        0        0     2927 2023-07-01 23:47:57.391127 pyirecovery-0.1.6/pyirecovery/no_backend_fix.py
+-rw-r--r--   0        0        0      470 2023-07-15 22:57:28.348582 pyirecovery-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 pyirecovery-0.1.6/PKG-INFO
```

### Comparing `pyirecovery-0.1.5/LICENSE` & `pyirecovery-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyirecovery-0.1.5/pyirecovery/__main__.py` & `pyirecovery-0.1.6/pyirecovery/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 ret, cmd_arr = parse_command(cmd)
                 if ret == 0:
                     try:
                         # TODO: Remove the necessary of reset() before sending command
                         client.reset()
                         client.send_command(cmd, b_request=1 if is_breq_command(cmd) else 0)
                     except:
-                        pass
+                        click.secho(f'[WARNING] Caught exception: {e}', fg='yellow')
                 else:
                     if ret == CommandType.UPLOAD:
                         try:
                             cmd_arr[1]
                             with open(cmd_arr[1], 'rb') as f:
                                 data = f.read()
                         except:
```

### Comparing `pyirecovery-0.1.5/pyirecovery/no_backend_fix.py` & `pyirecovery-0.1.6/pyirecovery/no_backend_fix.py`

 * *Files identical despite different names*

### Comparing `pyirecovery-0.1.5/PKG-INFO` & `pyirecovery-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyirecovery
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 License: GPL-3.0-only
 Author: Mini-Exploit
 Author-email: miniexploitttt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

