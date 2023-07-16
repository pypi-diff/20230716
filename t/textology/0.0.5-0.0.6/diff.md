# Comparing `tmp/textology-0.0.5.tar.gz` & `tmp/textology-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textology-0.0.5.tar", last modified: Sun Jul  9 16:28:27 2023, max compression
+gzip compressed data, was "textology-0.0.6.tar", last modified: Sun Jul 16 17:19:26 2023, max compression
```

## Comparing `textology-0.0.5.tar` & `textology-0.0.6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.314627 textology-0.0.5/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.0.5/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.0.5/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    12230 2023-07-09 16:28:27.314966 textology-0.0.5/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)    10868 2023-07-09 16:23:23.000000 textology-0.0.5/README.md
--rw-r--r--   0 dfritz     (502) staff       (20)       22 2023-07-08 19:46:35.000000 textology-0.0.5/requirements-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.0.5/requirements-full-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.0.5/requirements.txt
--rw-r--r--   0 dfritz     (502) staff       (20)     1672 2023-07-09 16:28:27.316897 textology-0.0.5/setup.cfg
--rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.0.5/setup.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.300225 textology-0.0.5/textology/
--rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-09 16:23:23.000000 textology-0.0.5/textology/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     9798 2023-07-09 16:23:23.000000 textology-0.0.5/textology/apps.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2362 2023-07-08 19:46:35.000000 textology-0.0.5/textology/dash_compat.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.0.5/textology/history.py
--rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.0.5/textology/logging.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.305437 textology-0.0.5/textology/observers/
--rw-r--r--   0 dfritz     (502) staff       (20)      711 2023-07-04 19:31:50.000000 textology-0.0.5/textology/observers/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2944 2023-07-04 19:31:50.000000 textology-0.0.5/textology/observers/_dependencies.py
--rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-04 19:31:50.000000 textology-0.0.5/textology/observers/_exceptions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    18649 2023-07-09 16:23:23.000000 textology-0.0.5/textology/observers/_managers.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16596 2023-07-08 19:46:35.000000 textology-0.0.5/textology/pytest_utils.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17750 2023-07-09 14:50:38.000000 textology-0.0.5/textology/router.py
--rw-r--r--   0 dfritz     (502) staff       (20)    29250 2023-07-08 19:46:35.000000 textology-0.0.5/textology/test-template.html
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.313853 textology-0.0.5/textology/widgets/
--rw-r--r--   0 dfritz     (502) staff       (20)     1165 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1248 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_containers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_extensions.py
--rw-r--r--   0 dfritz     (502) staff       (20)     9554 2023-07-09 16:23:23.000000 textology-0.0.5/textology/widgets/_horizontal_menus.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_label.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2047 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/_list_item.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/_list_item_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1981 2023-07-08 19:46:35.000000 textology-0.0.5/textology/widgets/_list_item_meta.py
--rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_list_view.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8683 2023-07-09 16:23:23.000000 textology-0.0.5/textology/widgets/_location.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_modal_dialog.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_static.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.0.5/textology/widgets/_store.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-09 16:28:27.303153 textology-0.0.5/textology.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    12230 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     1050 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      279 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-09 16:28:27.000000 textology-0.0.5/textology.egg-info/top_level.txt
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.205187 textology-0.0.6/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.0.6/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.0.6/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    15352 2023-07-16 17:19:26.205347 textology-0.0.6/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    13990 2023-07-16 17:16:06.000000 textology-0.0.6/README.md
+-rw-r--r--   0 dfritz     (502) staff       (20)       22 2023-07-08 19:46:35.000000 textology-0.0.6/requirements-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      168 2023-07-08 19:46:35.000000 textology-0.0.6/requirements-full-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-04 21:18:52.000000 textology-0.0.6/requirements.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-07-16 17:19:26.206331 textology-0.0.6/setup.cfg
+-rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.0.6/setup.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.193153 textology-0.0.6/textology/
+-rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-07-16 17:16:06.000000 textology-0.0.6/textology/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    12177 2023-07-16 17:16:06.000000 textology-0.0.6/textology/apps.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2362 2023-07-08 19:46:35.000000 textology-0.0.6/textology/dash_compat.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.0.6/textology/history.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.0.6/textology/logging.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.198110 textology-0.0.6/textology/observers/
+-rw-r--r--   0 dfritz     (502) staff       (20)      814 2023-07-16 17:16:06.000000 textology-0.0.6/textology/observers/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3944 2023-07-16 17:16:06.000000 textology-0.0.6/textology/observers/_dependencies.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-04 19:31:50.000000 textology-0.0.6/textology/observers/_exceptions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    23617 2023-07-16 17:16:06.000000 textology-0.0.6/textology/observers/_managers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.0.6/textology/pytest_utils.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.0.6/textology/router.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    29250 2023-07-09 19:13:48.000000 textology-0.0.6/textology/test-template.html
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.204811 textology-0.0.6/textology/widgets/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1165 2023-07-08 19:46:35.000000 textology-0.0.6/textology/widgets/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1712 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1248 2023-07-15 18:59:20.000000 textology-0.0.6/textology/widgets/_containers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     9394 2023-07-15 18:57:36.000000 textology-0.0.6/textology/widgets/_extensions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    11892 2023-07-16 17:16:06.000000 textology-0.0.6/textology/widgets/_horizontal_menus.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1665 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_label.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2265 2023-07-16 17:16:06.000000 textology-0.0.6/textology/widgets/_list_item.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1992 2023-07-08 19:46:35.000000 textology-0.0.6/textology/widgets/_list_item_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1993 2023-07-16 17:16:06.000000 textology-0.0.6/textology/widgets/_list_item_meta.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     4919 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_list_view.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     8683 2023-07-09 16:23:23.000000 textology-0.0.6/textology/widgets/_location.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_modal_dialog.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1765 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_static.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1962 2023-07-04 21:18:52.000000 textology-0.0.6/textology/widgets/_store.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-07-16 17:19:26.195962 textology-0.0.6/textology.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    15352 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     1050 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      279 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-07-16 17:19:26.000000 textology-0.0.6/textology.egg-info/top_level.txt
```

### Comparing `textology-0.0.5/LICENSE` & `textology-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/PKG-INFO` & `textology-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,7 @@
-Metadata-Version: 2.1
-Name: textology
-Version: 0.0.5
-Summary: Textual extensions for creating Terminal User Interfaces
-Home-page: https://github.com/dfrtz/textology
-Author: David Fritz
-License: MIT
-Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
-Project-URL: Source Code, https://github.com/dfrtz/textology
-Platform: MacOS
-Platform: Linux
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Widget Sets
-Classifier: Typing :: Typed
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: full-dev
-License-File: LICENSE
-
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
@@ -99,15 +64,17 @@
 
 - Extended basic widgets, such as:
   - Buttons with ability to declare callbacks inline, and track click counts
   - ListItems with metadata objects and ability to disable event messages
 - New widgets, such as:
   - ListItemHeaders (non-interactive ListItems)
   - HorizontalMenus (walkable list of ListViews with peeking at following lists)
-- "Observer" apps, with "event driven architecture" to detect changes and automatically update UI elements.
+- "Observer" apps, with "event driven architecture" to detect changes, and automatically update UI elements.
+  - Listen to reactive attribute changes.
+  - Listen to posted events/messages.
 - Enhanced testing support
   - Parallel tests via python-xdist
   - Custom testing arguments, such as updating snapshots on failures
 
 
 ## Getting Started
 
