# Comparing `tmp/snap-helpers-0.3.2.tar.gz` & `tmp/snap-helpers-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap-helpers-0.3.2.tar", last modified: Sat Jan 14 09:09:36 2023, max compression
+gzip compressed data, was "snap-helpers-0.4.0.tar", last modified: Sun Jul 16 17:10:42 2023, max compression
```

## Comparing `snap-helpers-0.3.2.tar` & `snap-helpers-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,29 @@
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-01-14 09:09:36.893046 snap-helpers-0.3.2/
--rw-rw-r--   0 ack       (1000) ack       (1000)     1717 2023-01-14 09:08:51.000000 snap-helpers-0.3.2/CHANGES.rst
--rw-rw-r--   0 ack       (1000) ack       (1000)     7652 2019-03-06 14:04:03.000000 snap-helpers-0.3.2/LICENSE.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       43 2021-10-29 22:32:22.000000 snap-helpers-0.3.2/MANIFEST.in
--rw-rw-r--   0 ack       (1000) ack       (1000)     9009 2023-01-14 09:09:36.893046 snap-helpers-0.3.2/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)     8213 2022-12-03 09:17:20.000000 snap-helpers-0.3.2/README.rst
--rw-rw-r--   0 ack       (1000) ack       (1000)      475 2022-12-07 09:53:03.000000 snap-helpers-0.3.2/pyproject.toml
--rw-rw-r--   0 ack       (1000) ack       (1000)     2175 2023-01-14 09:09:36.897046 snap-helpers-0.3.2/setup.cfg
--rw-r--r--   0 ack       (1000) ack       (1000)       38 2019-11-12 21:47:16.000000 snap-helpers-0.3.2/setup.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-01-14 09:09:36.893046 snap-helpers-0.3.2/snap_helpers.egg-info/
--rw-rw-r--   0 ack       (1000) ack       (1000)     9009 2023-01-14 09:09:36.000000 snap-helpers-0.3.2/snap_helpers.egg-info/PKG-INFO
--rw-rw-r--   0 ack       (1000) ack       (1000)      668 2023-01-14 09:09:36.000000 snap-helpers-0.3.2/snap_helpers.egg-info/SOURCES.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-01-14 09:09:36.000000 snap-helpers-0.3.2/snap_helpers.egg-info/dependency_links.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       73 2023-01-14 09:09:36.000000 snap-helpers-0.3.2/snap_helpers.egg-info/entry_points.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       47 2023-01-14 09:09:36.000000 snap-helpers-0.3.2/snap_helpers.egg-info/requires.txt
--rw-rw-r--   0 ack       (1000) ack       (1000)       12 2023-01-14 09:09:36.000000 snap-helpers-0.3.2/snap_helpers.egg-info/top_level.txt
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-01-14 09:09:36.893046 snap-helpers-0.3.2/snaphelpers/
--rw-rw-r--   0 ack       (1000) ack       (1000)      790 2023-01-11 22:18:18.000000 snap-helpers-0.3.2/snaphelpers/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3728 2023-01-11 21:33:18.000000 snap-helpers-0.3.2/snaphelpers/_conf.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     8156 2022-12-07 09:53:03.000000 snap-helpers-0.3.2/snaphelpers/_ctl.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1528 2022-12-07 09:53:03.000000 snap-helpers-0.3.2/snaphelpers/_env.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1808 2022-11-12 21:45:07.000000 snap-helpers-0.3.2/snaphelpers/_health.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1648 2022-12-07 09:53:03.000000 snap-helpers-0.3.2/snaphelpers/_hook.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2114 2022-12-03 09:25:20.000000 snap-helpers-0.3.2/snaphelpers/_meta.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      880 2022-12-07 09:53:03.000000 snap-helpers-0.3.2/snaphelpers/_path.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     2422 2022-11-12 21:45:07.000000 snap-helpers-0.3.2/snaphelpers/_service.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1487 2022-11-19 01:18:35.000000 snap-helpers-0.3.2/snaphelpers/_snap.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     3606 2023-01-11 21:33:18.000000 snap-helpers-0.3.2/snaphelpers/conftest.py
-drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-01-14 09:09:36.893046 snap-helpers-0.3.2/snaphelpers/scripts/
--rw-r--r--   0 ack       (1000) ack       (1000)        0 2019-03-07 17:24:09.000000 snap-helpers-0.3.2/snaphelpers/scripts/__init__.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     1430 2022-12-07 09:53:03.000000 snap-helpers-0.3.2/snaphelpers/scripts/_script.py
--rw-rw-r--   0 ack       (1000) ack       (1000)      532 2022-12-03 08:52:33.000000 snap-helpers-0.3.2/snaphelpers/scripts/conftest.py
--rw-rw-r--   0 ack       (1000) ack       (1000)     4228 2022-12-07 09:37:41.000000 snap-helpers-0.3.2/snaphelpers/scripts/snaphelpers.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/
+-rw-rw-r--   0 ack       (1000) ack       (1000)     7652 2019-03-06 14:04:03.000000 snap-helpers-0.4.0/LICENSE.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)    18980 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)     8758 2023-04-06 22:14:25.000000 snap-helpers-0.4.0/README.rst
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2301 2023-07-16 16:35:24.000000 snap-helpers-0.4.0/pyproject.toml
+-rw-rw-r--   0 ack       (1000) ack       (1000)       38 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/setup.cfg
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/snap_helpers.egg-info/
+-rw-rw-r--   0 ack       (1000) ack       (1000)    18980 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/PKG-INFO
+-rw-rw-r--   0 ack       (1000) ack       (1000)      596 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/SOURCES.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)        1 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/dependency_links.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       73 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/entry_points.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       84 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/requires.txt
+-rw-rw-r--   0 ack       (1000) ack       (1000)       12 2023-07-16 17:10:42.000000 snap-helpers-0.4.0/snap_helpers.egg-info/top_level.txt
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/snaphelpers/
+-rw-rw-r--   0 ack       (1000) ack       (1000)      670 2023-07-16 16:46:21.000000 snap-helpers-0.4.0/snaphelpers/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     3798 2023-03-15 07:35:35.000000 snap-helpers-0.4.0/snaphelpers/_conf.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     9301 2023-04-22 08:36:28.000000 snap-helpers-0.4.0/snaphelpers/_ctl.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1590 2023-03-15 07:43:44.000000 snap-helpers-0.4.0/snaphelpers/_env.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1862 2023-03-05 09:31:10.000000 snap-helpers-0.4.0/snaphelpers/_health.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1768 2023-07-16 16:35:24.000000 snap-helpers-0.4.0/snaphelpers/_hook.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      366 2023-07-16 16:35:24.000000 snap-helpers-0.4.0/snaphelpers/_importlib.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2244 2023-03-11 23:44:03.000000 snap-helpers-0.4.0/snaphelpers/_meta.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)      964 2023-03-11 23:44:03.000000 snap-helpers-0.4.0/snaphelpers/_path.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     2585 2023-03-05 09:31:10.000000 snap-helpers-0.4.0/snaphelpers/_service.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1949 2023-03-15 07:42:04.000000 snap-helpers-0.4.0/snaphelpers/_snap.py
+drwxrwxr-x   0 ack       (1000) ack       (1000)        0 2023-07-16 17:10:42.927907 snap-helpers-0.4.0/snaphelpers/scripts/
+-rw-rw-r--   0 ack       (1000) ack       (1000)        0 2023-02-27 23:36:00.000000 snap-helpers-0.4.0/snaphelpers/scripts/__init__.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     1434 2023-03-14 16:12:46.000000 snap-helpers-0.4.0/snaphelpers/scripts/_script.py
+-rw-rw-r--   0 ack       (1000) ack       (1000)     4666 2023-03-14 19:36:28.000000 snap-helpers-0.4.0/snaphelpers/scripts/snap_helpers.py
```

### Comparing `snap-helpers-0.3.2/LICENSE.txt` & `snap-helpers-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snap-helpers-0.3.2/PKG-INFO` & `snap-helpers-0.4.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,15 @@
-Metadata-Version: 2.1
-Name: snap-helpers
-Version: 0.3.2
-Summary: Helpers for interacting with the Snap system within a Snap
-Home-page: https://github.com/albertodonato/snap-helpers
-Author: Alberto Donato
-Author-email: alberto.donato@gmail.com
-Maintainer: Alberto Donato
-Maintainer-email: alberto.donato@gmail.com
-License: LGPLv3+
-Keywords: snap,snappy,snapcraft
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Archiving :: Packaging
-Classifier: Topic :: System :: Software Distribution
-Requires-Python: >=3.6
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 snap-helpers - Interact with the Snap system within a Snap
 ==========================================================
 
 |Latest Version| |Snap Package| |Build Status| |Coverage Status| |Documentation|
 
 
