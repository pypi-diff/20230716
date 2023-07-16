# Comparing `tmp/idlerich-0.1.0.tar.gz` & `tmp/idlerich-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idlerich-0.1.0.tar", last modified: Sun Jul 16 20:23:53 2023, max compression
+gzip compressed data, was "idlerich-0.2.0.tar", last modified: Sun Jul 16 21:01:36 2023, max compression
```

## Comparing `idlerich-0.1.0.tar` & `idlerich-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 20:23:53.592244 idlerich-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-07-16 16:33:58.000000 idlerich-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      722 2023-07-16 20:23:53.592244 idlerich-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      362 2023-07-16 18:49:46.000000 idlerich-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 20:23:53.505298 idlerich-0.1.0/idlerich/
--rw-rw-rw-   0        0        0       50 2023-07-16 17:28:09.000000 idlerich-0.1.0/idlerich/__init__.py
--rw-rw-rw-   0        0        0     2943 2023-07-16 20:02:25.000000 idlerich-0.1.0/idlerich/idlerich.py
--rw-rw-rw-   0        0        0      151 2023-07-16 17:11:40.000000 idlerich-0.1.0/idlerich/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-16 20:23:53.589247 idlerich-0.1.0/idlerich.egg-info/
--rw-rw-rw-   0        0        0      722 2023-07-16 20:23:53.000000 idlerich-0.1.0/idlerich.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-16 20:23:53.000000 idlerich-0.1.0/idlerich.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 20:23:53.000000 idlerich-0.1.0/idlerich.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-16 20:23:53.000000 idlerich-0.1.0/idlerich.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-07-16 20:23:53.000000 idlerich-0.1.0/idlerich.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 20:23:53.000000 idlerich-0.1.0/idlerich.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 20:23:53.593245 idlerich-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-07-16 18:10:47.000000 idlerich-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:01:36.944076 idlerich-0.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-07-16 16:33:58.000000 idlerich-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      796 2023-07-16 21:01:36.943076 idlerich-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-07-16 20:59:39.000000 idlerich-0.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 21:01:36.898101 idlerich-0.2.0/idlerich/
+-rw-rw-rw-   0        0        0       13 2023-07-16 20:54:31.000000 idlerich-0.2.0/idlerich/__init__.py
+-rw-rw-rw-   0        0        0     3364 2023-07-16 20:57:15.000000 idlerich-0.2.0/idlerich/__main__.py
+-rw-rw-rw-   0        0        0      151 2023-07-16 21:00:41.000000 idlerich-0.2.0/idlerich/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-16 21:01:36.940080 idlerich-0.2.0/idlerich.egg-info/
+-rw-rw-rw-   0        0        0      796 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 21:01:36.000000 idlerich-0.2.0/idlerich.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 21:01:36.945073 idlerich-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      796 2023-07-16 20:52:35.000000 idlerich-0.2.0/setup.py
```

### Comparing `idlerich-0.1.0/LICENSE` & `idlerich-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idlerich-0.1.0/PKG-INFO` & `idlerich-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlerich
-Version: 0.1.0
+Version: 0.2.0
 Summary: A bootloader that caches and auto-richifies IDLE because I felt lazy.
 Home-page: https://github.com/CuboidRaptor/idlerich
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -16,8 +16,9 @@
 
 This just literally bootloads IDLE with Rich in it.
 I'm so creative.
 
 WARNING: This package is *extremely* hacky. Do not use it for any sort of stable use.
 -------------------------------------------------------------------------------------
 