@@ -143,17 +110,17 @@
 ```python
 from textology.apps import ObservedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
 app = ObservedApp(
     layout=Container(
-        Button('Ping', id='ping-btn'),
-        Button('Pong', id='pong-btn'),
-        Button('Sing-a-long', id='sing-btn'),
+        Button("Ping", id="ping-btn"),
+        Button("Pong", id="pong-btn"),
+        Button("Sing-a-long", id="sing-btn"),
         Container(
             id="content",
         ),
     )
 )
 
 @app.when(
@@ -180,37 +147,138 @@
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
 app.run()
 ```
 
-- Observation callbacks can also be async:
+- Callbacks can also be async:
 ```python
 @app.when(
     Modified("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 async def delayed_pong(clicks):
     await asyncio.sleep(3)
     return Label(f"Pong pressed {clicks} and updated 3 seconds later")
 ```
 
+
+- <details>
+  <summary>Callbacks can also listen for stateless events, not just stateful attribute updates</summary>
+
+    ```python
+    from textology.apps import ObservedApp
+    from textology.observers import Published, Select, Update
+    from textology.widgets import Button, Container, Label
+    
+    app = ObservedApp(
+        layout=Container(
+            Button("Ping", id="ping-btn"),
+            Button("Pong", id="pong-btn"),
+            Button("Sing-a-long", id="sing-btn"),
+            Container(
+                id="content",
+            ),
+        )
+    )
+    
+    @app.when(
+        Published("ping-btn", Button.Pressed),
+        Update("content", "children"),
+    )
+    def ping(event):
+        return Label(f"Ping pressed {event.button.n_clicks}")
+    
+    @app.when(
+        Published("pong-btn", Button.Pressed),
+        Update("content", "children"),
+    )
+    def pong(event):
+        return Label(f"Pong pressed {event.button.n_clicks}")
+    
+    @app.when(
+        Published("sing-btn", Button.Pressed),
+        Select("ping-btn", "n_clicks"),
+        Select("pong-btn", "n_clicks"),
+        Update("content", "children"),
+    )
+    def song(event, ping_clicks, pong_clicks):
+        if not ping_clicks or not pong_clicks:
+            return Label(f"Press Ping and Pong first to complete the song!")
+        return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
+    
+    app.run()
+    ```
+
+
+- <details>
+  <summary>Callbacks can also be registered on methods, to share across all application instances</summary>
+
+    ```python
+    from textology.apps import ObservedApp
+    from textology.observers import Published, Select, Update, when
+    from textology.widgets import Button, Container, Label
+    
+    
+    class Page(Container):
+        def compose(self):
+            yield Button("Ping", id="ping-btn")
+            yield Button("Pong", id="pong-btn")
+            yield Button("Sing-a-long", id="sing-btn")
+            yield Container(
+                id="content",
+            )
+    
+        @when(
+            Published("ping-btn", Button.Pressed),
+            Update("content", "children"),
+        )
+        def ping(self, event):
+            return Label(f"Ping pressed {event.button.n_clicks}")
+    
+        @when(
+            Published("pong-btn", Button.Pressed),
+            Update("content", "children"),
+        )
+        def pong(self, event):
+            return Label(f"Pong pressed {event.button.n_clicks}")
+    
+        @when(
+            Published("sing-btn", Button.Pressed),
+            Select("ping-btn", "n_clicks"),
+            Select("pong-btn", "n_clicks"),
+            Update("content", "children"),
+        )
+        def song(self, event, ping_clicks, pong_clicks):
+            if not ping_clicks or not pong_clicks:
+                return Label(f"Press Ping and Pong first to complete the song!")
+            return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
+    
+    
+    app = ObservedApp(
+        layout=Page()
+    )
+    
+    app.run()
+    ```
+
+
 - <details>
-  <summary>Observer/callback application (Same as above, but with Dash compatibility object and calls)</summary>
+  <summary>Callbacks can also use Dash code style (Same as others, but with Dash compatibility object and calls)</summary>
 
     ```python
     from textology.dash_compat import DashCompatApp, Input, Output, State
     from textology.widgets import Button, Container, Label
 
     app = DashCompatApp(
         layout=Container(
-            Button('Ping', id='ping-btn'),
-            Button('Pong', id='pong-btn'),
-            Button('Sing-a-long', id='sing-btn'),
+            Button("Ping", id="ping-btn"),
+            Button("Pong", id="pong-btn"),
+            Button("Sing-a-long", id="sing-btn"),
             Container(
                 id="content",
             ),
         )
     )
 
     @app.callback(
@@ -237,15 +305,14 @@
         if not ping_clicks or not pong_clicks:
             return Label(f"Press Ping and Pong first to complete the song!")
         return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
     app.run()
     ```
 
- </details>
 
 ### Extended Widgets
 
 Native Textual widgets can be directly swapped out with Textology extended equivalents. They can then be used as is
 (standard Textual usage), or with extensions (via extra keyword arguments).
 
 - Basic swap (no extensions):
@@ -321,9 +388,7 @@
 
 Other advanced testing features include:
 - Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
 
 View all options by running `pytest -h` and referring to `Custom options:` section.
-
-
```

### Comparing `textology-0.0.5/README.md` & `textology-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: textology
+Version: 0.0.6
+Summary: Textual extensions for creating Terminal User Interfaces
+Home-page: https://github.com/dfrtz/textology
+Author: David Fritz
+License: MIT
+Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
+Project-URL: Source Code, https://github.com/dfrtz/textology
+Platform: MacOS
+Platform: Linux
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Widget Sets
+Classifier: Typing :: Typed
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: full-dev
+License-File: LICENSE
+
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/dfrtz/textology/main/docs/banner.svg" width="450">
 </div>
 
 -----------------
 
@@ -64,15 +99,17 @@
 
 - Extended basic widgets, such as:
   - Buttons with ability to declare callbacks inline, and track click counts
   - ListItems with metadata objects and ability to disable event messages
 - New widgets, such as:
   - ListItemHeaders (non-interactive ListItems)
   - HorizontalMenus (walkable list of ListViews with peeking at following lists)
-- "Observer" apps, with "event driven architecture" to detect changes and automatically update UI elements.
+- "Observer" apps, with "event driven architecture" to detect changes, and automatically update UI elements.
+  - Listen to reactive attribute changes.
+  - Listen to posted events/messages.
 - Enhanced testing support
   - Parallel tests via python-xdist
   - Custom testing arguments, such as updating snapshots on failures
 
 
 ## Getting Started
 
@@ -108,17 +145,17 @@
 ```python
 from textology.apps import ObservedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
 app = ObservedApp(
     layout=Container(
-        Button('Ping', id='ping-btn'),
-        Button('Pong', id='pong-btn'),
-        Button('Sing-a-long', id='sing-btn'),
+        Button("Ping", id="ping-btn"),
+        Button("Pong", id="pong-btn"),
+        Button("Sing-a-long", id="sing-btn"),
         Container(
             id="content",
         ),
     )
 )
 
 @app.when(
@@ -145,37 +182,138 @@
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
 app.run()
 ```
 
-- Observation callbacks can also be async:
+- Callbacks can also be async:
 ```python
 @app.when(
     Modified("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 async def delayed_pong(clicks):
     await asyncio.sleep(3)
     return Label(f"Pong pressed {clicks} and updated 3 seconds later")
 ```
 