-A Python library to interact with snap configuration and properties from inside a snap.
+A Python library to interact with snap configuration and properties from inside
+a snap.
 
 It exposes a top-level ``snaphelpers.Snap`` object which provides access to:
 
 - snap details:
 
   .. code:: python
 
@@ -127,14 +106,20 @@
 
   These can be accessed as follows:
 
   .. code:: python
 
      >>> snap.metadata_files.snap
      SnapMetadataFile(/snap/snap-helpers/138/meta/snap.yaml)
+     >>> snap.metadata_files.snap.path
+     PosixPath('/snap/snap-helpers/138/meta/snap.yaml')
+     >>> snap.metadata_files.snap["name"]
+     'snap-helpers'
+     >>> snap.metadata_files.snap["base"]
+     'core22'
      >>> pprint.pprint(dict(snap.metadata_files.snap))
      {'apps': {'python': {'command': 'bin/python3',
                           'plugs': ['home', 'network', 'network-bind']},
                'snap-helpers': {'command': 'bin/snap-helpers-shell',
                                 'plugs': ['home', 'network', 'network-bind']}},
       'architectures': ['amd64'],
       'base': 'core22',
@@ -158,39 +143,47 @@
       'summary': 'Test snap for the snap-helpers Python library.',
       'version': '0.3.0+git5.5794660'}
 
 
 Hook helpers
 ------------
 
-The library provides helpers to reduce boilerplate when setting up hooks for the snap.
+The library provides helpers to reduce boilerplate when setting up hooks for
+the snap, by using ``entry-points`` in the package metadata.
 
-Hooks can be defined by simply registering functions to be called as hooks via
-``entry_points`` in the application ``setup.py``:
+This can be done in ``setup.py``:
 
 .. code:: python
 
    setup(
        # ...
        entry_points={
            "snaphelpers.hooks": [
                "configure = testapp:configure_hook",
                "install = testapp:install_hook",
            ]
        }
    )
 
-or in ``setup.cfg`` with:
+or in ``setup.cfg``:
 
 .. code:: ini
 
    [options.entry_points]
    snaphelpers.hooks =
-       install = testapp:install_hook
        configure = testapp:configure_hook
+       install = testapp:install_hook
+
+or in ``pyproject.toml``:
+
+.. code:: toml
+
+   [project.entry-points."snaphelpers.hooks"]
+   configure = "testapp:configure_hook"
+   install = "testapp:install_hook"
 
 
 Hook functions are called with a ``Snap`` object as argument:
 
 .. code:: python
 
    def install_hook(snap: snaphelpers.Snap):
