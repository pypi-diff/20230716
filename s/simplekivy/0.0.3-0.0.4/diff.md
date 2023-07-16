# Comparing `tmp/simplekivy-0.0.3.tar.gz` & `tmp/simplekivy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplekivy-0.0.3.tar", last modified: Sun Jul  9 14:13:05 2023, max compression
+gzip compressed data, was "simplekivy-0.0.4.tar", last modified: Sun Jul 16 12:32:23 2023, max compression
```

## Comparing `simplekivy-0.0.3.tar` & `simplekivy-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.498063 simplekivy-0.0.3/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1057 2023-06-26 12:44:34.000000 simplekivy-0.0.3/LICENSE
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4044 2023-07-09 14:13:05.494063 simplekivy-0.0.3/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     3492 2023-07-08 23:37:27.000000 simplekivy-0.0.3/README.md
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-08 23:32:00.000000 simplekivy-0.0.3/pyproject.toml
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-09 14:13:05.498063 simplekivy-0.0.3/setup.cfg
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.494063 simplekivy-0.0.3/simplekivy/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.3/simplekivy/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      786 2023-07-06 16:35:37.000000 simplekivy-0.0.3/simplekivy/simplekivy.py
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.494063 simplekivy-0.0.3/simplekivy/widgets/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       25 2023-06-25 14:58:13.000000 simplekivy-0.0.3/simplekivy/widgets/__init__.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1763 2023-07-09 14:06:29.000000 simplekivy-0.0.3/simplekivy/widgets/app.py
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.3/simplekivy/widgets/main.kv
-drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-09 14:13:05.494063 simplekivy-0.0.3/simplekivy.egg-info/
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4044 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/PKG-INFO
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/SOURCES.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/dependency_links.txt
--rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-09 14:13:05.000000 simplekivy-0.0.3/simplekivy.egg-info/top_level.txt
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     1058 2023-07-13 13:38:06.000000 simplekivy-0.0.4/LICENSE
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4691 2023-07-16 12:32:23.277637 simplekivy-0.0.4/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4139 2023-07-16 12:25:53.000000 simplekivy-0.0.4/README.md
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      693 2023-07-16 12:21:27.000000 simplekivy-0.0.4/pyproject.toml
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       38 2023-07-16 12:32:23.277637 simplekivy-0.0.4/setup.cfg
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/simplekivy/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       35 2023-06-26 13:46:46.000000 simplekivy-0.0.4/simplekivy/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      912 2023-07-16 11:59:18.000000 simplekivy-0.0.4/simplekivy/simplekivy.py
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/simplekivy/widgets/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       37 2023-07-16 11:58:18.000000 simplekivy-0.0.4/simplekivy/widgets/__init__.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     2849 2023-07-16 11:57:21.000000 simplekivy-0.0.4/simplekivy/widgets/app.py
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      443 2023-07-03 11:21:37.000000 simplekivy-0.0.4/simplekivy/widgets/main.kv
+drwxrwxr-x   0 yoyo      (1000) yoyo      (1000)        0 2023-07-16 12:32:23.277637 simplekivy-0.0.4/simplekivy.egg-info/
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)     4691 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/PKG-INFO
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)      300 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)        1 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yoyo      (1000) yoyo      (1000)       11 2023-07-16 12:32:23.000000 simplekivy-0.0.4/simplekivy.egg-info/top_level.txt
```

### Comparing `simplekivy-0.0.3/LICENSE` & `simplekivy-0.0.4/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 yousuf mahmoud
+Copyright (c) 2023 Yousuf mahmoud
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `simplekivy-0.0.3/PKG-INFO` & `simplekivy-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.3
+Version: 0.0.4
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,28 +20,53 @@
 
 ### Perfect versions:
 -------
 * [kivy==2.2.1]("https://pypi.org/project/Kivy/2.2.1/") 
 * python >= 3.7
 
 
-simplekivy is built on kivy to write simple code faster
+simplekivy is built with kivy to write quickly simple codes
 
 you can write kvlang and creat your own classes and widgets as kivy is flexible
 
 the widgets are added only once via simpleKivyObject + [
 
 #kv_widgets
 
 ]
 
+and you can build simplekivy way using `s.build`
+
 ### Examples to test:
 -----
 
 ```python