+
+- <details>
+  <summary>Callbacks can also listen for stateless events, not just stateful attribute updates</summary>
+
+    ```python
+    from textology.apps import ObservedApp
+    from textology.observers import Published, Select, Update
+    from textology.widgets import Button, Container, Label
+    
+    app = ObservedApp(
+        layout=Container(
+            Button("Ping", id="ping-btn"),
+            Button("Pong", id="pong-btn"),
+            Button("Sing-a-long", id="sing-btn"),
+            Container(
+                id="content",
+            ),
+        )
+    )
+    
+    @app.when(
+        Published("ping-btn", Button.Pressed),
+        Update("content", "children"),
+    )
+    def ping(event):
+        return Label(f"Ping pressed {event.button.n_clicks}")
+    
+    @app.when(
+        Published("pong-btn", Button.Pressed),
+        Update("content", "children"),
+    )
+    def pong(event):
+        return Label(f"Pong pressed {event.button.n_clicks}")
+    
+    @app.when(
+        Published("sing-btn", Button.Pressed),
+        Select("ping-btn", "n_clicks"),
+        Select("pong-btn", "n_clicks"),
+        Update("content", "children"),
+    )
+    def song(event, ping_clicks, pong_clicks):
+        if not ping_clicks or not pong_clicks:
+            return Label(f"Press Ping and Pong first to complete the song!")
+        return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
+    
+    app.run()
+    ```
+
+
+- <details>
+  <summary>Callbacks can also be registered on methods, to share across all application instances</summary>
+
+    ```python
+    from textology.apps import ObservedApp
+    from textology.observers import Published, Select, Update, when
+    from textology.widgets import Button, Container, Label
+    
+    
+    class Page(Container):
+        def compose(self):
+            yield Button("Ping", id="ping-btn")
+            yield Button("Pong", id="pong-btn")
+            yield Button("Sing-a-long", id="sing-btn")
+            yield Container(
+                id="content",
+            )
+    
+        @when(
+            Published("ping-btn", Button.Pressed),
+            Update("content", "children"),
+        )
+        def ping(self, event):
+            return Label(f"Ping pressed {event.button.n_clicks}")
+    
+        @when(
+            Published("pong-btn", Button.Pressed),
+            Update("content", "children"),
+        )
+        def pong(self, event):
+            return Label(f"Pong pressed {event.button.n_clicks}")
+    
+        @when(
+            Published("sing-btn", Button.Pressed),
+            Select("ping-btn", "n_clicks"),
+            Select("pong-btn", "n_clicks"),
+            Update("content", "children"),
+        )
+        def song(self, event, ping_clicks, pong_clicks):
+            if not ping_clicks or not pong_clicks:
+                return Label(f"Press Ping and Pong first to complete the song!")
+            return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
+    
+    
+    app = ObservedApp(
+        layout=Page()
+    )
+    
+    app.run()
+    ```
+
+
 - <details>
-  <summary>Observer/callback application (Same as above, but with Dash compatibility object and calls)</summary>
+  <summary>Callbacks can also use Dash code style (Same as others, but with Dash compatibility object and calls)</summary>
 
     ```python
     from textology.dash_compat import DashCompatApp, Input, Output, State
     from textology.widgets import Button, Container, Label
 
     app = DashCompatApp(
         layout=Container(
-            Button('Ping', id='ping-btn'),
-            Button('Pong', id='pong-btn'),
-            Button('Sing-a-long', id='sing-btn'),
+            Button("Ping", id="ping-btn"),
+            Button("Pong", id="pong-btn"),
+            Button("Sing-a-long", id="sing-btn"),
             Container(
                 id="content",
             ),
         )
     )
 
     @app.callback(
@@ -202,15 +340,14 @@
         if not ping_clicks or not pong_clicks:
             return Label(f"Press Ping and Pong first to complete the song!")
         return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
     app.run()
     ```
 
- </details>
 
 ### Extended Widgets
 
 Native Textual widgets can be directly swapped out with Textology extended equivalents. They can then be used as is
 (standard Textual usage), or with extensions (via extra keyword arguments).
 
 - Basic swap (no extensions):
@@ -286,7 +423,9 @@
 
 Other advanced testing features include:
 - Ability to pass and App, App Pilot, or a module containing an instantiated App or Pilot, to fixtures
 - Custom snapshot paths, including reusing the same snapshot across multiple tests
 - Automatic SVG updates with `pytest --txtology-snap-update`
 
 View all options by running `pytest -h` and referring to `Custom options:` section.
+
+
```

### Comparing `textology-0.0.5/setup.cfg` & `textology-0.0.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 [tool:pytest]
 norecursedirs = .* __pycache__ site-packages venv virtualenv virtualenvs
 filterwarnings = 
 	error
 
 [mypy]
-exclude = (__pycache__|test)/
+exclude = (__pycache__)/
 ignore_missing_imports = True
 warn_unused_configs = True
 show_error_codes = True
 incremental = False
 follow_imports = skip
 disable_error_code = attr-defined,
 	name-defined,