@@ -200,20 +193,30 @@
    def configure_hook(snap: snaphelpers.Snap):
        # ...
 
 ``snap-helpers`` will take care of the hooks plumbing (i.e. creating hook files
 in ``$SNAP/snap/hooks``).
 
 
+Supported snap bases
+--------------------
+
+Currently supported snap bases are:
+
+- ``core20`` (Python 3.8)
+- ``core22`` (Python 3.10)
+
+The ``core18`` base (with Python 3.6) is supported until the ``0.3.2`` release.
+
 
 Testing with the snap
 ---------------------
 
-The ``snap-helpers`` snap provides a way to easily test code using the library in
-a real snap environment with strict confinement.
+The ``snap-helpers`` snap provides a way to easily test code using the library
+in a real snap environment with strict confinement.
 
 It provides an IPython_ shell which automatically imports the ``snaphelpers``
 module and provides a ``Snap`` instance for the current snap.
 
 .. code::
 
    $ snap-helpers
@@ -285,9 +288,7 @@
    :target: https://github.com/albertodonato/snap-helpers/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://img.shields.io/codecov/c/github/albertodonato/snap-helpers/main.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/albertodonato/snap-helpers
 .. |Documentation| image:: https://readthedocs.org/projects/snap-helpers/badge/?version=stable
    :alt: Documentation
    :target: https://snap-helpers.readthedocs.io/en/stable/?badge=stable
-
-
```

### Comparing `snap-helpers-0.3.2/snaphelpers/__init__.py` & `snap-helpers-0.4.0/snaphelpers/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 """Helpers for interacting with the Snap system within a Snap."""
 
-from packaging.version import parse
-from pkg_resources import get_distribution
-
 from ._conf import (
     InvalidKey,
     SnapConfig,
     SnapConfigOptions,
     UnknownConfigKey,
 )
 from ._ctl import (
@@ -34,8 +31,8 @@
     "SnapHealth",
     "SnapPaths",
     "SnapServices",
     "UnknownConfigKey",
     "__version__",
 ]
 
-__version__ = parse(get_distribution("snap-helpers").version)
+__version__ = "0.4.0"
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_conf.py` & `snap-helpers-0.4.0/snaphelpers/_conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 from ._ctl import SnapCtl
 
 
 class UnknownConfigKey(Exception):
     """The specified config key is unknown."""
 
+    #: The unknown key
     key: str
 
     def __init__(self, key: str):
         self.key = key
         super().__init__(f"Unknown config key: {key}")
 
 
 class InvalidKey(Exception):
     """The specified key is invalid."""
 
+    #: The invalid key
     key: str
 
     def __init__(self, key: str):
         self.key = key
         super().__init__(f"Invalid top-level key: {key}")
 
 
@@ -75,15 +77,15 @@
 
         """
         try:
             return self[key]
         except UnknownConfigKey:
             return default
 
-    def fetch(self):
+    def fetch(self) -> None:
         """Fetch (or refresh) configuration for the set of keys."""
         self._config = self._snapctl.config_get(*self._keys)
 
     def as_dict(self) -> Dict[str, Any]:
         """Return the configuration as a :class:`dict`."""
         if self._config is None:
             return {}
@@ -119,22 +121,22 @@
         :raises UnknownConfigKey: if the option doesn't exist.
 
         """
         top_key = key.split(".", maxsplit=1)[0]
         options = self.get_options(top_key)
         return options[key]
 
-    def set(self, options: Dict[str, Any]):
+    def set(self, options: Dict[str, Any]) -> None:
         """Set config options.
 
         :param options: a dict with configs. Keys can use dotted notation.
 
         """
         self._snapctl.config_set(options)
 
-    def unset(self, options: List[str]):
+    def unset(self, options: List[str]) -> None:
         """Unset snap configuration keys.
 
         :param options: A list of keys to unset. Keys can use dotted notation.
 
         """
         self._snapctl.config_unset(*options)
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_ctl.py` & `snap-helpers-0.4.0/snaphelpers/_ctl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,172 +1,182 @@
+from __future__ import annotations  # for subscritable Popen type
+
 from enum import Enum
 import json
 import re
 from subprocess import (
     PIPE,
     Popen,
 )
 from typing import (
     Any,
     cast,
     Dict,
     IO,
-    List,
     NamedTuple,
-    Optional,
     Sequence,
-    Tuple,
 )
 
+import yaml
+
 from ._env import SnapEnviron
 
 
 class ServiceInfo(NamedTuple):
     """Information for a service in the snap."""
 
+    #: Name of the service
     name: str
+    #: Whether the service is enabled
     enabled: bool
+    #: Whether the service is active
     active: bool
-    notes: List[str]
+    #: Additional metadata about the service
+    notes: list[str]
 
 
 class SnapHealthStatus(Enum):
     """Possible values for snap health status."""
 
     OKAY = "okay"
     WAITING = "waiting"
     BLOCKED = "blocked"
     ERROR = "error"
 
 
 class SnapCtlError(Exception):
     """A snapctl command failed."""
 
+    #: The process return code
     returncode: int
+    #: The error message
     error: str
 
-    def __init__(self, process: Popen):
+    def __init__(self, process: Popen[bytes]):
         self.returncode = process.returncode
-        self.error = cast(IO, process.stderr).read().decode("utf-8")
+        self.error = cast(IO[bytes], process.stderr).read().decode("utf-8")
         super().__init__(
-            f"Call to snapctl failed with error {self.returncode}: " + self.error
+            f"Call to snapctl failed with error {self.returncode}: "
+            + self.error
         )
 
 
 class SnapCtl:
     """Run the :data:`snapctl` command."""
 
     _SERVICE_RE = re.compile(
         r"[^.]+\.(?P<name>\S+)\s+"
         r"(?P<startup>\S+)\s+"
         r"(?P<current>\S+)\s+"
         r"(?P<notes>\S+)"
     )
 
     def __init__(
-        self, executable: str = "/usr/bin/snapctl", env: Optional[SnapEnviron] = None
+        self,
+        executable: str = "/usr/bin/snapctl",
+        env: SnapEnviron | None = None,
     ):
         if env is None:
             env = SnapEnviron()
         self._executable = executable
         self._instance_name = env.INSTANCE_NAME
 
