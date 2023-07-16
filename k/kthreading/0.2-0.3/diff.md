# Comparing `tmp/kthreading-0.2.tar.gz` & `tmp/kthreading-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthreading-0.2.tar", last modified: Sun Jul 16 05:36:47 2023, max compression
+gzip compressed data, was "kthreading-0.3.tar", last modified: Sun Jul 16 16:08:44 2023, max compression
```

## Comparing `kthreading-0.2.tar` & `kthreading-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 05:36:47.163765 kthreading-0.2/
--rw-rw-rw-   0        0        0     1093 2023-07-16 05:11:51.000000 kthreading-0.2/LICENSE.md
--rw-rw-rw-   0        0        0     1166 2023-07-16 05:36:47.162767 kthreading-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      874 2023-07-16 05:24:18.000000 kthreading-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 05:36:47.137471 kthreading-0.2/kthreading/
--rw-rw-rw-   0        0        0      349 2023-07-12 09:40:43.000000 kthreading-0.2/kthreading/__init__.py
--rw-rw-rw-   0        0        0     1753 2023-07-15 13:47:57.000000 kthreading-0.2/kthreading/classes.py
--rw-rw-rw-   0        0        0      388 2023-07-12 09:40:43.000000 kthreading-0.2/kthreading/exceptions.py
--rw-rw-rw-   0        0        0      213 2023-07-12 01:41:50.000000 kthreading-0.2/kthreading/functions.py
--rw-rw-rw-   0        0        0     2843 2023-07-15 15:05:34.000000 kthreading-0.2/kthreading/kthread.py
--rw-rw-rw-   0        0        0      626 2023-07-12 09:40:44.000000 kthreading-0.2/kthreading/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-16 05:36:47.161762 kthreading-0.2/kthreading.egg-info/
--rw-rw-rw-   0        0        0     1166 2023-07-16 05:36:46.000000 kthreading-0.2/kthreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-07-16 05:36:47.000000 kthreading-0.2/kthreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 05:36:47.000000 kthreading-0.2/kthreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-16 05:36:47.000000 kthreading-0.2/kthreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 05:36:47.163765 kthreading-0.2/setup.cfg
--rw-rw-rw-   0        0        0      610 2023-07-16 05:32:07.000000 kthreading-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:08:44.737407 kthreading-0.3/
+-rw-rw-rw-   0        0        0     1093 2023-07-16 05:11:51.000000 kthreading-0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     1327 2023-07-16 16:08:44.736406 kthreading-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1035 2023-07-16 16:02:58.000000 kthreading-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 16:08:44.714135 kthreading-0.3/kthreading/
+-rw-rw-rw-   0        0        0      349 2023-07-12 09:40:43.000000 kthreading-0.3/kthreading/__init__.py
+-rw-rw-rw-   0        0        0     1753 2023-07-15 13:47:57.000000 kthreading-0.3/kthreading/classes.py
+-rw-rw-rw-   0        0        0      388 2023-07-12 09:40:43.000000 kthreading-0.3/kthreading/exceptions.py
+-rw-rw-rw-   0        0        0      276 2023-07-16 16:01:57.000000 kthreading-0.3/kthreading/functions.py
+-rw-rw-rw-   0        0        0     3200 2023-07-16 16:02:04.000000 kthreading-0.3/kthreading/kthread.py
+-rw-rw-rw-   0        0        0      626 2023-07-12 09:40:44.000000 kthreading-0.3/kthreading/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:08:44.734909 kthreading-0.3/kthreading.egg-info/
+-rw-rw-rw-   0        0        0     1327 2023-07-16 16:08:44.000000 kthreading-0.3/kthreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-16 16:08:44.000000 kthreading-0.3/kthreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 16:08:44.000000 kthreading-0.3/kthreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 16:08:44.000000 kthreading-0.3/kthreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 16:08:44.737407 kthreading-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-07-16 16:08:42.000000 kthreading-0.3/setup.py
```

### Comparing `kthreading-0.2/LICENSE.md` & `kthreading-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kthreading-0.2/PKG-INFO` & `kthreading-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthreading
-Version: 0.2
+Version: 0.3
 Summary: Get more controls over threads
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -12,8 +12,12 @@
 ### KThreading is a Python library that provides advanced functionality for interacting with threads.
 # Features
 1. Forced thread termination: The library allows you to forcibly terminate threads.
 2. Timed execution of functions: KThreading enables you to launch functions with a specified timeout.
 3. Retrieval of function results: The library provides the capability to retrieve the results of functions running in separate threads.
 4. Quick thread launch: KThreading offers a simple and convenient interface for launching threads with a single line of code.
 5. Usage of functions as error handlers: The library allows for the usage of functions as error handlers, which will be called in case of exceptions occurring in a thread.
