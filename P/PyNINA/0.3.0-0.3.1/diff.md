# Comparing `tmp/PyNINA-0.3.0.tar.gz` & `tmp/PyNINA-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNINA-0.3.0.tar", last modified: Sun Apr 30 11:38:04 2023, max compression
+gzip compressed data, was "PyNINA-0.3.1.tar", last modified: Sun Jul 16 11:25:38 2023, max compression
```

## Comparing `PyNINA-0.3.0.tar` & `PyNINA-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-30 11:38:04.448151 PyNINA-0.3.0/
--rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 PyNINA-0.3.0/LICENSE
--rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-04-30 11:38:04.444534 PyNINA-0.3.0/PKG-INFO
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-30 11:38:04.253357 PyNINA-0.3.0/PyNINA.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)      285 2023-04-30 11:38:04.000000 PyNINA-0.3.0/PyNINA.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-04-30 11:38:03.000000 PyNINA-0.3.0/PyNINA.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1000) user      (1000)      552 2021-09-11 21:30:24.000000 PyNINA-0.3.0/README.md
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-04-30 11:38:04.413967 PyNINA-0.3.0/pynina/
--rwxrwxrwx   0 user      (1000) user      (1000)      138 2023-04-30 11:36:00.000000 PyNINA-0.3.0/pynina/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1431 2023-04-30 11:34:43.000000 PyNINA-0.3.0/pynina/baseApi.py
--rwxrwxrwx   0 user      (1000) user      (1000)    15135 2023-04-30 11:32:16.000000 PyNINA-0.3.0/pynina/const.py
--rwxrwxrwx   0 user      (1000) user      (1000)      696 2022-12-08 20:25:43.000000 PyNINA-0.3.0/pynina/label_matcher.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2143 2022-12-08 20:25:43.000000 PyNINA-0.3.0/pynina/nina.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2434 2022-12-08 20:25:43.000000 PyNINA-0.3.0/pynina/warning.py
--rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-04-30 11:38:04.449874 PyNINA-0.3.0/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)      585 2023-04-30 11:35:19.000000 PyNINA-0.3.0/setup.py
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-16 11:25:38.861994 PyNINA-0.3.1/
+-rwxrwxrwx   0 user      (1000) user      (1000)     1087 2021-08-31 18:45:53.000000 PyNINA-0.3.1/LICENSE
+-rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-07-16 11:25:38.859426 PyNINA-0.3.1/PKG-INFO
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-16 11:25:38.760341 PyNINA-0.3.1/PyNINA.egg-info/
+-rwxrwxrwx   0 user      (1000) user      (1000)     2061 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1000) user      (1000)      285 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        1 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)       15 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)        7 2023-07-16 11:25:38.000000 PyNINA-0.3.1/PyNINA.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1000) user      (1000)      552 2021-09-11 21:30:24.000000 PyNINA-0.3.1/README.md
+drwxrwxrwx   0 user      (1000) user      (1000)        0 2023-07-16 11:25:38.843569 PyNINA-0.3.1/pynina/
+-rwxrwxrwx   0 user      (1000) user      (1000)      138 2023-07-16 11:20:13.000000 PyNINA-0.3.1/pynina/__init__.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     1431 2023-04-30 11:34:43.000000 PyNINA-0.3.1/pynina/baseApi.py
+-rwxrwxrwx   0 user      (1000) user      (1000)    15135 2023-04-30 11:32:16.000000 PyNINA-0.3.1/pynina/const.py
+-rwxrwxrwx   0 user      (1000) user      (1000)      696 2022-12-08 20:25:43.000000 PyNINA-0.3.1/pynina/label_matcher.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2143 2022-12-08 20:25:43.000000 PyNINA-0.3.1/pynina/nina.py
+-rwxrwxrwx   0 user      (1000) user      (1000)     2596 2023-07-16 11:19:44.000000 PyNINA-0.3.1/pynina/warning.py
+-rwxrwxrwx   0 user      (1000) user      (1000)       38 2023-07-16 11:25:38.862535 PyNINA-0.3.1/setup.cfg
+-rwxrwxrwx   0 user      (1000) user      (1000)      585 2023-07-16 11:20:13.000000 PyNINA-0.3.1/setup.py
```

### Comparing `PyNINA-0.3.0/LICENSE` & `PyNINA-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.0/PKG-INFO` & `PyNINA-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNINA
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python API wrapper to retrieve warnings from the german NINA app.
 Home-page: https://gitlab.com/DeerMaximum/pynina
 Author: DeerMaximum
 Author-email: git983456@parabelmail.de
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `PyNINA-0.3.0/PyNINA.egg-info/PKG-INFO` & `PyNINA-0.3.1/PyNINA.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNINA
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python API wrapper to retrieve warnings from the german NINA app.
 Home-page: https://gitlab.com/DeerMaximum/pynina
 Author: DeerMaximum
 Author-email: git983456@parabelmail.de
 License: MIT License
         
         Copyright (c) 2021 DeerMaximum
```

### Comparing `PyNINA-0.3.0/README.md` & `PyNINA-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.0/pynina/baseApi.py` & `PyNINA-0.3.1/pynina/baseApi.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.0/pynina/const.py` & `PyNINA-0.3.1/pynina/const.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.0/pynina/label_matcher.py` & `PyNINA-0.3.1/pynina/label_matcher.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.0/pynina/nina.py` & `PyNINA-0.3.1/pynina/nina.py`

 * *Files identical despite different names*

### Comparing `PyNINA-0.3.0/pynina/warning.py` & `PyNINA-0.3.1/pynina/warning.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
         recommended_actions_raw: list[str] = []
 
         for parameter in infos["parameter"]:
             if parameter["valueName"] == "instructionCode":
                 recommended_actions_raw = parameter["value"].split(" ")
 
-        if matcher is not None:
+        if "instruction" in infos:
+            self.recommended_actions = [infos["instruction"].replace("<br/>", " ")]
+
+        if matcher is not None and len(self.recommended_actions) == 0:
             for code in recommended_actions_raw:
                 self.recommended_actions.append(matcher.match(code))
 
     def __repr__(self) -> str:
         return f"{self.id} ({self.sent}): [{self.sender}, {self.start} - " \
                f"{self.expires} ({self.sent})] {self.headline}, {self.description}"
```

### Comparing `PyNINA-0.3.0/setup.py` & `PyNINA-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setup(
     name="PyNINA",
-    version="0.3.0",
+    version="0.3.1",
     description="A Python API wrapper to retrieve warnings from the german NINA app.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/DeerMaximum/pynina",
     author="DeerMaximum",
     author_email="git983456@parabelmail.de",
     license=license,
```