-    def start(self, *services: str, enable: bool = False):
+    def start(self, *services: str, enable: bool = False) -> None:
         """Start all or specified services in the snap.
 
         :param services: a list of services defined in the snap to start.
           If not specified, all services will be started.
         :param enable: whether to also enable services at startup.
 
         """
         self._run_for_services("start", services, options={"enable": enable})
 
-    def stop(self, *services: str, disable: bool = False):
+    def stop(self, *services: str, disable: bool = False) -> None:
         """Stop all or specified services in the snap.
 
         :param services: a list of services defined in the snap to stop.
           If not specified, all services will be stopped.
         :param disable: whether to also disable services at startup.
 
         """
         self._run_for_services("stop", services, options={"disable": disable})
 
-    def restart(self, *services: str, reload: bool = False):
+    def restart(self, *services: str, reload: bool = False) -> None:
         """Restart all or specified services in the snap.
 
         :param services: a list of services defined in the snap to restart.
           If not specified, all services will be restarted.
         :param reload: whether to reload services if supported.
 
         """
         self._run_for_services("restart", services, options={"reload": reload})
 
-    def services(self, *services: str) -> List[ServiceInfo]:
+    def services(self, *services: str) -> list[ServiceInfo]:
         """Return info about services in the snap.
 
         :param services: a list of services to return info for.
           If not specified, all services are returned.
 
         """
         lines = self._run_for_services("services", services)
         service_infos = []
         # skip header
         for line in lines.splitlines()[1:]:
             match = self._SERVICE_RE.match(line)
             if match:
                 info = match.groupdict()
-                notes: List[str] = []
+                notes: list[str] = []
                 if info["notes"] != "-":
                     notes = info["notes"].split(",")
                 service_infos.append(
                     ServiceInfo(
                         name=info["name"],
                         enabled=info["startup"] == "enabled",
                         active=info["current"] == "active",
                         notes=notes,
                     )
                 )
         return service_infos
 
-    def config_get(self, *keys: str) -> Dict[str, Any]:
+    def config_get(self, *keys: str) -> dict[str, Any]:
         """Return the snap configuration.
 
         :param keys: a list of config keys to return.
 
         """
-        conf: Dict[str, Any]
+        conf: dict[str, Any]
         conf = json.loads(self.run("get", "-d", *keys))
         return conf
 
-    def config_set(self, configs: Dict[str, Any]):
+    def config_set(self, configs: dict[str, Any]) -> None:
         """Set snap configuration.
 
         :param configs: a dict with configs. Keys can use dotted notation.
 
         """
         self.run("set", *self._set_args(configs))
 
-    def config_unset(self, *keys: str):
+    def config_unset(self, *keys: str) -> None:
         """Unset snap configuration keys.
 
         :param keys: config keys to unset.
 
         """
         self.run("set", *self._unset_args(keys))
 
-    def connection_set(self, name: str, configs: Dict[str, Any]):
+    def connection_set(self, name: str, configs: dict[str, Any]) -> None:
         """Set plug or slot configuration.
 
         :param name: the plug/slot name.
         :param configs: a dict with configs. Keys can use dotted notation.
 
         """
         self.run("set", f":{name}", *self._set_args(configs))
 
-    def connection_unset(self, name: str, *keys: str):
+    def connection_unset(self, name: str, *keys: str) -> None:
         """Unset plug or slot configuration.
 
         :param name: the plug/slot name.
         :param keys: keys to unset. Dotted notation can be used.
 
         """
         self.run("set", f":{name}", *self._unset_args(keys))