-### Read docs at [this webpage](https://its-matrix.gitbook.io/kthreading/, "Open docs").
+# Whats new in 0.3
+- Add "ident" property to KThread class
+- Set default "daemon" attribute value to "False"
+- Add "daemon" param to "start_kthread" function
+### Read docs at [this webpage](https://its-matrix.gitbook.io/kthreading/ "Open docs").
```

### Comparing `kthreading-0.2/README.md` & `kthreading-0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,8 +2,12 @@
 ### KThreading is a Python library that provides advanced functionality for interacting with threads.
 # Features
 1. Forced thread termination: The library allows you to forcibly terminate threads.
 2. Timed execution of functions: KThreading enables you to launch functions with a specified timeout.
 3. Retrieval of function results: The library provides the capability to retrieve the results of functions running in separate threads.
 4. Quick thread launch: KThreading offers a simple and convenient interface for launching threads with a single line of code.
 5. Usage of functions as error handlers: The library allows for the usage of functions as error handlers, which will be called in case of exceptions occurring in a thread.
-### Read docs at [this webpage](https://its-matrix.gitbook.io/kthreading/, "Open docs").
+# Whats new in 0.3
+- Add "ident" property to KThread class
+- Set default "daemon" attribute value to "False"
+- Add "daemon" param to "start_kthread" function
+### Read docs at [this webpage](https://its-matrix.gitbook.io/kthreading/ "Open docs").
```

### Comparing `kthreading-0.2/kthreading/classes.py` & `kthreading-0.3/kthreading/classes.py`

 * *Files identical despite different names*

### Comparing `kthreading-0.2/kthreading/kthread.py` & `kthreading-0.3/kthreading/kthread.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class KThread:
     def __init__(
         self,
         target: Callable,
         name: str = None,
-        daemon: bool = True,
+        daemon: bool = False,
         on_error: Callable | None = None,
     ) -> None:
         self.__target: Callable = target
         self.__thread: ResultThread | None = None
         self.__errhnd: Callable | None = on_error
 
         self.daemon: bool = daemon
@@ -81,14 +81,26 @@
     @property
     def status(self) -> KThreadExecutionStatus | None:
         return self.__thread.status if isinstance(self.__thread, ResultThread) else None
 
     @status.setter
     def status(self, _) -> None:
         raise TypeError("Cannot modify the `status` property. It is read-only.")
+    
+    @property
+    def ident(self) -> int:
+        if self.alive:
+            return self.__thread.ident
+        
+        else:
+            raise KThreadNotAlive("Cannot get not running thread ident")
+        
+    @ident.setter
+    def ident(self, _) -> None:
+        raise TypeError("Cannot modify the `ident` property. It is read-only.")
 
     def __repr__(self) -> str:
         status = "started" if self.alive else "stopped"
 
         if self.daemon:
             status += " daemon"
```

### Comparing `kthreading-0.2/kthreading/utils.py` & `kthreading-0.3/kthreading/utils.py`

 * *Files identical despite different names*

### Comparing `kthreading-0.2/kthreading.egg-info/PKG-INFO` & `kthreading-0.3/kthreading.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthreading
-Version: 0.2
+Version: 0.3
 Summary: Get more controls over threads
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -12,8 +12,12 @@
 ### KThreading is a Python library that provides advanced functionality for interacting with threads.
 # Features
 1. Forced thread termination: The library allows you to forcibly terminate threads.
 2. Timed execution of functions: KThreading enables you to launch functions with a specified timeout.
 3. Retrieval of function results: The library provides the capability to retrieve the results of functions running in separate threads.
 4. Quick thread launch: KThreading offers a simple and convenient interface for launching threads with a single line of code.
 5. Usage of functions as error handlers: The library allows for the usage of functions as error handlers, which will be called in case of exceptions occurring in a thread.
-### Read docs at [this webpage](https://its-matrix.gitbook.io/kthreading/, "Open docs").
+# Whats new in 0.3
+- Add "ident" property to KThread class
+- Set default "daemon" attribute value to "False"
+- Add "daemon" param to "start_kthread" function
+### Read docs at [this webpage](https://its-matrix.gitbook.io/kthreading/ "Open docs").
```

### Comparing `kthreading-0.2/setup.py` & `kthreading-0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,18 @@
     readme_contents = file.read()
 
 with open("LICENSE.md", "r", encoding="utf-8", errors="IGNORE") as file:
     license_contents = file.read()
 
 setuptools.setup(
     name="kthreading",
-    version="0.2",
+    version="0.3",
     description="Get more controls over threads",
     long_description=readme_contents,
-    long_description_content_type = "text/markdown",
+    long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
-    python_requires = ">=3.5"
+    python_requires=">=3.5",
+    packages=["kthreading"],
 )
```