```

### Comparing `textology-0.0.5/setup.py` & `textology-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/apps.py` & `textology-0.0.6/textology/apps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Custom textual Apps with textology extensions included."""
 
 from __future__ import annotations
 
 import logging
+from collections import defaultdict
+from inspect import isawaitable
 from typing import Any
 from typing import Callable
 
 from textual import events
 from textual.app import App
 from textual.app import ComposeResult
 from textual.app import CSSPathType
@@ -190,64 +192,111 @@
             layout=layout,
             driver_class=driver_class,
             css_path=css_path,
             watch_css=watch_css,
         )
         # Manually set up observer manager mixin since App inheritance does not automatically trigger.
         ObserverManager.__init__(self, logger=logger or logging.root)
+        self._observer_message_handler_map = {}
 
     def apply_update(
         self,
         observer_id: str,
         component: Widget,
         component_id: str,
         component_property: str,
         value: Any,
     ) -> None:
         """Apply an update operation on a Widget."""
         if component_property == "children":
             # Children is a special property on widgets, it cannot be directly applied. Manually swap children.
             component.remove_children()
-            if not isinstance(value, list):
-                value = [value]
-            component.mount_all(value)
+            if value:
+                if not isinstance(value, list):
+                    value = [value]
+                component.mount_all(value)
         elif component_property == "screen":
             # Screen is a special property on applications, it cannot be directly applied. Manually add to stack.
             component.app.push_screen(value)
         else:
             super().apply_update(observer_id, component, component_id, component_property, value)
 
     def get_component(self, component_id: str) -> Any:
         """Fina a component in the DOM."""
         try:
             return self.query_one(f"#{component_id}")
         except NoMatches:
             return None
 
+    async def _on_message(self, message: events.Message) -> None:
+        """Process messages after sending to registered observers first."""
+        control = message.control
+        if control:
+            controller_id = control.id
+            if controller_id:
+                cls = message.__class__
+                callbacks = self._observer_message_handler_map.get(f"{controller_id}@{cls.__module__}.{cls.__name__}")
+                if callbacks:
+                    for callback in callbacks:
+                        result = callback(None, message)
+                        if isawaitable(result):
+                            await result
+        await super()._on_message(message)
+
     def on_mount(self, _: events.Mount) -> None:
-        """Ensure the logger is fully loaded after mounting."""
+        """Ensure the widget and observers are fully loaded after mounting."""
         if self.logger == logging.root:
             self.logger = self.log
 
-    def _register_widget_observers(self, widget: Widget) -> None:
+        # Combine global observers with local observers outside init, so that apps can be declared anywhere in modules.
+        combined_observer_map = defaultdict(lambda: defaultdict(list))
+        for observer_map in (self._observer_map, self._observer_map_global):
+            for widget_id, property_map in observer_map.items():
+                for property_id, observers in property_map.items():
+                    combined_observer_map[widget_id][property_id].extend(observers)
+
+        # Register event watchers.
+        for widget_id, property_map in combined_observer_map.items():
+            for property_id, observers in property_map.items():
+                for observer in observers:
+                    if observer.publications:
+                        self._observer_message_handler_map.setdefault(f"{widget_id}@{property_id}", []).append(
+                            self._generate_callback(
+                                widget_id,
+                                property_id,
+                                observer,
+                            )
+                        )
+        self.attach_to_observers(self)
+
+    def _register_reactive_observers(self, widget: Widget) -> None:
         """Enable observers for a newly added widget and its reactive attributes if it has an ID."""
         # Do not watch any widgets or properties for changes that have not had an observer set up.
-        if widget.id not in self._observer_map:
+        widget_id = widget.id
+        if not widget_id or (widget_id not in self._observer_map and widget_id not in self._observer_map_global):
             return
         for property_name in widget._reactives.keys():  # pylint: disable=protected-access
-            if property_name not in self._observer_map[widget.id]:
+            if (
+                property_name not in self._observer_map[widget_id]
+                and property_name not in self._observer_map_global[widget_id]
+            ):
                 continue
-            for callback in self.generate_callbacks(widget.id, property_name):
+            for callback in self.generate_callbacks(widget_id, property_name):
                 self.watch(widget, property_name, callback, init=False)
 
 
 def _post_mount_patch(self: Widget) -> None:
     """Called after the object has been mounted, regardless of mount event, to register observer support."""
     # Call the original function being patched to ensure the widget is fully set up before registering.
     _widget_post_mount(self)
-    if self.id and hasattr(self.app, "_register_widget_observers"):
-        self.app._register_widget_observers(self)  # pylint: disable=protected-access
+    attach_to_observers = getattr(self.app, "attach_to_observers", None)
+    if attach_to_observers:
+        attach_to_observers(self)
+    if self.id:
+        _register_reactive_observers = getattr(self.app, "_register_reactive_observers", None)
+        if _register_reactive_observers:
+            _register_reactive_observers(self)
 
 
 # Patch the base Widget class to allow all reactive attributes to register to observer applications.
 _widget_post_mount = Widget._post_mount  # pylint: disable=protected-access
 Widget._post_mount = _post_mount_patch  # pylint: disable=protected-access
```

### Comparing `textology-0.0.5/textology/dash_compat.py` & `textology-0.0.6/textology/dash_compat.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/history.py` & `textology-0.0.6/textology/history.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/observers/__init__.py` & `textology-0.0.6/textology/observers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Utilities for routing component input/output requests via observation callbacks."""
 
 from ._dependencies import Dependency
 from ._dependencies import Modified
 from ._dependencies import NoUpdate
+from ._dependencies import Published
 from ._dependencies import Select
 from ._dependencies import SupportsID
 from ._dependencies import Update
 from ._dependencies import flatten_dependencies
 from ._exceptions import ObserverException
 from ._exceptions import PreventUpdate
 from ._exceptions import UnknownObserver
+from ._managers import WHEN_DECORATOR
 from ._managers import ObservedObject
 from ._managers import ObservedValue
 from ._managers import Observer
 from ._managers import ObserverManager
 from ._managers import ValueUpdateHandler
 from ._managers import create_observer_register
+from ._managers import when
```

### Comparing `textology-0.0.5/textology/observers/_managers.py` & `textology-0.0.6/textology/observers/_managers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,144 @@
 """Managers for routing component input/output requests via observation callbacks."""
 
 from __future__ import annotations
 
 import abc
 import asyncio
-import functools
+import itertools
 import logging
+import traceback
+import weakref
 from collections import defaultdict
 from inspect import isawaitable
 from typing import Any
 from typing import Callable
 from typing import Coroutine
 
 from textology.logging import NullLogger
 
 from ._dependencies import Dependency
 from ._dependencies import Modified
 from ._dependencies import NoUpdate
+from ._dependencies import Published
 from ._dependencies import Select
 from ._dependencies import Update
 from ._dependencies import flatten_dependencies
 from ._exceptions import PreventUpdate
 from ._exceptions import UnknownObserver
 
 # Type alias to represent function receiving 2 arguments (old value and new value) and returning nothing.
 ValueUpdateHandler = Callable[[Any, Any], Coroutine]
 
+_GLOBAL_OBSERVER_ID_MAP: dict[str, Observer] = {}
+_GLOBAL_OBSERVER_MAP: dict[str, dict[str, list[Observer]]] = defaultdict(lambda: defaultdict(list))
+
+WHEN_DECORATOR = "_textology_when"
+
 
 class Observer:
-    """Specification details for an input/output observer."""
+    """Specification details for an input/output observer.
+
+    External callbacks should be considered stateless: they should not store or request any
+    variables created during previous callbacks, and should only rely on the arguments they provide.
+    To share data across external callbacks, use an external storage type such as a database.
+    """
 
     def __init__(
         self,
+        publications: list[Published],
         modifications: list[Modified],
         selections: list[Select],
         updates: list[Update],
-        callback: Callable | None = None,
-        external: bool = False,
+        func: Callable = False,
     ) -> None:
         """Initialize specifications for observing values.
 
         Args:
+            publications: Component IDs and published event types that provide arguments and trigger the callback.
             modifications: Component IDs and properties that provide arguments and trigger the callback.
             selections: Component IDs and properties that provide additional arguments without triggering the callback.
             updates: Component IDs and properties to update based on the results of the callback.
-            callback: The function to call with input values when triggered.
-            external: Whether the callback is handled by an external endpoint, or locally.
-                Any callbacks handled externally should be considered stateless: they should not store or request any
-                variables created during previous callbacks, and should only rely on the arguments they provide.
-                To share data across external callbacks, use an external storage type such as a database.
+            func: The function to call with input values when triggered.
+                Indirectly called via "callback()" when triggered.
         """
         observer_id = (
-            "..".join(f"{dep.component_id}@{dep.component_property}" for dep in modifications)
+            "..".join(f"{dep.component_id}@{dep.component_property}" for dep in publications + modifications)
             + "..."
             + "..".join(f"{dep.component_id}@{dep.component_property}" for dep in updates)
         )
+        self._method_ref: weakref.ReferenceType | None = None
         self.observer_id = observer_id
+        self.publications = publications
         self.modifications = modifications
         self.selections = selections
         self.updates = updates
-        self.callback = callback
-        self.external = external
+        self.external = False
+        self.func = func
 
     def __hash__(self) -> int:
         """Convert object into hash usable in maps."""
         return hash(str(self))
 
     def __repr__(self) -> str:
         """Convert object into human-readable, machine loadable, text."""
         return (
             f"{self.__class__.__name__}("
-            f"'{self.observer_id}',"
+            f"'{self.publications}',"
             f" {self.modifications},"
             f" {self.selections},"
             f" {self.updates},"
             f"external={self.external})"
         )
 