@@ -179,97 +189,124 @@
         """
         try:
             self.run("is-connected", name)
         except SnapCtlError:
             return False
         return True
 
-    def plug_get(self, name: str, *keys: str, remote: bool = False) -> Dict[str, Any]:
+    def plug_get(
+        self, name: str, *keys: str, remote: bool = False
+    ) -> dict[str, Any]:
         """Return plug configuration.
 
         :param name: the plug name.
         :param keys: a list of config keys to return.
         :param remote: if True, return configs from the remote end.
 
         """
         remote_type = "slot" if remote else None
         return self._connection_get(name, keys, remote_type=remote_type)
 
-    def slot_get(self, name: str, *keys: str, remote: bool = False) -> Dict[str, Any]:
+    def slot_get(
+        self, name: str, *keys: str, remote: bool = False
+    ) -> dict[str, Any]:
         """Return slot configuration.
 
         :param name: the slot name.
         :param keys: a list of config keys to return.
         :param remote: if True, return configs from the remote end.
 
         """
         remote_type = "plug" if remote else None
         return self._connection_get(name, keys, remote_type=remote_type)
 
     def set_health(
         self,
         status: SnapHealthStatus,
-        message: Optional[str] = None,
-        code: Optional[str] = None,
-    ):
+        message: str | None = None,
+        code: str | None = None,
+    ) -> None:
         """Set snap health.
 
         :param status: the status to set
         :param message: an optional message string
         :param code: an optional code string
 
         """
         args = [status.value]
         if message is not None:
             args.append(message)
         if code is not None:
             args.extend(["--code", code])
         self.run("set-health", *args)
 
+    def system_mode(self) -> dict[str, Any]:
+        """Return info on the device current system mode."""
+        mode: dict[str, Any] = yaml.safe_load(self.run("system-mode"))
+        return mode
+
+    def refresh(self, action: str | None = None) -> dict[str, Any]:
+        """Return refresh state of the snap, optionally requesting an action.
+
+        To perform actions, the snap must have the ``snap-refresh-control``
+        interface.
+
+        :param action: Optional refresh action to perform, either ``proceed``
+          or ``hold``.
+
+        """
+        args = ["--pending"]
+        if action:
+            args.append(f"--{action}")
+        return cast(Dict[str, Any], yaml.safe_load(self.run("refresh", *args)))
+
     def run(self, *args: str) -> str:
         """Execute the command and return its output.
 
         :param args: command args.
 
         """
         process = Popen([self._executable, *args], stdout=PIPE, stderr=PIPE)
         process.wait()
         if process.returncode:
             raise SnapCtlError(process)
-        output: bytes = cast(IO, process.stdout).read()
+        output: bytes = cast(IO[bytes], process.stdout).read()
         return output.decode("utf-8")
 
     def _run_for_services(
         self,
         cmd: str,
         services: Sequence[str],
-        options: Optional[Dict[str, bool]] = None,
+        options: dict[str, bool] | None = None,
     ) -> str:
-        opts: List[str] = []
+        opts: list[str] = []
         if options:
-            opts = [f"--{option}" for option, value in options.items() if value]
+            opts = [
+                f"--{option}" for option, value in options.items() if value
+            ]
         if services:
-            service_names = [f"{self._instance_name}.{service}" for service in services]
+            service_names = [
+                f"{self._instance_name}.{service}" for service in services
+            ]
         else:
             service_names = [self._instance_name]
         return self.run(cmd, *opts, *service_names)
 
-    def _set_args(self, configs: Dict[str, Any]) -> List[str]:
+    def _set_args(self, configs: dict[str, Any]) -> list[str]:
         return [f"{key}={json.dumps(value)}" for key, value in configs.items()]
 
-    def _unset_args(self, configs: Tuple[str, ...]) -> List[str]:
+    def _unset_args(self, configs: tuple[str, ...]) -> list[str]:
         return [f"{key}!" for key in configs]
 
     def _connection_get(
         self,
         name: str,
-        keys: Tuple[str, ...],
-        remote_type: Optional[str] = None,
-    ) -> Dict[str, Any]:
+        keys: tuple[str, ...],
+        remote_type: str | None = None,
+    ) -> dict[str, Any]:
         args = ["get", "-d"]
         if remote_type:
             args.append(f"--{remote_type}")
         args.append(f":{name}")
         args.extend(keys)
-        conf: Dict[str, Any]
-        conf = json.loads(self.run(*args))
+        conf: dict[str, Any] = json.loads(self.run(*args))
         return conf
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_env.py` & `snap-helpers-0.4.0/snaphelpers/_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from collections import abc
 import os
 from typing import (
     Iterator,
     Mapping,
     Optional,
 )
 
 
 def is_snap(environ: Optional[Mapping[str, str]] = None) -> bool:
-    """Return whether running in a Snap."""
+    """Return whether running in a Snap.
+
+    :param environ: optionally, the mapping with environment variables.
+
+    """
     if environ is None:
         environ = os.environ
     return bool(environ.get("SNAP", ""))
 
 
-class SnapEnviron(abc.Mapping):
+class SnapEnviron(Mapping[str, str]):
     """Environment variables related to the Snap.
 
     This provides read-only access to environment variables starting with
     :data:`SNAP_`.
 
     These can be accessed either as a dict or as attributes, without the
     :data:`SNAP_` prefix. E.g.::
@@ -46,15 +49,15 @@
 
     def __getitem__(self, key: str) -> str:
         return self._env[key]
 
     def __len__(self) -> int:
         return len(self._env)
 
-    def __iter__(self) -> Iterator:
+    def __iter__(self) -> Iterator[str]:
         return iter(self._env)
 
     def __getattr__(self, attr: str) -> str:
         try:
             return self._env[attr]
         except KeyError as e:
             raise AttributeError(str(e))
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_health.py` & `snap-helpers-0.4.0/snaphelpers/_health.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,41 +16,43 @@
     This provides an interfaces for setting health for the snap.
 
     """
 
     def __init__(self, snapctl: Optional[SnapCtl] = None):
         self._snapctl = snapctl or SnapCtl()
 
-    def okay(self):
+    def okay(self) -> None:
         """Set the status of the snap to "okay"."""
         self._snapctl.set_health(SnapHealthStatus.OKAY)
 
-    def waiting(self, message: str, code: Optional[str] = None):
+    def waiting(self, message: str, code: Optional[str] = None) -> None:
         """Set the status of the snap to "waiting".
 
         :param message: a message string for the status
         :param code: an optional code string
         """
         self._set_health(SnapHealthStatus.WAITING, message, code)
 
-    def blocked(self, message: str, code: Optional[str] = None):
+    def blocked(self, message: str, code: Optional[str] = None) -> None:
         """Set the status of the snap to "blocked".
 
         :param message: a message string for the status
         :param code: an optional code string
         """
         self._set_health(SnapHealthStatus.BLOCKED, message, code)
 
-    def error(self, message: str, code: Optional[str] = None):
+    def error(self, message: str, code: Optional[str] = None) -> None:
         """Set the status of the snap to "error".
 
         :param message: a message string for the status
         :param code: an optional code string
         """
         self._set_health(SnapHealthStatus.ERROR, message, code)
 
-    def _set_health(self, status: SnapHealthStatus, message: str, code: Optional[str]):
+    def _set_health(
+        self, status: SnapHealthStatus, message: str, code: Optional[str]
+    ) -> None:
         if not message:
             raise ValueError("Health status message must not be empty")
         if code is not None and not STATUS_CODE_RE.match(code):
             raise ValueError("Invalid health status code format")
         self._snapctl.set_health(status, message=message, code=code)
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_hook.py` & `snap-helpers-0.4.0/snaphelpers/_hook.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import (
-    cast,
+    Callable,
     List,
     NamedTuple,
 )
 
-import pkg_resources
+from ._importlib import (
+    entry_points,
+    EntryPoint,
+    EntryPoints,
+)
 
 HOOKS_ENTRY_POINT = "snaphelpers.hooks"
 
 
 class Hook(NamedTuple):
     """A snap hook declared via ``entry_points``."""
 
@@ -16,57 +20,57 @@
     project: str
     module: str
     import_name: str
     path: str
     exists: bool
 
     @classmethod
-    def from_entry_point(cls, entry: pkg_resources.EntryPoint):
-        try:
-            entry.resolve()
-        except ImportError:
-            exists = False
-        else:
-            exists = True
+    def from_entry_point(
+        cls, entry: EntryPoint, skip_load: bool = False
+    ) -> "Hook":
+        """Return a ``Hook`` from an ``EntryPoint``."""
+        project = entry.dist.name if entry.dist else ""
+        exists = True
+        if not skip_load:
+            try:
+                entry.load()
+            except ModuleNotFoundError:
+                exists = False
         return cls(
             name=entry.name,
-            project=cast(pkg_resources.Distribution, entry.dist).project_name,
-            module=entry.module_name,
-            import_name=entry.attrs[0],
-            path=".".join(entry.attrs),
+            project=project,
+            module=entry.module,
+            import_name=entry.attr.split(".")[0],
+            path=entry.attr,
             exists=exists,
         )
 
     @property
     def location(self) -> str:
         """The hook location."""
         return f"{self.module}:{self.path}"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.location} ({self.project})"
 
 
-def get_hooks(pkg_resources=pkg_resources) -> List[Hook]:
+def get_hooks(
+    entry_points: Callable[..., EntryPoints] = entry_points
+) -> List[Hook]:
     """Return registered snap hooks.
 
