# Comparing `tmp/winbundle-0.1.0.post1.tar.gz` & `tmp/winbundle-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winbundle-0.1.0.post1.tar", last modified: Sat Jul 15 20:56:31 2023, max compression
+gzip compressed data, was "winbundle-0.1.1.tar", last modified: Sun Jul 16 17:14:27 2023, max compression
```

## Comparing `winbundle-0.1.0.post1.tar` & `winbundle-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 20:56:31.386338 winbundle-0.1.0.post1/
--rw-rw-rw-   0        0        0     1095 2023-07-15 14:51:52.000000 winbundle-0.1.0.post1/LICENSE
--rw-rw-rw-   0        0        0      415 2023-07-15 20:56:31.385338 winbundle-0.1.0.post1/PKG-INFO
--rw-rw-rw-   0        0        0      154 2023-07-15 20:50:38.000000 winbundle-0.1.0.post1/README.md
--rw-rw-rw-   0        0        0      412 2023-07-15 20:55:53.000000 winbundle-0.1.0.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 20:56:31.386338 winbundle-0.1.0.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 20:56:31.367338 winbundle-0.1.0.post1/winbundle/
--rw-rw-rw-   0        0        0       74 2023-07-15 20:39:31.000000 winbundle-0.1.0.post1/winbundle/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-07-15 20:39:31.000000 winbundle-0.1.0.post1/winbundle/__main__.py
--rw-rw-rw-   0        0        0    10720 2023-07-15 20:40:10.000000 winbundle-0.1.0.post1/winbundle/builder.py
--rw-rw-rw-   0        0        0     3278 2023-07-15 20:39:31.000000 winbundle-0.1.0.post1/winbundle/newconfig.py
--rw-rw-rw-   0        0        0      913 2023-07-15 13:24:35.000000 winbundle-0.1.0.post1/winbundle/util.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:56:31.384340 winbundle-0.1.0.post1/winbundle.egg-info/
--rw-rw-rw-   0        0        0      415 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 17:14:27.932824 winbundle-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2023-07-15 14:51:52.000000 winbundle-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      470 2023-07-16 17:14:27.932324 winbundle-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-07-15 20:50:38.000000 winbundle-0.1.1/README.md
+-rw-rw-rw-   0        0        0      558 2023-07-16 17:08:26.000000 winbundle-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 17:14:27.932824 winbundle-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-16 17:14:27.912326 winbundle-0.1.1/winbundle/
+-rw-rw-rw-   0        0        0       73 2023-07-16 17:05:41.000000 winbundle-0.1.1/winbundle/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-07-15 20:39:31.000000 winbundle-0.1.1/winbundle/__main__.py
+-rw-rw-rw-   0        0        0     9822 2023-07-16 15:26:55.000000 winbundle-0.1.1/winbundle/builder.py
+-rw-rw-rw-   0        0        0     2031 2023-07-16 15:29:59.000000 winbundle-0.1.1/winbundle/icon.py
+-rw-rw-rw-   0        0        0     3278 2023-07-15 20:39:31.000000 winbundle-0.1.1/winbundle/newconfig.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 13:24:35.000000 winbundle-0.1.1/winbundle/util.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:14:27.930824 winbundle-0.1.1/winbundle.egg-info/
+-rw-rw-rw-   0        0        0      470 2023-07-16 17:14:27.000000 winbundle-0.1.1/winbundle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-16 17:14:27.000000 winbundle-0.1.1/winbundle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:14:27.000000 winbundle-0.1.1/winbundle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-16 17:14:27.000000 winbundle-0.1.1/winbundle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 17:14:27.000000 winbundle-0.1.1/winbundle.egg-info/top_level.txt
```

### Comparing `winbundle-0.1.0.post1/LICENSE` & `winbundle-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0.post1/winbundle/__main__.py` & `winbundle-0.1.1/winbundle/__main__.py`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0.post1/winbundle/builder.py` & `winbundle-0.1.1/winbundle/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import urllib.parse
 import urllib.request
 import zipfile
 
 import distlib.scripts
 
 import winbundle.util
+import winbundle.icon
 
 
 def _get_launcher(self, kind):
     # Needed to override the internals to allow control over arch
     if self._machine == 'amd64':
         bits = '64'
     else:
@@ -59,15 +60,14 @@
         self._output_path = self._build_path / self.name
         self._final_path = self.root / 'dist' / (
             f"{self.name}{'' if self.version is None else '-' + self.version}"
             f"-py{self.py_version}-{self.machine}"
         )
         self.dependencies = [] if dependencies is None else dependencies
         self.files = files
-        self._rh_path = self._cache_path / 'resourcehacker'
         self._wix_path = self._cache_path / 'wix'
 
     @classmethod
     def from_path(cls, path):
         path = pathlib.Path(path).resolve()
         if path.is_dir():
             path = (path / 'pyproject.toml').resolve()
@@ -115,26 +115,18 @@
     def _download_python_installer(self):
         url = (
             f"https://www.python.org/ftp/python/{self.py_version}/python-{self.py_version}"
             f"{'-' + self.machine if self.machine != 'win32' else ''}.exe"
         )
         return self._download_item(url)
 
-    def _download_resource_hacker(self):
-        url = "http://www.angusj.com/resourcehacker/resource_hacker.zip"
-        return self._download_item(url)
-
     def _extract_wix(self, path):
         with zipfile.ZipFile(path) as zf:
             zf.extractall(self._wix_path)
 
-    def _extract_resource_hacker(self, path):
-        with zipfile.ZipFile(path) as zf:
-            zf.extractall(self._rh_path)
-
     def _extract_python(self, path):
         if not self._output_path.exists():
             self._output_path.mkdir(exist_ok=True, parents=True)
             with zipfile.ZipFile(path) as zf:
                 zf.extractall(self._output_path)
 
     def _copy_source(self):
@@ -180,29 +172,18 @@
         shutil.copytree((tcltk_build / 'Lib' / 'tkinter'), (self._output_path / 'tkinter'))
         shutil.copytree((tcltk_build / 'Lib' / 'idlelib'), (self._output_path / 'idlelib'))
         shutil.copytree((tcltk_build / 'tcl'), (self._output_path / 'tcl'))
 
     def _add_icon(self, exes, icon):
         if not icon:
             return
-        if not self._rh_path.is_dir():
-            rh = self._download_resource_hacker()
-            self._extract_resource_hacker(rh)
-            self._has_rh = True
         icon = self.root / icon
         exes = [pathlib.Path(x).resolve() for x in exes]
         for exe in exes:
-            subprocess.run([
-                str(self._rh_path / 'ResourceHacker.exe'), '-open', str(exe), '-save', str(exe), '-action',
-                'delete', '-mask', 'ICONGROUP,101,'
-            ])
-            subprocess.run([
-                str(self._rh_path / 'ResourceHacker.exe'), '-open', str(exe), '-save', str(exe), '-action',
-                'addoverwrite', '-res', str(icon), '-mask', 'ICONGROUP,MAINICON,'
-            ])
+            winbundle.icon.apply_icon(exe, icon)
 
     def _install_dependencies(self):
         args = [sys.executable, '-m', 'pip', 'install', '--target', str(self._output_path)]
         only_bin = False
         if self.machine != winbundle.util.this_machine()[0]:
             only_bin = True
             arch = 'win-amd64' if self.machine == 'amd64' else 'win32'
```

### Comparing `winbundle-0.1.0.post1/winbundle/newconfig.py` & `winbundle-0.1.1/winbundle/newconfig.py`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0.post1/winbundle/util.py` & `winbundle-0.1.1/winbundle/util.py`

 * *Files identical despite different names*