+    async def callback(self, *args: Any, **kwargs: Any) -> dict[str, dict[str, Any]] | None:
+        """Call the original function with additional callback management, such as conversion to standardized results.
+
+        Args:
+            args: Original positional arguments for function.
+            kwargs: Original keyword arguments for function.
+
+        Returns:
+            A mapping of all results by component ID and property.
+        """
+        func = self.func
+        if self._method_ref:
+            ref = self._method_ref()
+            if ref:
+                func = func.__get__(ref)  # Required to access the method. pylint: disable=unnecessary-dunder-call
+        results = func(*args, **kwargs)  # Invoke original callback.
+        results = await results if isawaitable(results) else results
+
+        if results is NoUpdate or isinstance(results, NoUpdate) or not self.updates:
+            return None
+
+        if len(self.updates) == 1:
+            results = [results]
+
+        component_updates = defaultdict(dict)
+        has_update = False
+        for update_val, update in zip(results, self.updates):
+            if update_val is NoUpdate or isinstance(update_val, NoUpdate):
+                continue
+            has_update = True
+            component_updates[update.component_id][update.component_property] = update_val
+
+        if not has_update:
+            return None
+
+        return component_updates
+
+    def update_method_ref(self, obj: Any) -> None:
+        """Update the weak reference used when the callback is a method.
+
+        Args:
+            obj: Object to store a new weak reference for, and use during callbacks.
+        """
+        self._method_ref = weakref.ref(obj)
+
 
 class ObserverManager:
     """Register and execute input/output callbacks when observed properties change.
 
     Can be used directly as a nested object within an application, or as a "mixin" for an application class. Example:
         manager = ObserverManager() # Or:
         class ObservedApp(ObserverManager):
@@ -94,18 +152,18 @@
     ) -> None:
         """Initialize observation trackers and handlers.
 
         Args:
             logger: Custom logger to send messages to.
         """
         super().__init__()
+        self._observer_id_map = {}
         # Structured as: _observer_map[component_id][component_property] = Observer
         self._observer_map = defaultdict(lambda: defaultdict(list))
-        self._observer_id_map = {}
-        self.logger = logger or NullLogger(__name__)
+        self.logger: logging.Logger | None = logger or NullLogger(__name__)
 
     def apply_update(  # Pass all component arguments to allow subclasses to use. pylint: disable=unused-argument
         self,
         observer_id: str,
         component: Any,
         component_id: str,
         component_property: str,
@@ -120,41 +178,60 @@
             component: Component that the value update will be applied to.
             component_id: ID used to locate the updated component.
             component_property: Property name on the component that the updated value will be applied to.
             value: Updated value to apply to the property.
         """
         setattr(component, component_property, value)
 
-    def _generate_callback(self, modified_id: str, modified_property: str, observer: Observer) -> ValueUpdateHandler:
+    @staticmethod
+    def attach_to_observers(obj: Any) -> None:
+        """Allow observers to call functions as methods with required references if registered at the class level.
+
+        Args:
+            obj: Fully instantiated object with or without functions decorated as observers.
+        """
+        for value in obj.__class__.__dict__.values():
+            if callable(value):
+                observers = getattr(value, WHEN_DECORATOR, None)
+                if observers:
+                    for observer in observers:
+                        observer.update_method_ref(obj)
+
+    def _generate_callback(self, trigger_id: str, modified_property: str, observer: Observer) -> ValueUpdateHandler:
         """Create a callback wrapper that will call the original function with input/output management applied."""
 
         async def _on_update(old_value: Any, new_value: Any) -> None:
             """Process value changes for a component property and apply the requested update operations."""
             update_components = self._get_update_components(observer)
-            if not update_components:
+            if observer.updates and not update_components:
                 # One or more components missing, do not trigger callback.
                 return
             observer_id = observer.observer_id
             args = []
-            for dep in observer.modifications + observer.selections:
-                if dep.component_id == modified_id and dep.component_property == modified_property:
+            for dep in observer.publications + observer.modifications + observer.selections:
+                if isinstance(dep, Published):
+                    # Published events are stateless; they are not available if they are not the trigger.
+                    # Fill events, other than the triggering event, with empty values.
+                    args.append(new_value if dep.component_id == trigger_id else None)
+                elif dep.component_id == trigger_id and dep.component_property == modified_property:
+                    # Properties are stateful; they are available at all times.
+                    # Use new value if this was the trigger, otherwise use historical value to represent "current" state.
                     args.append(old_value if isinstance(dep, Select) else new_value)
                 else:
                     try:
                         args.append(
                             self.get_callback_arg(observer.observer_id, dep.component_id, dep.component_property)
                         )
                     except Exception as error:  # pylint: disable=broad-exception-caught
                         self.on_callback_error(observer_id, error)
                         return
 
             try:
                 updates = observer.callback(*args) if not observer.external else self.send_callback(observer_id, *args)
-                if isawaitable(updates):
-                    updates = await updates
+                updates = await updates if isawaitable(updates) else updates
             except PreventUpdate:
                 updates = None
             except BaseException as error:  # pylint: disable=broad-exception-caught
                 # Catch all errors to prevent fatal crashes in application callback loops.
                 self.on_callback_error(observer_id, error)
                 updates = None
 
@@ -178,14 +255,16 @@
             component_id: ID of a component with a property that will trigger callbacks.
             component_property: Property name on the component that will trigger callbacks.
 
         Returns:
             Callbacks to the original registered functions with automatic input/output management.
         """
         callbacks = []
+        for observer in self._observer_map_global[component_id][component_property]:
+            callbacks.append(self._generate_callback(component_id, component_property, observer))
         for observer in self._observer_map[component_id][component_property]:
             callbacks.append(self._generate_callback(component_id, component_property, observer))
         return callbacks
 
     def get_callback_arg(
         self,
         observer_id: str,
@@ -226,29 +305,47 @@
         for dep in observer.updates:
             component = self.get_component(dep.component_id)
             if not component:
                 return None
             output_components[dep.component_id] = component
         return output_components
 
+    @property
+    def _observer_id_map_global(self) -> dict[str, Observer]:
+        """Return the global observer ID map used across all managers.
+
+        The global observer ID map is populated when functions are decorated at the class or module level.
+        """
+        return _GLOBAL_OBSERVER_ID_MAP
+
+    @property
+    def _observer_map_global(self) -> dict[str, dict[str, list[Observer]]]:
+        """Return the global observer map used across all managers.
+
+        The global observer map is populated when functions are decorated at the class or module level.
+        """
+        return _GLOBAL_OBSERVER_MAP
+
     def on_callback_error(self, observer_id: str, error: BaseException) -> None:
         """Action to perform when a callback fails.
 
         Args:
             observer_id: ID of the observer that failed to run the callback.
             error: Original error that caused the failure.
 
         Raises:
             Original error if lower level than Exception type.
         """
         if not isinstance(error, Exception):
             # Unhandled fatal error; reraise.
             raise error
+        # Not all third party loggers have ".exception()" to print stacktraces, collect manually and use error.
+        full_trace = traceback.format_exc()
         # Standard error, log and continue.
-        self.logger.error(f"Failed callback for {observer_id}: {type(error).__name__} {error}")
+        self.logger.error(f"Failed callback for {observer_id}: {type(error).__name__} {error}\n{full_trace}")
 
     def send_callback(self, observer_id: str, *callback_args: Any) -> dict[str, dict[str, Any]]:
         """Forward a callback request to be handled externally.
 
         Override to send the request to an external endpoint, and wait for the response.
         Any callbacks handled externally should be considered stateless: they should not store or request any
         variables created during a previous callback, and should only rely on the callback arguments they provide.