+from simplekivy import SimpleKivy
+s = SimpleKivy(title="test app")
+
+box = s.build([s.Label(text="qf47", pos_hint={"center_y": .8})])
+floatL = s.build("""
+FloatLayout:
+    
+    Button:
+        text:"test"
+        size_hint:.3, .2
+        pos_hint: {"center_y": .8}
+""")
+s + [(
+    {s.BoxLayout: box,
+    s.BoxLayout(size_hint=(None, None)): [s.Label(text="qfe")],
+    floatL: s.Label(text="testo testo"),
+    },)
+]
+#as you know for python dict .. key "objects" should be different objects
+
+```
+
+```python
 
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test")
 dp = s.metrics.dp
 s + [
     (# floatlayout <=> ()
         {"size_hint": (1, None)},#<=> add the floatlayout kwargs
@@ -103,21 +128,18 @@
     s.Label(text="hello world", halign="center"),
     s.Label(text="testo")],
     ({"size_hint":(.4, .6), "pos_hint":{"center_x":.5}},
         ainput
     )
 ]
 ```
-<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="500">
-
-
 
 you can also add kvlang string directly instead of using 
 `s.lang.Builder`
-or `kivy.lang.Builder`
+or `kivy.lang.Builder` or `s.build`
 
 ```python
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test app", make_app=True)
 
 def on_enter(instance):
     print(instance.text)
@@ -152,20 +174,25 @@
     ({"size_hint": (1, .4)},
         KV_BTN),
 ]
 
 
 ```
 
-<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
-
 ### Hints
 ------
 
 - list => BoxLayout
 - tuple => FloatLayout
 - set `make_app` to `False` if you do not want to run the kivy App 
 ```python
 s = SimpleKivy(make_app=False)
 ```
 - to reach the main App object do `s.myapp`
+- you can pass to `s.build` a `list, tuple, dict and kivy lang string`
 - the more you understand kivy, the more you enjoy its flexibility
+
+----
+
+<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="300">
+
+<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="300">
```

### Comparing `simplekivy-0.0.3/README.md` & `simplekivy-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,53 @@
 
 ### Perfect versions:
 -------
 * [kivy==2.2.1]("https://pypi.org/project/Kivy/2.2.1/") 
 * python >= 3.7
 
 
-simplekivy is built on kivy to write simple code faster
+simplekivy is built with kivy to write quickly simple codes
 
 you can write kvlang and creat your own classes and widgets as kivy is flexible
 
 the widgets are added only once via simpleKivyObject + [
 
 #kv_widgets
 
 ]
 
+and you can build simplekivy way using `s.build`
+
 ### Examples to test:
 -----
 
 ```python
+from simplekivy import SimpleKivy
+s = SimpleKivy(title="test app")
+
+box = s.build([s.Label(text="qf47", pos_hint={"center_y": .8})])
+floatL = s.build("""
+FloatLayout:
+    
+    Button:
+        text:"test"
+        size_hint:.3, .2
+        pos_hint: {"center_y": .8}
+""")
+s + [(
+    {s.BoxLayout: box,
+    s.BoxLayout(size_hint=(None, None)): [s.Label(text="qfe")],
+    floatL: s.Label(text="testo testo"),
+    },)
+]
+#as you know for python dict .. key "objects" should be different objects
+
+```
+
+```python
 
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test")
 dp = s.metrics.dp
 s + [
     (# floatlayout <=> ()
         {"size_hint": (1, None)},#<=> add the floatlayout kwargs
@@ -89,21 +114,18 @@
     s.Label(text="hello world", halign="center"),
     s.Label(text="testo")],
     ({"size_hint":(.4, .6), "pos_hint":{"center_x":.5}},
         ainput
     )
 ]
 ```
-<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="500">
-
-
 
 you can also add kvlang string directly instead of using 
 `s.lang.Builder`
-or `kivy.lang.Builder`
+or `kivy.lang.Builder` or `s.build`
 
 ```python
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test app", make_app=True)
 
 def on_enter(instance):
     print(instance.text)
@@ -138,20 +160,25 @@
     ({"size_hint": (1, .4)},
         KV_BTN),
 ]
 
 
 ```
 
-<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
-
 ### Hints
 ------
 
 - list => BoxLayout
 - tuple => FloatLayout
 - set `make_app` to `False` if you do not want to run the kivy App 
 ```python
 s = SimpleKivy(make_app=False)
 ```
 - to reach the main App object do `s.myapp`
+- you can pass to `s.build` a `list, tuple, dict and kivy lang string`
 - the more you understand kivy, the more you enjoy its flexibility
