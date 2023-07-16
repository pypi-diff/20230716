# Comparing `tmp/ssh_terminal_manager-0.6.0.tar.gz` & `tmp/ssh_terminal_manager-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.6.0.tar", last modified: Sat Jul 15 08:27:42 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.7.0.tar", last modified: Sun Jul 16 06:16:04 2023, max compression
```

## Comparing `ssh_terminal_manager-0.6.0.tar` & `ssh_terminal_manager-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.6.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.6.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-15 08:16:29.000000 ssh_terminal_manager-0.6.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.521275 ssh_terminal_manager-0.6.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.521275 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8370 2023-07-14 05:16:44.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-14 04:14:01.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:04.003744 ssh_terminal_manager-0.7.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.7.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-16 06:16:04.003744 ssh_terminal_manager-0.7.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.7.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-16 06:13:09.000000 ssh_terminal_manager-0.7.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-16 06:16:04.003744 ssh_terminal_manager-0.7.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:03.999744 ssh_terminal_manager-0.7.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:03.999744 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8529 2023-07-16 04:48:17.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-15 08:37:34.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-16 06:16:03.999744 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-16 06:16:03.000000 ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.6.0/LICENSE` & `ssh_terminal_manager-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.6.0/PKG-INFO` & `ssh_terminal_manager-0.7.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh_terminal_manager
-Version: 0.6.0
+Name: ssh-terminal-manager
+Version: 0.7.0
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ssh_terminal_manager-0.6.0/pyproject.toml` & `ssh_terminal_manager-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
@@ -20,14 +20,14 @@
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.6.0",
+  "terminal-manager >= 0.7.0",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.7.0/src/ssh_terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         self.on_change = Event()
 
     def update(self, name, value) -> None:
         if getattr(self, name) == value:
             return
 
         setattr(self, name, value)
-        self._manager.logger.info(
-            "[%s] State: %s => %s", self._manager.name, name, value
+        self._manager.logger.debug(
+            "%s: state.%s => %s", self._manager.name, name, value
         )
         self.on_change.notify(self)
 
 
 class SSHManager(Manager):
     def __init__(
         self,
@@ -139,20 +139,27 @@
             return CommandOutput(
                 time(),
                 ["".join(line.splitlines()) for line in stdout],
                 ["".join(line.splitlines()) for line in stderr],
                 stdout.channel.recv_exit_status(),
             )
         except TimeoutError as exc:
-            stdin.channel.close()
-            raise CommandError(f"Timeout of {timeout} seconds reached") from exc
+            pass
         except Exception as exc:
             self._disconnect()
             raise CommandError(f"Disconnected during execution ({exc})") from exc
 
+        try:
+            stdin.channel.close()
+        except Exception as exc:
+            self._disconnect()
+            raise CommandError(f"Disconnected after timeout ({exc})") from exc
+
+        raise CommandError("Channel closed after timeout")
+
     def _connect(self) -> None:
         if self.state.connected:
             return
 
         try:
             self.client.connect(
                 self.host,
@@ -237,15 +244,15 @@
             host = await icmplib.async_ping(
                 self.host,
                 count=1,
                 timeout=self.ping_timeout,
                 privileged=False,
             )
         except Exception as exc:  # pylint: disable=broad-except
-            self.logger.info("[%s] Ping request failed (%s)", self.name, exc)
+            self.logger.debug("%s: Ping request failed (%s)", self.name, exc)
             self.state.update(ONLINE, False)
         else:
             self.state.update(ONLINE, host.is_alive)
 
         if not self.state.online:
             if raise_errors:
                 raise OfflineError(f"Host is offline")
```

### Comparing `ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ssh-terminal-manager
-Version: 0.6.0
+Name: ssh_terminal_manager
+Version: 0.7.0
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