@@ -269,15 +366,15 @@
         )
         return observer.callback(*callback_args)
 
     def when(
         self,
         *args: Dependency,
     ) -> Callable:
-        """Register a callback that triggers when observed values change.
+        """Register a callback that triggers when observed values change while this instance is active.
 
         Example:
             @app.when(
                 Modified('url', 'path'),
                 Update('content-wrapper', 'content'),
             )
             def route_url(path: str) -> str:
@@ -361,80 +458,96 @@
             value: The initial value.
             callback: Where to send old and new values on update.
         """
         self.value = value
         self.callback = callback
 
 
-def _create_callback(func: Callable, updates: list[Update]) -> Callable:
-    """Wrap a function with additional callback management, such as error handling and result standardization."""
-
-    @functools.wraps(func)
-    async def _callback(*args: Any, **kwargs: Any) -> dict[str, dict[str, Any]]:
-        """Wrap original function with additional callback management such as conversion to standardized result map."""
-        results = func(*args, **kwargs)  # Invoke original callback.
-        if isawaitable(results):
-            results = await results
-        if not isinstance(results, (list, tuple)):
-            results = [results]
-
-        if results is NoUpdate or isinstance(results, NoUpdate):
-            raise PreventUpdate()
-
-        component_updates = defaultdict(dict)
-        has_update = False
-        for update_val, update in zip(results, updates):
-            if update_val is NoUpdate or isinstance(update_val, NoUpdate):
-                continue
-            has_update = True
-            component_updates[update.component_id][update.component_property] = update_val
-
-        if not has_update:
-            raise PreventUpdate()
-
-        return component_updates
-
-    return _callback
-
-
 def create_observer_register(
     observer_map: dict[str, dict[str, list[Observer]]],
     observer_id_map: dict[str, Observer],
-    *observer_args: Any,
+    *observer_args: Dependency,
+    split_publications: bool = False,
     split_modifications: bool = False,
     external: bool = False,
 ) -> Callable:
     """Create a decorator that will wrap a function with additional callback management, and register the observer.
 
     Args:
         observer_map: All currently registered observers by component ID and component property.
             Modified in place when new observer is registered.
         observer_id_map: All currently registered observers by full observer ID.
             Modified in place when new observer is registered.
         observer_args: Positional arguments containing one or more Dependencies.
-        split_modifications: Register the observer once per Modification, instead of once per all Modifications.
+        split_publications: Register the observer once per publication, instead of once per all publications.
+        split_modifications: Register the observer once per modification, instead of once per all modifications.
         external: Whether the callback is handled by an external endpoint, or locally.
             Any callbacks handled externally should be considered stateless: they should not store or request any
             variables created during a previous callback, and should only rely on the callback arguments they provide.
 
     Returns:
         Decorator to register a function as an input/output reaction to one or more property changes.
     """
 
     def _decorator(func: Callable) -> Callable:
         """Wrap the original function with additional callback management, and register the final observer."""
-        modifications, selections, updates = flatten_dependencies(observer_args)
-        callback = _create_callback(func, updates)
-        for modification_group in [[dep] for dep in modifications] if split_modifications else [modifications]:
-            observer = Observer(
-                modification_group,
-                selections,
-                updates,
-                callback=callback,
-                external=external,
+        publications, modifications, selections, updates = flatten_dependencies(observer_args)
+
+        # Triggers can be 1 input/argument per callback, or all per callback.
+        if publications:
+            publications = [[dep] for dep in publications] if split_publications else [publications]
+        if modifications:
+            modifications = [[dep] for dep in modifications] if split_modifications else [modifications]
+
+        observers = []
+        for publication_group, modification_group in itertools.product(publications or [[]], modifications or [[]]):
+            observers.append(
+                Observer(
+                    publication_group,
+                    modification_group,
+                    selections,
+                    updates,
+                    func=func,
+                )
             )
+        for observer in observers:
+            observer.external = external
+            # If the function is not a method (object pre-attached), then tag it in case an object needs to be added.
+            # Tagged functions can be searched later, such as during object init, to convert the callback into a method.
+            if type(func).__name__ != "method":
+                if not hasattr(func, WHEN_DECORATOR):
+                    setattr(func, WHEN_DECORATOR, [])
+                getattr(func, WHEN_DECORATOR).append(observer)
             observer_id_map[observer.observer_id] = observer
-            for dep in modification_group:
-                observer_map[dep.component_id][dep.component_property].append(observer)
-        return callback
+            for dep in observer.publications + observer.modifications:
+                observer_map.setdefault(dep.component_id, {}).setdefault(dep.component_property, []).append(observer)
+
+        # Return the original, unmodified, function; the decorator only tags and/or maps for later usage.
+        return func
 
     return _decorator
+
+
+def when(
+    *args: Dependency,
+) -> Callable:
+    """Register a callback that triggers when observed values change globally.
+
+    Example:
+        @when(
+            Modified('url', 'path'),
+            Update('content-wrapper', 'content'),
+        )
+        def route_url(path: str) -> str:
+            ...
+
+    Args:
+        args: Positional arguments containing one or more observation Dependencies.
+
+    Returns:
+        Decorator to register a function as an input/output reaction to one or more property changes.
+    """
+    return create_observer_register(
+        _GLOBAL_OBSERVER_MAP,
+        _GLOBAL_OBSERVER_ID_MAP,
+        *args,
+    )
```

### Comparing `textology-0.0.5/textology/pytest_utils.py` & `textology-0.0.6/textology/pytest_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,16 +360,16 @@
         report = template.replace(
             'let testResult = "DUMMIES";',
             f"let testResult = {json.dumps(final_result, indent=4)};",
         )
 
         report_path_opt = session.config.getoption(OPT_SNAP_REPORT)
         report_path = Path(report_path_opt) if report_path_opt else Path(session_root / "snapshot_test_report.html")
-        with open(report_path, "w+", encoding="utf-8") as snapshot_file:
-            snapshot_file.write(report)
+        report_path.write_text(report, encoding="utf-8")
+
         session.config.txtology_report_path = report_path
         session.config.txtology_report_count = len(failures)
 
 
 def pytest_terminal_summary(
     terminalreporter: "pytest.TerminalReporter",
     exitstatus: int,  # Match pytest arguments. pylint: disable=unused-argument
```

### Comparing `textology-0.0.5/textology/router.py` & `textology-0.0.6/textology/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     ) -> None:
         """Initialize route endpoint trackers and handlers.
 
         Args:
             logger: Custom logger to send messages to.
         """
         super().__init__()
-        self.logger = logger or NullLogger(__name__)
+        self.logger: logging.Logger | None = logger or NullLogger(__name__)
         self.weighted_endpoints: list[Endpoint] = []
         self.dynamic_endpoints: dict[str, dict[str, Endpoint]] = {}  # dynamic_endpoints[path][method]
         self.static_endpoints: dict[str, dict[str, Endpoint]] = {}  # static_endpoints[path][method]
         self.endpoint_not_allowed: Endpoint = Endpoint([], "", self._default_not_allowed_handler)
         self.endpoint_not_found: Endpoint = Endpoint([], "", self._default_not_found_handler)
         self.error_handler = self._default_error_handler
```

### Comparing `textology-0.0.5/textology/test-template.html` & `textology-0.0.6/textology/test-template.html`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/__init__.py` & `textology-0.0.6/textology/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_button.py` & `textology-0.0.6/textology/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_containers.py` & `textology-0.0.6/textology/widgets/_containers.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_extensions.py` & `textology-0.0.6/textology/widgets/_extensions.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_horizontal_menus.py` & `textology-0.0.6/textology/widgets/_horizontal_menus.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Progressive horizontal set of ListViews with tracking for active item and peeking at next menu."""
 