-    Resources registred as ``snaphelpers.hooks`` in ``entry_points`` are loaded
+    Resources registred as ``snaphelpers.hooks`` in ``entry-points`` are loaded
     as hooks, based on their name.
 
-    For example:
+    For example, in ``pyproject.toml``:
 
-    .. code:: python
+    .. code:: toml
 
-       setup(
-           # ...
-           entry_points={
-               "snaphelpers.hooks"': [
-                   "install = foo.bar:install_hook",
-                   "configure = foo.bar:configure_hook",
-               ]
-           }
-       )
+       [project.entry-points."snaphelpers.hooks"]
+       configure = "foo.bar:configure_hook"
+       install = "foo.bar:install_hook"
 
     """
     return [
         Hook.from_entry_point(entry_point)
-        for entry_point in pkg_resources.iter_entry_points(HOOKS_ENTRY_POINT)
+        for entry_point in entry_points(group=HOOKS_ENTRY_POINT)
     ]
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_meta.py` & `snap-helpers-0.4.0/snaphelpers/_meta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-from collections.abc import Mapping
 from pathlib import Path
 from typing import (
     Any,
     Dict,
+    Iterator,
+    Mapping,
     Optional,
 )
 
 import yaml
 
 from ._env import SnapEnviron
 
 
-class SnapMetadataFile(Mapping):
+class SnapMetadataFile(Mapping[str, Any]):
     """A YAML metadata file from the snap.
 
-    The content is read at the first access, and is accessible as a normal
+    The content is read at the first access, and is accessible as a regular
     dict.
 
     """
 
+    path: Path  #: the file Path
+
     def __init__(self, path: Path):
         self.path = path
         self._loaded = False
         self._data: Dict[str, Any] = {}
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.path)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.path})"
 
-    def __getitem__(self, item: str):
+    def __getitem__(self, item: str) -> Any:
         self._ensure_loaded()
         return self._data[item]
 
-    def __len__(self):
+    def __len__(self) -> int:
         self._ensure_loaded()
         return len(self._data)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         self._ensure_loaded()
         return iter(self._data)
 
     def exists(self) -> bool:
         """Return whether the file exists."""
         return self.path.exists()
 
-    def _ensure_loaded(self):
+    def _ensure_loaded(self) -> None:
         if self._loaded:
             return
 
         with self.path.open() as fd:
             self._data = yaml.safe_load(fd)
 
         self._loaded = True
@@ -58,15 +61,17 @@
 
 class MetadataFileProperty:
     """Wrapper to get :class:`SnapMetadataFile` instances for files."""
 
     def __init__(self, local_path: str):
         self.local_path = local_path
 
-    def __get__(self, instance, owner) -> SnapMetadataFile:
+    def __get__(
+        self, instance: "SnapMetadataFiles", owner: type
+    ) -> SnapMetadataFile:
         path = Path(instance._environ["SNAP"]) / self.local_path
         return SnapMetadataFile(path)
 
 
 class SnapMetadataFiles:
     """Metadata files for a snap.
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_path.py` & `snap-helpers-0.4.0/snaphelpers/_path.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,26 +3,35 @@
 
 from ._env import SnapEnviron
 
 
 class SnapPaths:
     """Paths related to the snap."""
 