-If you still want to, :code:`pip install` and run :code:`idlerich` in console.
+If you still want to, :code:`pip install` and run :code:`python -m idlerich` in console.
+Then, you can just run :code:`idle.pyw` in the idlelib folder.
```

### Comparing `idlerich-0.1.0/idlerich/idlerich.py` & `idlerich-0.2.0/idlerich/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,22 @@
         pyshellcode = f.read()
 
     pyshellcode = pyshellcode.replace("def begin(self", """\
 # New patch wrapper from Idlerich for IDLE
     def begin(self, *args, **kwargs):
         retval = self.begin_idle(*args, **kwargs)
         self.write("Python-Rich in namespace.")
-        self.interp.runcode("import rich.pretty, rich.traceback; rich.pretty.install(); rich.traceback.install(show_locals=False)")
+        self.interp.runcode(\"\"\"\
+import pkgutil
+module_name = "rich"
+for loader, module_name, is_pkg in pkgutil.walk_packages(__path__):
+    _module = loader.find_module(module_name).load_module(module_name)
+    globals()[module_name] = _module
+rich.pretty.install()
+rich.traceback.install(show_locals=False)\"\"\")
         return retval
 
     # Original begin() from IDLE
     def begin_idle(self""")
 
     with open(f"{fdir}/idlelib/pyshell.py", "w") as f:
         f.write(pyshellcode)
@@ -48,14 +55,15 @@
 
             with open(f"{fdir}/idlelib/{file}", "w") as f:
                 f.write(f"# Idlerich patch for imports\nimport sys, os\nsys.path.insert(0, os.path.abspath(os.path.dirname(os.path.abspath(__file__)) + \"/..\"))\n\n" + script)
 
 def main():
     global idlepath, fdir, pyver
 
+    print("Idlerich Patcher started!")
     print(f"Idlepath: {idlepath}")
     print(f"Current file dir of pkg: {fdir}")
     print(f"Currrent py ver: {pyver}")
 
     try:
         with open(f"{fdir}/idlelib/ir_version.txt", "r") as f:
             ir_version = int(f.read())
@@ -71,22 +79,26 @@
     pywpath = list(os.path.split(os.path.abspath(sys.executable)))
     pywpath[~0] = pywpath[~0].split(".")
     pywpath[~0][0] += "w"
     pywpath[~0] = ".".join(pywpath[~0])
     pywpath = "/".join(pywpath)
     print(f"Pythonw path: {pywpath}")
 
-    subprocess.Popen(f"{pywpath} \"{fdir}/idlelib/idle.pyw\"")
+    print("To run Idlerich, run pythonw on idle.pyw in idlelib in your site-packages folder, at python.")
+    print(f"Your pythonw path is {pywpath}, and your idle script path is {fdir}/idlelib/idle.pyw .")
 
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     # idfk y u would pyinstaller idle but ok
     sys.stderr.write("WARNING: Idlerich may not run properly in a PyInstaller environment.\n")
 else:
     pass
 
 if not str(sys.version).startswith("3"):
     # python 2 is literally a joke from the gods
     sys.stderr.write("WARNING: Idlerich may not run properly without Python 3.\n")
 
 idlepath = os.path.dirname(sys.executable) + "/Lib/idlelib"
 fdir = os.path.dirname(__file__)
 pyver = sys.hexversion
+
+if __name__ == "__main__":
+    main()
```

### Comparing `idlerich-0.1.0/idlerich.egg-info/PKG-INFO` & `idlerich-0.2.0/idlerich.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlerich
-Version: 0.1.0
+Version: 0.2.0
 Summary: A bootloader that caches and auto-richifies IDLE because I felt lazy.
 Home-page: https://github.com/CuboidRaptor/idlerich
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -16,8 +16,9 @@
 
 This just literally bootloads IDLE with Rich in it.
 I'm so creative.
 
 WARNING: This package is *extremely* hacky. Do not use it for any sort of stable use.
 -------------------------------------------------------------------------------------
 
-If you still want to, :code:`pip install` and run :code:`idlerich` in console.
+If you still want to, :code:`pip install` and run :code:`python -m idlerich` in console.
+Then, you can just run :code:`idle.pyw` in the idlelib folder.
```

### Comparing `idlerich-0.1.0/setup.py` & `idlerich-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,9 @@
     license="MIT License",
     packages=["idlerich"],
     install_requires=[
         "rich>=13.0.0a1"
     ],
     python_requires=">=3.6",
     long_description=readme,
-    long_description_content_type="text/x-rst",
-    entry_points = {
-        "console_scripts": ["idlerich=idlerich:main"]
-    }
+    long_description_content_type="text/x-rst"
 )
```