+from __future__ import annotations
+
 from typing import Any
 from typing import Callable
 from typing import ClassVar
+from typing import Iterable
 
 from textual import containers
 from textual import events
 from textual.binding import Binding
 from textual.binding import BindingType
 from textual.reactive import reactive
 from textual.widget import Widget
@@ -34,14 +37,52 @@
     # Currently focused item across sub-menus.
     focused: ListItem | None = reactive(None, repaint=False, init=False)
     # Current primary item highlighted across sub-menus (right-most).
     highlighted: ListItem | None = reactive(None, repaint=False, init=False)
     # All highlighted items across sub-menus.
     highlights: list[ListItem] = reactive([], repaint=False, init=False)
 
+    class Focused(events.Message, bubble=True):
+        """Posted when the focused item changes."""
+
+        def __init__(self, horizontal_menu: HorizontalMenus, item: ListItem | None) -> None:
+            """Initialize focused event.
+
+            Args:
+                horizontal_menu: Parent menu containing the item.
+                item: New item that was focused.
+            """
+            super().__init__()
+            self.horizontal_menu: HorizontalMenus = horizontal_menu
+            self.item: ListItem | None = item
+
+        @property
+        def control(self) -> HorizontalMenus:
+            """The primary controlling widget that contains the focused item, used by "on()" decorator."""
+            return self.horizontal_menu
+
+    class Highlighted(events.Message, bubble=True):
+        """Posted when the highlighted item changes."""
+
+        def __init__(self, horizontal_menu: HorizontalMenus, item: ListItem | None) -> None:
+            """Initialize highlight event.
+
+            Args:
+                horizontal_menu: Parent menu containing the item.
+                item: New item that was highlighted.
+            """
+            super().__init__()
+            self.horizontal_menu: HorizontalMenus = horizontal_menu
+            self.item: ListItem | None = item
+
+        @property
+        def control(self) -> HorizontalMenus:
+            """The primary controlling widget that contains the highlighted item, used by "on()" decorator."""
+            return self.horizontal_menu
+
     def __init__(
         self,
         *children: Widget | ListItem | ListItemMeta,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
@@ -64,16 +105,15 @@
             menu_creator: Called to create new sub-menus when an item with children is highlighted.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
         self.menu_creator = menu_creator or self._default_menu_creator
         if any(isinstance(child, (ListItem, ListItemMeta)) for child in children):
             if not all(isinstance(child, (ListItem, ListItemMeta)) for child in children):
                 raise ValueError("All initial children must be of same type: ListItem, ListItemMeta, or ListView")
-            for child in children:
-                child.menu_index = 0
+            self._update_menu_index(children, 0)
             children = [
                 self.menu_creator(
                     0,
                     [child.to_item() if isinstance(child, ListItemMeta) else child for child in children],
                 )
             ]
         super().__init__(
@@ -190,35 +230,55 @@
 
         Args:
             index: Position of the menu to create or update.
             items: New items to show in the menu at the provided index.
         """
         for item in items:
             item.menu_index = index
+        self._update_menu_index(items, index)
         if index >= len(self.menus):
             self._add_menu(items)
         else:
             self._update_menu(index, items)
 
     def _update_menu(self, index: int, new_items: list[ListItem]) -> None:
         """Update the items in an existing menu."""
         # Do not count headers towards the available items to display in a sub-menu.
         non_headers = [item for item in new_items if not isinstance(item, ListItemHeader)]
         self.remove_menus(index if non_headers else index - 1)
         if index < len(self.menus):
             self.menus[index].replace(new_items)
 
+    @staticmethod
+    def _update_menu_index(items: Iterable[ListItem | ListItemMeta], index: int) -> None:
+        """Update the menu index value on all items in a list."""
+        for item in items:
+            item.menu_index = index
+
+    def watch_focused(self, old_value: ListItem | None, new_value: ListItem | None) -> None:
+        """Monitor the focused item to update listeners.
+
+        Args:
+            old_value: Previously focused list item.
+            new_value: Newly focused list item.
+        """
+        if new_value == old_value or not new_value:
+            return
+        self.post_message(self.Focused(self, new_value))
+
     def watch_highlighted(self, old_value: ListItem | None, new_value: ListItem | None) -> None:
-        """Monitor the highlighted item to update the submenus.
+        """Monitor the highlighted item to update the submenus and listeners.
 
         Args:
             old_value: Previously highlighted list item.
             new_value: Newly highlighted list item.
         """
         if new_value == old_value or not new_value:
             return
         menu_items = new_value.data.get("menu_items")
+        menu_index = new_value.menu_index or 0
         if menu_items:
             list_items = [item.to_item() for item in menu_items]
-            self.show_menu(new_value.menu_index + 1, list_items)
+            self.show_menu(menu_index + 1, list_items)
         else:
-            self.remove_menus(new_value.menu_index)
+            self.remove_menus(menu_index)
+        self.post_message(self.Highlighted(self, new_value))
```

### Comparing `textology-0.0.5/textology/widgets/_label.py` & `textology-0.0.6/textology/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_list_item.py` & `textology-0.0.6/textology/widgets/_list_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,23 +33,28 @@
         **extension_configs: Any,
     ) -> None:
         """Initialize a ListItem with extension arguments.
 
         Args:
             *children: Child widgets.
             name: The name of the widget.
+                If no child is provided for display, and no "data" with "label" key, name will be used in a Label.
             id: The ID of the widget in the DOM.
             classes: The CSS classes for the widget.
             disabled: Whether the widget is disabled or not.
             data: Optional data associated with the list item.
                 If no child is provided for display, the data will be searched for a "label" key to use in a Label.
             extension_configs: Widget extension configurations, such as dynamically provided local callbacks by name.
         """
-        if not children and (data and "label" in data):
-            children = [Label(data["label"], disable_messages=LIST_ITEM_EVENT_IGNORES)]
+        if not children:
+            label = name
+            if data and "label" in data:
+                label = data["label"]
+            if label:
+                children = [Label(label, disable_messages=LIST_ITEM_EVENT_IGNORES)]
 
         super().__init__(*children, name=name, id=id, classes=classes, disabled=disabled)
         if "disable_messages" not in extension_configs:
             extension_configs["disable_messages"] = LIST_ITEM_EVENT_IGNORES
         self.__extend_widget__(**extension_configs)
         self.data = data
-        self.menu_index = None
+        self.menu_index: int | None = None
```

### Comparing `textology-0.0.5/textology/widgets/_list_item_header.py` & `textology-0.0.6/textology/widgets/_list_item_header.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_list_item_meta.py` & `textology-0.0.6/textology/widgets/_list_item_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             raise ValueError("Item type must be a subclass of ListItem")
         self.item_type = item_type
         self.name = name
         self.id = id
         self.classes = classes
         self.data = data
         self.extension_configs = extension_configs
-        self.menu_index = None
+        self.menu_index: int | None = None
 
     def to_item(self) -> ListItem:
         """Create the underlying list item widget.
 
         Returns:
             Newly created item that can be used in a list view.
         """
```

### Comparing `textology-0.0.5/textology/widgets/_list_view.py` & `textology-0.0.6/textology/widgets/_list_view.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_location.py` & `textology-0.0.6/textology/widgets/_location.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_modal_dialog.py` & `textology-0.0.6/textology/widgets/_modal_dialog.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_static.py` & `textology-0.0.6/textology/widgets/_static.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology/widgets/_store.py` & `textology-0.0.6/textology/widgets/_store.py`

 * *Files identical despite different names*

### Comparing `textology-0.0.5/textology.egg-info/PKG-INFO` & `textology-0.0.6/textology.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.0.5
+Version: 0.0.6
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
@@ -99,15 +99,17 @@
 
 - Extended basic widgets, such as:
   - Buttons with ability to declare callbacks inline, and track click counts
   - ListItems with metadata objects and ability to disable event messages
 - New widgets, such as:
   - ListItemHeaders (non-interactive ListItems)
   - HorizontalMenus (walkable list of ListViews with peeking at following lists)
-- "Observer" apps, with "event driven architecture" to detect changes and automatically update UI elements.
+- "Observer" apps, with "event driven architecture" to detect changes, and automatically update UI elements.
+  - Listen to reactive attribute changes.
+  - Listen to posted events/messages.
 - Enhanced testing support
   - Parallel tests via python-xdist
   - Custom testing arguments, such as updating snapshots on failures
 
 
 ## Getting Started
 
@@ -143,17 +145,17 @@
 ```python
 from textology.apps import ObservedApp
 from textology.observers import Modified, Select, Update
 from textology.widgets import Button, Container, Label
 
 app = ObservedApp(
     layout=Container(
-        Button('Ping', id='ping-btn'),
-        Button('Pong', id='pong-btn'),
-        Button('Sing-a-long', id='sing-btn'),
+        Button("Ping", id="ping-btn"),
+        Button("Pong", id="pong-btn"),
+        Button("Sing-a-long", id="sing-btn"),
         Container(
             id="content",
         ),
     )
 )
 
 @app.when(
@@ -180,37 +182,138 @@
     if not ping_clicks or not pong_clicks:
         return Label(f"Press Ping and Pong first to complete the song!")
     return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
 app.run()
 ```
 
-- Observation callbacks can also be async:
+- Callbacks can also be async:
 ```python
 @app.when(
     Modified("pong-btn", "n_clicks"),
     Update("content", "children"),
 )
 async def delayed_pong(clicks):
     await asyncio.sleep(3)
     return Label(f"Pong pressed {clicks} and updated 3 seconds later")
 ```
 
+
+- <details>
+  <summary>Callbacks can also listen for stateless events, not just stateful attribute updates</summary>
+
+    ```python
+    from textology.apps import ObservedApp
+    from textology.observers import Published, Select, Update
+    from textology.widgets import Button, Container, Label
+    
+    app = ObservedApp(
+        layout=Container(
+            Button("Ping", id="ping-btn"),
+            Button("Pong", id="pong-btn"),
+            Button("Sing-a-long", id="sing-btn"),
+            Container(
+                id="content",
+            ),
+        )
+    )
+    
+    @app.when(
+        Published("ping-btn", Button.Pressed),
+        Update("content", "children"),
+    )
+    def ping(event):
+        return Label(f"Ping pressed {event.button.n_clicks}")
+    
+    @app.when(
+        Published("pong-btn", Button.Pressed),
+        Update("content", "children"),
+    )
+    def pong(event):
+        return Label(f"Pong pressed {event.button.n_clicks}")
+    
+    @app.when(
+        Published("sing-btn", Button.Pressed),
+        Select("ping-btn", "n_clicks"),
+        Select("pong-btn", "n_clicks"),
+        Update("content", "children"),
+    )
+    def song(event, ping_clicks, pong_clicks):
+        if not ping_clicks or not pong_clicks:
+            return Label(f"Press Ping and Pong first to complete the song!")
+        return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
+    
+    app.run()
+    ```
+
+
+- <details>
+  <summary>Callbacks can also be registered on methods, to share across all application instances</summary>
+
+    ```python
+    from textology.apps import ObservedApp
+    from textology.observers import Published, Select, Update, when
+    from textology.widgets import Button, Container, Label
+    
+    
+    class Page(Container):
+        def compose(self):
+            yield Button("Ping", id="ping-btn")
+            yield Button("Pong", id="pong-btn")
+            yield Button("Sing-a-long", id="sing-btn")
+            yield Container(
+                id="content",
+            )
+    
+        @when(
+            Published("ping-btn", Button.Pressed),
+            Update("content", "children"),
+        )
+        def ping(self, event):
+            return Label(f"Ping pressed {event.button.n_clicks}")
+    
+        @when(
+            Published("pong-btn", Button.Pressed),
+            Update("content", "children"),
+        )
+        def pong(self, event):
+            return Label(f"Pong pressed {event.button.n_clicks}")
+    
+        @when(
+            Published("sing-btn", Button.Pressed),
+            Select("ping-btn", "n_clicks"),
+            Select("pong-btn", "n_clicks"),
+            Update("content", "children"),
+        )
+        def song(self, event, ping_clicks, pong_clicks):
+            if not ping_clicks or not pong_clicks:
+                return Label(f"Press Ping and Pong first to complete the song!")
+            return Label(f"Ping, pong, sing-a-long song pressed {event.button.n_clicks}")
+    
+    
+    app = ObservedApp(
+        layout=Page()
+    )
+    
+    app.run()
+    ```
+
+
 - <details>
-  <summary>Observer/callback application (Same as above, but with Dash compatibility object and calls)</summary>
+  <summary>Callbacks can also use Dash code style (Same as others, but with Dash compatibility object and calls)</summary>
 
     ```python
     from textology.dash_compat import DashCompatApp, Input, Output, State
     from textology.widgets import Button, Container, Label
 
     app = DashCompatApp(
         layout=Container(
-            Button('Ping', id='ping-btn'),
-            Button('Pong', id='pong-btn'),
-            Button('Sing-a-long', id='sing-btn'),
+            Button("Ping", id="ping-btn"),
+            Button("Pong", id="pong-btn"),
+            Button("Sing-a-long", id="sing-btn"),
             Container(
                 id="content",
             ),
         )
     )
 
     @app.callback(
@@ -237,15 +340,14 @@
         if not ping_clicks or not pong_clicks:
             return Label(f"Press Ping and Pong first to complete the song!")
         return Label(f"Ping, pong, sing-a-long song pressed {song_clicks}")
 
     app.run()
     ```
 
- </details>
 
 ### Extended Widgets
 
 Native Textual widgets can be directly swapped out with Textology extended equivalents. They can then be used as is
 (standard Textual usage), or with extensions (via extra keyword arguments).
 
 - Basic swap (no extensions):
```

### Comparing `textology-0.0.5/textology.egg-info/SOURCES.txt` & `textology-0.0.6/textology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