-    __slots__ = ("common", "data", "real_home", "snap", "user_common", "user_data")
+    __slots__ = (
+        "common",
+        "data",
+        "real_home",
+        "snap",
+        "user_common",
+        "user_data",
+    )
 
     common: Path  #: the SNAP_COMMON path
     data: Path  #: the SNAP_DATA path
     real_home: Path  #: the SNAP_REAL_HOME path
     snap: Path  #: the SNAP path
     user_common: Path  #: the SNAP_USER_COMMON path
     user_data: Path  #: the SNAP_USER_DATA path
 
     def __init__(self, env: Optional[SnapEnviron] = None):
         if env is None:
             env = SnapEnviron()
         for key in self.__slots__:
             setattr(self, key, Path(env[key.upper()]))
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         name = self.__class__.__name__
-        values = " ".join(f"{key}={str(getattr(self, key))}" for key in self.__slots__)
+        values = " ".join(
+            f"{key}={str(getattr(self, key))}" for key in self.__slots__
+        )
         return f"{name}({values})"
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_service.py` & `snap-helpers-0.4.0/snaphelpers/_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import (
+    Any,
     Dict,
     Optional,
 )
 
 from ._ctl import (
     ServiceInfo,
     SnapCtl,
@@ -12,49 +13,51 @@
 class SnapService:
     """A service defined in the Snap."""
 
     def __init__(self, info: ServiceInfo, snapctl: Optional[SnapCtl] = None):
         self._info = info
         self._snapctl = snapctl or SnapCtl()
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         # forward attributes defined in ServiceInfo
         return getattr(self._info, attr)
 
-    def __eq__(self, other) -> bool:
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, SnapService):
+            return NotImplemented
         return self._info == other._info and self._snapctl is other._snapctl
 
-    def start(self, enable: bool = False):
+    def start(self, enable: bool = False) -> None:
         """Start the service.
 
         :param enable: whether to also enable the service at startup.
 
         """
         self._snapctl.start(self.name, enable=enable)
         self.refresh_status()
 
-    def stop(self, disable: bool = False):
+    def stop(self, disable: bool = False) -> None:
         """Stop the service.
 
         :param disable: whether to also disable the service at startup.
 
         """
         self._snapctl.stop(self.name, disable=disable)
         self.refresh_status()
 
-    def restart(self, reload: bool = False):
+    def restart(self, reload: bool = False) -> None:
         """Restart the service.
 
         :param reload: whether to reload the service if supported.
 
         """
         self._snapctl.restart(self.name, reload=reload)
         self.refresh_status()
 
-    def refresh_status(self):
+    def refresh_status(self) -> None:
         """Update the status of the ervice service."""
         [self._info] = self._snapctl.services(self.name)
 
 
 class SnapServices:
     """Manage services in the snap."""
 
@@ -64,30 +67,30 @@
     def list(self) -> Dict[str, SnapService]:
         """Return services by name."""
         return {
             info.name: SnapService(info, snapctl=self._snapctl)
             for info in self._snapctl.services()
         }
 
-    def start(self, enable: bool = False):
+    def start(self, enable: bool = False) -> None:
         """Start all services.
 
         :param enable: whether to also enable services at startup.
 
         """
         self._snapctl.start(enable=enable)
 
-    def stop(self, disable: bool = False):
+    def stop(self, disable: bool = False) -> None:
         """Stop all services.
 
         :param disable: whether to also disable services at startup.
 
         """
         self._snapctl.stop(disable=disable)
 
-    def restart(self, reload: bool = False):
+    def restart(self, reload: bool = False) -> None:
         """Restart all services.
 
         :param reload: whether to reload services if supported.
 
         """
         self._snapctl.restart(reload=reload)
```

### Comparing `snap-helpers-0.3.2/snaphelpers/_snap.py` & `snap-helpers-0.4.0/snaphelpers/_snap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from typing import (
+    Any,
+    cast,
     Mapping,
     Optional,
 )
 
 from ._conf import SnapConfig
 from ._ctl import SnapCtl
 from ._env import SnapEnviron
@@ -14,39 +16,51 @@
 
 class EnvironProperty:
     """Wrapper to get properties from a :class:`SnapEnviron` instance."""
 
     def __init__(self, name: str):
         self.name = name
 
-    def __get__(self, instance, owner):
-        return getattr(instance.environ, self.name)
+    def __get__(self, instance: "Snap", owner: Any) -> str:
+        return cast(str, getattr(instance.environ, self.name))
 
 
 class Snap:
     """Top-level wrapper for a Snap."""
 
+    #: Access to snap configuration
     config: SnapConfig
+    #: Access to snap environment variables
     environ: SnapEnviron
+    #: Access to snap health status
     health: SnapHealth
+    #: Access to snap-specific paths
     paths: SnapPaths
+    #: Access to snap services
     services: SnapServices
+    #: Access to snap metadata files
     metadata_files: SnapMetadataFiles
 
+    #: The snap name
     name = EnvironProperty("NAME")
+    #: The snap instance name (usually same as the ``name``, unless parallel
+    # installs are used)
     instance_name = EnvironProperty("INSTANCE_NAME")
+    #: The snap version
     version = EnvironProperty("VERSION")
+    #: The snap revision
     revision = EnvironProperty("REVISION")
 
     def __init__(self, environ: Optional[Mapping[str, str]] = None):
         self.environ = SnapEnviron(environ=environ)
         self.paths = SnapPaths(env=self.environ)
         snapctl = SnapCtl(env=self.environ)
         self.config = SnapConfig(snapctl=snapctl)
         self.health = SnapHealth(snapctl=snapctl)
         self.services = SnapServices(snapctl=snapctl)
         self.metadata_files = SnapMetadataFiles(environ=self.environ)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
-            f"{self.__class__.__name__}" f"({self.name} {self.version} {self.revision})"
+            f"{self.__class__.__name__}"
+            f"({self.name} {self.version} {self.revision})"
         )
```

### Comparing `snap-helpers-0.3.2/snaphelpers/scripts/_script.py` & `snap-helpers-0.4.0/snaphelpers/scripts/_script.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,35 +21,37 @@
         super().__init__(message)
         self.code = code
 
 
 class Script(ABC):
     """A Script."""
 