+
+----
+
+<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="300">
+
+<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="300">
```

### Comparing `simplekivy-0.0.3/pyproject.toml` & `simplekivy-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "simplekivy"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="yousuf", email="yosefmahmoud356@gmail.com" },
 ]
 description = "the idea is inspired by PySimpleGui , to quickly create simple kivy apps "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplekivy-0.0.3/simplekivy/simplekivy.py` & `simplekivy-0.0.4/simplekivy/simplekivy.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import kivy
 from kivy.factory import Factory as F
 from kivy.clock import mainthread
 
 from threading import Thread
 from time import sleep
 
-from .widgets import MainApp
+from .widgets import MainApp, AppMethods
 
 
 class SimpleKivy:
     def __init__(self, make_app=True, *args, **kwargs):
         if make_app:
             self.myapp = MainApp(*args, **kwargs)
         
@@ -28,8 +28,11 @@
             return getattr(F, attr)
 
         else:
             raise Exception(attr + " doasn't exists")
     def get_running_app(self):
         return kivy.app.App.get_running_app()
 
-
+    def build(self, widgets):
+        app = AppMethods()
+        widget = app.freeze(widgets)
+        return widget
```

### Comparing `simplekivy-0.0.3/simplekivy.egg-info/PKG-INFO` & `simplekivy-0.0.4/simplekivy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplekivy
-Version: 0.0.3
+Version: 0.0.4
 Summary: the idea is inspired by PySimpleGui , to quickly create simple kivy apps 
 Author-email: yousuf <yosefmahmoud356@gmail.com>
 Project-URL: Homepage, https://github.com/yousuf60/SimpleKivy
 Project-URL: Bug Tracker, https://github.com/yousuf60/SimpleKivy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,28 +20,53 @@
 
 ### Perfect versions:
 -------
 * [kivy==2.2.1]("https://pypi.org/project/Kivy/2.2.1/") 
 * python >= 3.7
 
 
-simplekivy is built on kivy to write simple code faster
+simplekivy is built with kivy to write quickly simple codes
 
 you can write kvlang and creat your own classes and widgets as kivy is flexible
 
 the widgets are added only once via simpleKivyObject + [
 
 #kv_widgets
 
 ]
 
+and you can build simplekivy way using `s.build`
+
 ### Examples to test:
 -----
 
 ```python
+from simplekivy import SimpleKivy
+s = SimpleKivy(title="test app")
+
+box = s.build([s.Label(text="qf47", pos_hint={"center_y": .8})])
+floatL = s.build("""
+FloatLayout:
+    
+    Button:
+        text:"test"
+        size_hint:.3, .2
+        pos_hint: {"center_y": .8}
+""")
+s + [(
+    {s.BoxLayout: box,
+    s.BoxLayout(size_hint=(None, None)): [s.Label(text="qfe")],
+    floatL: s.Label(text="testo testo"),
+    },)
+]
+#as you know for python dict .. key "objects" should be different objects
+
+```
+
+```python
 
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test")
 dp = s.metrics.dp
 s + [
     (# floatlayout <=> ()
         {"size_hint": (1, None)},#<=> add the floatlayout kwargs
@@ -103,21 +128,18 @@
     s.Label(text="hello world", halign="center"),
     s.Label(text="testo")],
     ({"size_hint":(.4, .6), "pos_hint":{"center_x":.5}},
         ainput
     )
 ]
 ```
-<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="500">
-
-
 
 you can also add kvlang string directly instead of using 
 `s.lang.Builder`
-or `kivy.lang.Builder`
+or `kivy.lang.Builder` or `s.build`
 
 ```python
 from simplekivy import SimpleKivy
 s = SimpleKivy(title="test app", make_app=True)
 
 def on_enter(instance):
     print(instance.text)
@@ -152,20 +174,25 @@
     ({"size_hint": (1, .4)},
         KV_BTN),
 ]
 
 
 ```
 
-<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="500">
-
 ### Hints
 ------
 
 - list => BoxLayout
 - tuple => FloatLayout
 - set `make_app` to `False` if you do not want to run the kivy App 
 ```python
 s = SimpleKivy(make_app=False)
 ```
 - to reach the main App object do `s.myapp`
+- you can pass to `s.build` a `list, tuple, dict and kivy lang string`
 - the more you understand kivy, the more you enjoy its flexibility
+
+----
+
+<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/997481b1-20cb-4571-91f5-fed311f6f7bc" width="300">
+
+<img src="https://github.com/yousuf60/SimpleKivy/assets/64571068/9e9e445e-0c6f-45de-9580-cd7fbde1f010" width="300">
```