-    def __init__(self, stdout: IO = sys.stdout, stderr: IO = sys.stderr):
+    def __init__(
+        self, stdout: IO[str] = sys.stdout, stderr: IO[str] = sys.stderr
+    ):
         self.stdout = stdout
         self.stderr = stderr
 
     @abstractmethod
     def get_parser(self) -> ArgumentParser:
         """Return a parser for the script.
 
         Subclasses must implement this method.
 
         """
 
     @abstractmethod
-    def run(self, options: Namespace) -> Optional[int]:
+    def run(self, options: Namespace) -> int:
         """Run the script
 
         Subclasses must implement this method.
 
         """
 
-    def __call__(self, args: Optional[List[str]] = None) -> Optional[int]:
+    def __call__(self, args: Optional[List[str]] = None) -> int:
         parser = self.get_parser()
         opts = parser.parse_args(args=args)
         try:
             return self.run(opts)
         except ScriptError as error:
             self.print(str(error), err=True)
             return error.code
```

### Comparing `snap-helpers-0.3.2/snaphelpers/scripts/snaphelpers.py` & `snap-helpers-0.4.0/snaphelpers/scripts/snap_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 )
 from collections import defaultdict
 from operator import attrgetter
 import os
 from pathlib import Path
 from textwrap import dedent
 from typing import (
+    Callable,
     Dict,
     List,
 )
 
 from .._hook import (
     get_hooks,
     Hook,
@@ -42,79 +43,94 @@
             from snaphelpers import Snap
             from {self.hook.module} import {self.hook.import_name}
 
             sys.exit({self.hook.path}(Snap()))
             """
         )
 
-    def write(self, hooks_dir: Path):
+    def write(self, hooks_dir: Path) -> None:
         """Write the hook script in the specified directory."""
         path = hooks_dir / self.hook.name
         path.write_text(self.render())
         path.chmod(0o755)
 
 
 class SnapHelpersScript(Script):
     """Tool to perform snap-helpers tasks."""
 
     def get_parser(self) -> ArgumentParser:
-        parser = ArgumentParser(description="Tool to perform snap-helpers tasks")
+        parser = ArgumentParser(
+            description="Tool to perform snap-helpers tasks"
+        )
         subparsers = parser.add_subparsers(
             metavar="ACTION", dest="action", help="action to perform"
         )
         subparsers.required = True
 
         write_hooks = subparsers.add_parser(
             "write-hooks",
             help="Write hook files",
             formatter_class=ArgumentDefaultsHelpFormatter,
         )
         write_hooks.add_argument(
-            "--prime-dir", help="snap prime directory (default from snacraft env var)"
+            "--prime-dir",
+            help="snap prime directory (default from snacraft env var)",
+        )
+        write_hooks.add_argument(
+            "--fail-empty",
+            help="fail if no hook is found.",
+            action="store_true",
         )
         return parser
 
-    def run(self, options: Namespace):
-        action = options.action.replace("-", "_")
-        getattr(self, f"_action_{action}")(options)
+    def run(self, options: Namespace) -> int:
+        action_name = options.action.replace("-", "_")
+        action: Callable[[Namespace], int] = getattr(
+            self, f"_action_{action_name}"
+        )
+        return action(options)
 
-    def _action_write_hooks(self, options: Namespace):
+    def _action_write_hooks(self, options: Namespace) -> int:
         if options.prime_dir:
             prime_dir = Path(options.prime_dir)
         else:
-            prime_dir = self._ensure_env_path("CRAFT_PRIME", fallback="SNAPCRAFT_PRIME")
+            prime_dir = self._ensure_env_path(
+                "CRAFT_PRIME", fallback="SNAPCRAFT_PRIME"
+            )
 
         hooks = sorted(get_hooks(), key=attrgetter("name"))
         self._validate_hooks(hooks)
         if not hooks:
             self.print(
                 "No hooks defined in the snap.\n"
                 f'Hooks must be defined in the "{HOOKS_ENTRY_POINT}" '
                 "section of entry points."
             )
-            return
+            return 1 if options.fail_empty else 0
 
         hooks_dir = prime_dir / "snap" / "hooks"
         hooks_dir.mkdir(parents=True, exist_ok=True)
 
         self.print(f"Writing hook files to {hooks_dir.absolute()}")
         for hook in hooks:
             hook_script = HookScript(hook)
             self.print(f" {hook.name}: {hook}")
             hook_script.write(hooks_dir)
 
+        return 0
+
     def _ensure_env_path(self, name: str, fallback: str = "") -> Path:
         value = os.environ.get(name)
         if value is None and fallback:
             value = os.environ.get(fallback)
         if value is None:
             raise ScriptError(f"{name} environment variable not defined")
         return Path(value)
 
-    def _validate_hooks(self, hooks: List[Hook]):
+    def _validate_hooks(self, hooks: List[Hook]) -> None:
         hooks_by_name: Dict[str, List[Hook]] = defaultdict(list)
         not_found_hooks = []
         for hook in hooks:
             if not hook.exists:
                 not_found_hooks.append(hook)
             hooks_by_name[hook.name].append(hook)
 
@@ -122,15 +138,17 @@
         duplicated = sorted(
             name for name, hooks in hooks_by_name.items() if len(hooks) > 1
         )
         if duplicated:
             message = ["Multiple definitions found for hook(s):"]
             for name in duplicated:
                 message.append(f"- {name}")
-                message.extend(f"    {hook}" for hook in sorted(hooks_by_name[name]))
+                message.extend(
+                    f"    {hook}" for hook in sorted(hooks_by_name[name])
+                )
             raise ScriptError("\n".join(message))
 
         # check that they exist
         if not_found_hooks:
             message = ["Hook function(s) not found:"]
             for hook in not_found_hooks:
                 message.append(f"- {hook}")
```

