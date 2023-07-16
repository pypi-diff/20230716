# Comparing `tmp/unigui-1.8.2.tar.gz` & `tmp/unigui-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.8.2.tar", last modified: Fri Jul 14 23:31:00 2023, max compression
+gzip compressed data, was "dist/unigui-1.8.3.tar", last modified: Sun Jul 16 01:30:50 2023, max compression
```

## Comparing `unigui-1.8.2.tar` & `unigui-1.8.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     8633 2023-07-12 21:13:45.000000 unigui-1.8.2/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3362 2023-07-14 23:14:58.000000 unigui-1.8.2/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      100 2023-07-14 22:20:13.000000 unigui-1.8.2/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2881 2023-07-14 19:50:43.000000 unigui-1.8.2/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     4564 2023-07-14 22:55:02.000000 unigui-1.8.2/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     9555 2023-07-14 22:58:25.000000 unigui-1.8.2/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/css/423.a6a82bd4.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    44594 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/423.0ad6769b.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/app.eb412190.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/vendor.e1e2597e.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.2/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      612 2023-07-14 23:07:35.000000 unigui-1.8.2/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18989 2023-07-14 23:31:00.000000 unigui-1.8.2/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-14 23:31:00.000000 unigui-1.8.2/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18684 2023-07-12 08:54:15.000000 unigui-1.8.2/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.2/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       39 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18989 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.2/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1222 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     8633 2023-07-12 21:13:45.000000 unigui-1.8.3/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3501 2023-07-16 00:57:22.000000 unigui-1.8.3/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      100 2023-07-14 22:20:13.000000 unigui-1.8.3/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     1993 2023-07-16 01:29:01.000000 unigui-1.8.3/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2881 2023-07-14 19:50:43.000000 unigui-1.8.3/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4564 2023-07-14 22:55:02.000000 unigui-1.8.3/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9724 2023-07-15 20:14:37.000000 unigui-1.8.3/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/css/310.054e803c.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    44988 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/js/310.1f9849f3.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1432869 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/js/vendor.f354d0dd.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/js/app.8ade4146.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-16 00:40:30.000000 unigui-1.8.3/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.3/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      612 2023-07-16 01:30:28.000000 unigui-1.8.3/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18989 2023-07-16 01:30:50.000000 unigui-1.8.3/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-16 01:30:50.000000 unigui-1.8.3/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18684 2023-07-12 08:54:15.000000 unigui-1.8.3/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.3/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       39 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18989 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.3/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1241 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-16 01:30:50.000000 unigui-1.8.3/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.8.2/unigui/guielements.py` & `unigui-1.8.3/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/server.py` & `unigui-1.8.3/unigui/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from aiohttp import web, WSMsgType
 from .users import *
 from config import port, pretty_print, socket_ip, upload_dir
 from pathlib import Path
 from .reloader import empty_app 
+from .autotest import recorder
 
 async def post_handler(request):
     reader = await request.multipart()
     field = await reader.next()   
     filename = upload_path(field.filename)  
     # You cannot rely on Content-Length if transfer is chunked.
     size = 0
@@ -53,16 +54,19 @@
         async for msg in ws:
             if msg.type == WSMsgType.TEXT:
                 if msg.data == 'close':
                     await ws.close()
                 else:
                     data = json.loads(msg.data)            
                     result = user.result4message(data)
-                    if result:                
-                        await ws.send_str(jsonString(user.prepare_result(result)))
+                    if result:            
+                        result = jsonString(user.prepare_result(result))    
+                        await ws.send_str(result)
+                    recorder(msg.data, result)
+                    
             elif msg.type == WSMsgType.ERROR:
                 print('ws connection closed with exception %s' %
                     ws.exception())
     except:
         type, value, traceback = sys.exc_info()
         user.log(f'{type}: {value} \n{traceback.format_exc()}\n')
```

### Comparing `unigui-1.8.2/unigui/utils.py` & `unigui-1.8.3/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/reloader.py` & `unigui-1.8.3/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/users.py` & `unigui-1.8.3/unigui/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 from threading import Thread
 import logging
 
 class User:      
     def __init__(self):          
         self.screens = []        
         self.active_dialog = None
-        self.screen_module = None                
-        self.tool_buttons = []
-        User.last_user = self
+        self.screen_module = None                        
+        User.last_user = self        
 
     def log(self, str, type = 'error'):        
         scr = self.screen.name if self.screens else 'omitted'
         str = f"session: {self.session__}, screen: {scr}, message: {self.message__} \n  {str}"
         if type == 'error':
             logging.error(str)
         else:
@@ -71,15 +70,15 @@
                        
     def load_module(self, file):
         screen_vars = {
             'icon' : None,
             'prepare' : None,            
             'blocks' : [],
             'header' : utils.appname,                        
-            'toolbar' : [], 
+            'toolbar' : User.toolbar, 
             'order' : 0
         }             
         name = file[0:-3]        
         path = f'{screens_dir}/{file}'                
         spec = importlib.util.spec_from_file_location(name,path)
         module = importlib.util.module_from_spec(spec)        
         
@@ -89,31 +88,33 @@
         spec.loader.exec_module(module)            
         screen = Screen(module.name)
         #set system vars
         for var in screen_vars:                                            
             setattr(screen, var, getattr(module,var,screen_vars[var])) 
         module.handlers__ = utils.handlers__
         
-        if not screen.toolbar:
-            screen.toolbar = self.tool_buttons
+        if screen.toolbar:
+            screen.toolbar += User.toolbar
+        else: 
+            screen.toolbar = User.toolbar  
                         
         screen.check()                         
         module.screen = screen
         return module
 
     def set_clean(self):
         #remove user modules from sys 
         if os.path.exists(blocks_dir):
             for file in os.listdir(blocks_dir):
                 if file.endswith(".py") and file != '__init__.py':
                     name = f'{blocks_dir}.{file[0:-3]}'
                     if name in sys.modules:
                         sys.modules[name].user = self
                         del sys.modules[name]                          
-    def load(self):            
+    def load(self):              
         if os.path.exists(screens_dir):
             for file in os.listdir(screens_dir):
                 if file.endswith(".py") and file != '__init__.py':
                     module = self.load_module(file)                
                     self.screens.append(module)                
             
         if self.screens:
@@ -199,15 +200,15 @@
             elif isinstance(raw,Gui):
                 raw = Message(raw, user = self)                 
             elif isinstance(raw, (list, tuple)) and all(isinstance(e,Gui) for e in raw):
                 raw = Message(*raw, user = self)
         return raw
 
     def process(self,arr):
-        self.message__ = arr
+        self.message__ = arr        
         if arr[0] == 'root':
             for s in self.screens:
                 if s.name == arr[1]:
                     self.screen_module = s
                     if getattr(s.screen,'prepare', False):
                         s.screen.prepare()
                     return True            
@@ -246,14 +247,16 @@
 def f(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever() 
     
 async_thread = Thread(target=f, args=(loop,))
 async_thread.start()  
 
-p = {'level' : logging.WARNING}
-if hasattr(config, 'logfile'):
-    p['filename'] = config.logfile
-logging.basicConfig(format='%(asctime)s - %(message)s', **p)
+User.toolbar = []
+
+#Logging 
+format = "%(asctime)s - %(levelname)s - %(message)s"
+handlers = [logging.FileHandler(config.logfile), logging.StreamHandler()] if hasattr(config,'logfile') else []
+logging.basicConfig(level = logging.WARNING, format = format, handlers = handlers)
+
 
-
```

### Comparing `unigui-1.8.2/unigui/web/favicon.ico` & `unigui-1.8.3/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/css/423.a6a82bd4.css` & `unigui-1.8.3/unigui/web/css/310.054e803c.css`

 * *Files 18% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-047e5584]{display:flex;justify-content:center}.custom-caption[data-v-047e5584]{padding:5px!important}.web-camera-container[data-v-047e5584]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-047e5584]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-047e5584]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-047e5584]{opacity:1}.web-camera-container .camera-shoot[data-v-047e5584]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-047e5584]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-047e5584]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-047e5584]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-047e5584]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-047e5584]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-047e5584]{animation:preload-047e5584 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-047e5584]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-047e5584]:nth-child(3){animation-delay:.4s}@keyframes preload-047e5584{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-047e5584]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-75b994fc]{display:flex;justify-content:center}.custom-caption[data-v-75b994fc]{padding:5px!important}.web-camera-container[data-v-75b994fc]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-75b994fc]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-75b994fc]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-75b994fc]{opacity:1}.web-camera-container .camera-shoot[data-v-75b994fc]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-75b994fc]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-75b994fc]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-75b994fc]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-75b994fc]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-75b994fc]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-75b994fc]{animation:preload-75b994fc 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-75b994fc]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-75b994fc]:nth-child(3){animation-delay:.4s}@keyframes preload-75b994fc{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-75b994fc]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.8.2/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.8.3/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/icons/favicon-96x96.png` & `unigui-1.8.3/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/icons/favicon-16x16.png` & `unigui-1.8.3/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/icons/favicon-32x32.png` & `unigui-1.8.3/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/icons/favicon-128x128.png` & `unigui-1.8.3/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.8.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.8.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.8.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.8.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.8.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/js/423.0ad6769b.js` & `unigui-1.8.3/unigui/web/js/310.1f9849f3.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [423], {
-        6423: (e, t, a) => {
+    [310], {
+        3310: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Xt
+                default: () => Gt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                     class: "q-pa-lg"
                 }, null, -1),
                 o = (0, l._)("div", {
@@ -188,30 +188,30 @@
             function M(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function $() {
+            function V() {
                 for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = w(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             K()
                         }))
                     }))
                 }))
             }
-            let V = (0, c.debounce)($, 200);
+            let $ = (0, c.debounce)(V, 200);
 
             function K(e) {
                 Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
-                const t = E(e),
-                    a = O(e);
+                const t = W(e),
+                    a = E(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = k[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = b[d];
                     for (let a of r.data.value.slice(1))
@@ -229,15 +229,15 @@
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function E(e) {
+            function W(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
@@ -295,15 +295,15 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function O(e) {
+            function E(e) {
                 e = null;
                 const t = e ? [e] : h.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
@@ -362,15 +362,15 @@
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
-            const W = (0, l.aZ)({
+            const O = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
                         C(["root", this.name])
                     }
                 },
                 props: {
@@ -385,21 +385,21 @@
                 }
             });
             var Q = a(4260),
                 H = a(3414),
                 U = a(2035),
                 N = a(4554),
                 F = a(2350),
-                T = a(7518),
-                P = a.n(T);
-            const I = (0, Q.Z)(W, [
+                P = a(7518),
+                T = a.n(P);
+            const I = (0, Q.Z)(O, [
                     ["render", d]
                 ]),
                 R = I;
-            P()(W, "components", {
+            T()(O, "components", {
                 QItem: H.Z,
                 QItemSection: U.Z,
                 QIcon: N.Z,
                 QItemLabel: F.Z
             });
             const L = {
                     key: 0,
@@ -504,15 +504,15 @@
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
                     _: 1
                 })
             }
             var ie = a(8880);
-            const oe = e => ((0, l.dD)("data-v-047e5584"), e = e(), (0, l.Cn)(), e),
+            const oe = e => ((0, l.dD)("data-v-75b994fc"), e = e(), (0, l.Cn)(), e),
                 ne = {
                     key: 4
                 },
                 de = ["width", "height"],
                 re = ["src"],
                 ce = {
                     key: 17,
@@ -562,15 +562,16 @@
                     y = (0, l.up)("linechart"),
                     w = (0, l.up)("q-input"),
                     b = (0, l.up)("q-tree"),
                     k = (0, l.up)("q-scroll-area"),
                     v = (0, l.up)("q-separator"),
                     x = (0, l.up)("q-uploader"),
                     C = (0, l.up)("cgraph"),
-                    q = (0, l.up)("q-tooltip");
+                    q = (0, l.up)("q-tooltip"),
+                    _ = (0, l.up)("q-spinner-puff");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
                     onClick: (0, ie.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
@@ -805,15 +806,31 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, l.kq)("", !0)])),
                     _: 1
-                }, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(g, {
+                }, 8, ["label", "icon", "onClick"])) : e.data.mode ? ((0, l.wg)(), (0, l.j4)(g, {
+                    key: 20,
+                    "no-caps": "",
+                    dense: "",
+                    onClick: e.sendValue
+                }, {
+                    default: (0, l.w5)((() => [(0, l.Wm)(_, {
+                        color: e.data.mode
+                    }, null, 8, ["color"]), e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
+                        key: 0,
+                        class: "text-body2"
+                    }, {
+                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
+                        _: 1
+                    })) : (0, l.kq)("", !0)])),
+                    _: 1
+                }, 8, ["onClick"])) : ((0, l.wg)(), (0, l.j4)(g, {
                     key: 19,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
                 }, {
                     default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
@@ -1277,50 +1294,50 @@
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
             var De = a(9267),
                 Me = a(4842),
-                $e = a(8870),
-                Ve = a(2165),
+                Ve = a(8870),
+                $e = a(2165),
                 Ke = a(8186),
-                Ee = a(2414),
-                Oe = a(3884),
-                We = a(5735),
+                We = a(2414),
+                Ee = a(3884),
+                Oe = a(5735),
                 Qe = a(7208);
             const He = (0, Q.Z)(Ze, [
                     ["render", Se]
                 ]),
                 Ue = He;
-            P()(Ze, "components", {
+            T()(Ze, "components", {
                 QTable: De.Z,
                 QInput: Me.Z,
                 QIcon: N.Z,
-                QTooltip: $e.Z,
-                QBtn: Ve.Z,
+                QTooltip: Ve.Z,
+                QBtn: $e.Z,
                 QTr: Ke.Z,
-                QTh: Ee.Z,
-                QTd: Oe.Z,
-                QCheckbox: We.Z,
+                QTh: We.Z,
+                QTd: Ee.Z,
+                QCheckbox: Oe.Z,
                 QSelect: Qe.Z
             });
             const Ne = ["nodes", "edges"];
 
             function Fe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
                 }, null, 12, Ne)
             }
-            var Te = a(2393),
-                Pe = a.n(Te);
-            const Ie = Pe().stylesheet().selector("node").css({
+            var Pe = a(2393),
+                Te = a.n(Pe);
+            const Ie = Te().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1380,15 +1397,15 @@
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Pe()({
+                        let e = Te()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1705,15 +1722,15 @@
                         C([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("update", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("changed", e.files[t - 1].name), V())
+                        t && (this.sendMessage("changed", e.files[t - 1].name), $())
                     },
                     sendValue() {
                         this.sendMessage("changed", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
@@ -1908,40 +1925,42 @@
             var yt = a(4027),
                 wt = a(9721),
                 bt = a(8886),
                 kt = a(8761),
                 vt = a(1232),
                 xt = a(5551),
                 Ct = a(5869),
-                qt = a(1745);
-            const _t = (0, Q.Z)(ft, [
+                qt = a(1745),
+                _t = a(8430);
+            const jt = (0, Q.Z)(ft, [
                     ["render", Ce],
-                    ["__scopeId", "data-v-047e5584"]
+                    ["__scopeId", "data-v-75b994fc"]
                 ]),
-                jt = _t;
-            P()(ft, "components", {
+                St = jt;
+            T()(ft, "components", {
                 QImg: yt.Z,
                 QIcon: N.Z,
                 QSelect: Qe.Z,
                 QBadge: wt.Z,
-                QCheckbox: We.Z,
+                QCheckbox: Oe.Z,
                 QToggle: bt.Z,
-                QBtn: Ve.Z,
+                QBtn: $e.Z,
                 QBtnToggle: kt.Z,
                 QInput: Me.Z,
                 QScrollArea: vt.Z,
                 QTree: xt.Z,
                 QSeparator: Ct.Z,
                 QUploader: qt.Z,
-                QTooltip: $e.Z
+                QTooltip: Ve.Z,
+                QSpinnerPuff: _t.Z
             });
-            const St = (0, l.aZ)({
+            const zt = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: jt
+                    element: St
                 },
                 data() {
                     return {
                         styleSize: y,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -2012,51 +2031,51 @@
                 },
                 watch: {
                     data(e) {
                         g && console.log("data update", this.name), this.styleSize = y, b[this.name] = this, this.expanding && (k[this.fullname] = this)
                     }
                 }
             });
-            var zt = a(151);
-            const At = (0, Q.Z)(St, [
+            var At = a(151);
+            const Zt = (0, Q.Z)(zt, [
                     ["render", se]
                 ]),
-                Zt = At;
-            P()(St, "components", {
-                QCard: zt.Z,
+                Dt = Zt;
+            T()(zt, "components", {
+                QCard: At.Z,
                 QIcon: N.Z,
                 QScrollArea: vt.Z
             });
-            const Dt = (0, l.aZ)({
+            const Mt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: Zt
+                        block: Dt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
                                     K()
                                 }))
                             }))
                         }))
                     }
                 }),
-                Mt = (0, Q.Z)(Dt, [
+                Vt = (0, Q.Z)(Mt, [
                     ["render", X]
                 ]),
-                $t = Mt,
-                Vt = {
+                $t = Vt,
+                Kt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Kt(e, t, a, i, o, n) {
+            function Wt(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -2072,15 +2091,15 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Vt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Kt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
@@ -2089,15 +2108,15 @@
             }
             const Et = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Zt
+                    block: Dt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -2114,28 +2133,28 @@
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
             var Ot = a(5926),
-                Wt = a(2025);
-            const Qt = (0, Q.Z)(Et, [
-                    ["render", Kt]
+                Qt = a(2025);
+            const Ht = (0, Q.Z)(Et, [
+                    ["render", Wt]
                 ]),
-                Ht = Qt;
-            P()(Et, "components", {
+                Ut = Ht;
+            T()(Et, "components", {
                 QDialog: Ot.Z,
-                QCard: zt.Z,
+                QCard: At.Z,
                 QItemLabel: F.Z,
-                QSpace: Wt.Z,
-                QBtn: Ve.Z
+                QSpace: Qt.Z,
+                QBtn: $e.Z
             });
-            let Ut = null;
-            const Nt = (0, l.aZ)({
+            let Nt = null;
+            const Ft = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         tooldata: {
@@ -2147,15 +2166,15 @@
                             blocks: []
                         }
                     }
                 },
                 components: {
                     menubar: R,
                     zone: $t,
-                    element: jt
+                    element: St
                 },
                 created() {
                     v(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
@@ -2163,23 +2182,23 @@
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         C(["root", e])
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), V()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), $()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ht
+                                component: Ut
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -2198,25 +2217,25 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Ut ? (l = {
+                        "progress" == t ? null == Nt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Ut = this.$q.notify(l)) : null == e ? (Ut(), Ut = null) : (l = {
+                        }, Nt = this.$q.notify(l)) : null == e ? (Nt(), Nt = null) : (l = {
                             caption: e
-                        }, Ut(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Nt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
@@ -2229,49 +2248,49 @@
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ht, t.componentProps = {
+                            t.component = Ut, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if ("answer" == e.type) D(e);
                         else {
                             e.updates && Z(e.updates);
                             let t = !1;
-                            ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), t = !0), t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
+                            ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), t = !0), t || e.updates || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Ut && "progress" != e.type && this.notify(null, "progress")
+                        Nt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var Ft = a(9214),
+            var Pt = a(9214),
                 Tt = a(3812),
-                Pt = a(9570),
-                It = a(7547),
-                Rt = a(3269),
-                Lt = a(2652),
-                Bt = a(4379);
-            const Yt = (0, Q.Z)(Nt, [
+                It = a(9570),
+                Rt = a(7547),
+                Lt = a(3269),
+                Bt = a(2652),
+                Yt = a(4379);
+            const Xt = (0, Q.Z)(Ft, [
                     ["render", n]
                 ]),
-                Xt = Yt;
-            P()(Nt, "components", {
-                QLayout: Ft.Z,
+                Gt = Xt;
+            T()(Ft, "components", {
+                QLayout: Pt.Z,
                 QHeader: Tt.Z,
-                QToolbar: Pt.Z,
-                QBtn: Ve.Z,
+                QToolbar: It.Z,
+                QBtn: $e.Z,
                 QItemLabel: F.Z,
-                QTabs: It.Z,
-                QTab: Rt.Z,
-                QPageContainer: Lt.Z,
-                QPage: Bt.Z
+                QTabs: Rt.Z,
+                QTab: Lt.Z,
+                QPageContainer: Bt.Z,
+                QPage: Yt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.8.2/unigui/web/js/430.591e9a73.js` & `unigui-1.8.3/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/js/app.eb412190.js` & `unigui-1.8.3/unigui/web/js/app.8ade4146.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(423)]).then(r.bind(r, 6423)),
+                        component: () => Promise.all([r.e(736), r.e(310)]).then(r.bind(r, 3310)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function b(e, t) {
+                async function g(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var g = r(6417),
+                var b = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: g.Z,
+                            Notify: b.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            423: "0ad6769b",
+            310: "1f9849f3",
             430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            423: "a6a82bd4",
+            310: "054e803c",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                423: 1
+                310: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.8.2/unigui/web/js/vendor.e1e2597e.js` & `unigui-1.8.3/unigui/web/js/vendor.f354d0dd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4698,15 +4698,15 @@
             n.d(t, {
                 Z: () => y
             });
             var r = n(3673),
                 i = n(1959),
                 o = n(8880),
                 a = n(4554),
-                s = n(9754),
+                s = n(6833),
                 l = n(6489),
                 u = n(3646),
                 c = n(908),
                 d = n(7657),
                 h = n(4716),
                 f = n(1436);
             const {
@@ -5807,15 +5807,15 @@
             "use strict";
             n.d(t, {
                 Z: () => h
             });
             var r = n(1959),
                 i = n(3673),
                 o = n(8880),
-                a = n(9754);
+                a = n(6833);
             const s = {
                 ratio: [String, Number]
             };
 
             function l(e, t) {
                 return (0, i.Fl)((() => {
                     const n = Number(e.ratio || (void 0 !== t ? t.value : void 0));
@@ -8804,50 +8804,36 @@
                 a = (0, i.L)({
                     name: "QSpace",
                     setup() {
                         return () => o
                     }
                 })
         },
-        9754: (e, t, n) => {
+        6833: (e, t, n) => {
             "use strict";
             n.d(t, {
-                Z: () => l
+                Z: () => a
             });
             var r = n(3673),
-                i = n(2417);
-            const o = {
-                size: {
-                    type: [Number, String],
-                    default: "1em"
-                },
-                color: String
-            };
-
-            function a(e) {
-                return {
-                    cSize: (0, r.Fl)((() => e.size in i.Ok ? `${i.Ok[e.size]}px` : e.size)),
-                    classes: (0, r.Fl)((() => "q-spinner" + (e.color ? ` text-${e.color}` : "")))
-                }
-            }
-            var s = n(908);
-            const l = (0, s.L)({
+                i = n(4633),
+                o = n(908);
+            const a = (0, o.L)({
                 name: "QSpinner",
                 props: {
-                    ...o,
+                    ...i.G,
                     thickness: {
                         type: Number,
                         default: 5
                     }
                 },
                 setup(e) {
                     const {
                         cSize: t,
                         classes: n
-                    } = a(e);
+                    } = (0, i.Z)(e);
                     return () => (0, r.h)("svg", {
                         class: n.value + " q-spinner-mat",
                         width: t.value,
                         height: t.value,
                         viewBox: "25 25 50 50"
                     }, [(0, r.h)("circle", {
                         class: "path",
@@ -8858,14 +8844,113 @@
                         stroke: "currentColor",
                         "stroke-width": e.thickness,
                         "stroke-miterlimit": "10"
                     })])
                 }
             })
         },
+        8430: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                Z: () => s
+            });
+            var r = n(3673),
+                i = n(4633),
+                o = n(908);
+            const a = [(0, r.h)("g", {
+                    fill: "none",
+                    "fill-rule": "evenodd",
+                    "stroke-width": "2"
+                }, [(0, r.h)("circle", {
+                    cx: "22",
+                    cy: "22",
+                    r: "1"
+                }, [(0, r.h)("animate", {
+                    attributeName: "r",
+                    begin: "0s",
+                    dur: "1.8s",
+                    values: "1; 20",
+                    calcMode: "spline",
+                    keyTimes: "0; 1",
+                    keySplines: "0.165, 0.84, 0.44, 1",
+                    repeatCount: "indefinite"
+                }), (0, r.h)("animate", {
+                    attributeName: "stroke-opacity",
+                    begin: "0s",
+                    dur: "1.8s",
+                    values: "1; 0",
+                    calcMode: "spline",
+                    keyTimes: "0; 1",
+                    keySplines: "0.3, 0.61, 0.355, 1",
+                    repeatCount: "indefinite"
+                })]), (0, r.h)("circle", {
+                    cx: "22",
+                    cy: "22",
+                    r: "1"
+                }, [(0, r.h)("animate", {
+                    attributeName: "r",
+                    begin: "-0.9s",
+                    dur: "1.8s",
+                    values: "1; 20",
+                    calcMode: "spline",
+                    keyTimes: "0; 1",
+                    keySplines: "0.165, 0.84, 0.44, 1",
+                    repeatCount: "indefinite"
+                }), (0, r.h)("animate", {
+                    attributeName: "stroke-opacity",
+                    begin: "-0.9s",
+                    dur: "1.8s",
+                    values: "1; 0",
+                    calcMode: "spline",
+                    keyTimes: "0; 1",
+                    keySplines: "0.3, 0.61, 0.355, 1",
+                    repeatCount: "indefinite"
+                })])])],
+                s = (0, o.L)({
+                    name: "QSpinnerPuff",
+                    props: i.G,
+                    setup(e) {
+                        const {
+                            cSize: t,
+                            classes: n
+                        } = (0, i.Z)(e);
+                        return () => (0, r.h)("svg", {
+                            class: n.value,
+                            stroke: "currentColor",
+                            width: t.value,
+                            height: t.value,
+                            viewBox: "0 0 44 44",
+                            xmlns: "http://www.w3.org/2000/svg"
+                        }, a)
+                    }
+                })
+        },
+        4633: (e, t, n) => {
+            "use strict";
+            n.d(t, {
+                G: () => o,
+                Z: () => a
+            });
+            var r = n(3673),
+                i = n(2417);
+            const o = {
+                size: {
+                    type: [Number, String],
+                    default: "1em"
+                },
+                color: String
+            };
+
+            function a(e) {
+                return {
+                    cSize: (0, r.Fl)((() => e.size in i.Ok ? `${i.Ok[e.size]}px` : e.size)),
+                    classes: (0, r.Fl)((() => "q-spinner" + (e.color ? ` text-${e.color}` : "")))
+                }
+            }
+        },
         9267: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => re
             });
             n(71);
             var r = n(3673),
@@ -11207,15 +11292,15 @@
                         css: !1,
                         appear: e.appear,
                         onEnter: v,
                         onLeave: g
                     }, t.default)
                 }
             });
-            var c = n(9754),
+            var c = n(6833),
                 d = n(2236),
                 h = n(4716),
                 f = n(1436),
                 p = n(9085);
             const v = ["none", "strict", "leaf", "leaf-filtered"],
                 g = (0, l.L)({
                     name: "QTree",
@@ -11579,15 +11664,15 @@
                 Z: () => H
             });
             n(71), n(7965);
             var r = n(3673),
                 i = n(1959),
                 o = n(2165),
                 a = n(4554),
-                s = n(9754),
+                s = n(6833),
                 l = n(2417);
             const u = {
                 ...l.LU,
                 min: {
                     type: Number,
                     default: 0
                 },
@@ -12811,15 +12896,15 @@
                 tL: () => O
             });
             var r = n(3673),
                 i = n(1959),
                 o = n(8880),
                 a = n(4688),
                 s = n(4554),
-                l = n(9754),
+                l = n(6833),
                 u = n(2236),
                 c = (n(71), n(2547));
 
             function d({
                 validate: e,
                 resetValidation: t,
                 requiresQForm: n
@@ -14674,15 +14759,15 @@
                                 dense: e.dense,
                                 keepColor: void 0 === t.keepColor ? e.keepColor : t.keepColor,
                                 "onUpdate:modelValue": c
                             }, o)])
                         })))
                     }
                 });
-            var E = n(9754),
+            var E = n(6833),
                 I = n(1436),
                 P = n(2162);
             const A = (0, l.L)({
                 name: "DialogPlugin",
                 props: {
                     ...g.S,
                     title: String,
@@ -15002,15 +15087,15 @@
                             class: "q-avatar__content row flex-center overflow-hidden",
                             style: o.value
                         }, (0, u.pf)(t.default, s))])
                     }
                 }
             });
             var d = n(2165),
-                h = n(9754),
+                h = n(6833),
                 f = (n(4716), n(8144)),
                 p = n(8242),
                 v = n(2162);
             let g = 0;
             const m = {},
                 y = {},
                 b = {},
@@ -37958,15 +38043,15 @@
                         var t = e.getData(),
                             n = e.getModel("lineStyle").getLineStyle();
                         n && !n.stroke && (n.stroke = t.getVisual("style").fill), t.setVisual("legendLineStyle", n)
                     }
                 }), e.registerProcessor(e.PRIORITY.PROCESSOR.STATISTIC, bt("line"))
             }
         },
-        9806: (e, t, n) => {
+        6423: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => A
             });
             var r = n(3223),
                 i = n(841),
                 o = n(391),
@@ -39253,15 +39338,15 @@
             });
             var r = n(3223),
                 i = n(841),
                 o = n(850),
                 a = n(5162),
                 s = n(1926),
                 l = n(5226),
-                u = n(9806),
+                u = n(6423),
                 c = n(5865);
 
             function d(e) {
                 var t, n = e.get("type"),
                     r = e.getModel(n + "Style");
                 return "line" === n ? (t = r.getLineStyle(), t.fill = null) : "shadow" === n && (t = r.getAreaStyle(), t.stroke = null), t
             }
@@ -41741,15 +41826,15 @@
                     return r - e + t
                 }
             }
             const pe = ue;
             var ve = n(841),
                 ge = n(391),
                 me = n(4740),
-                ye = n(9806),
+                ye = n(6423),
                 be = n(4956),
                 _e = (0, d.Yf)();
 
             function xe(e, t, n, r) {
                 var i = n.axis;
                 if (!i.scale.isBlank()) {
                     var o = n.getModel("splitArea"),
```

### Comparing `unigui-1.8.2/unigui/web/js/193.283445be.js` & `unigui-1.8.3/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui/web/index.html` & `unigui-1.8.3/unigui/web/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.e1e2597e.js></script><script defer src=js/app.eb412190.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.f354d0dd.js></script><script defer src=js/app.8ade4146.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.8.2/LICENSE` & `unigui-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/setup.py` & `unigui-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.8.2',      
+      version='1.8.3',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.8.2/PKG-INFO` & `unigui-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.2
+Version: 1.8.3
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.8.2/README.md` & `unigui-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.8.2/unigui.egg-info/PKG-INFO` & `unigui-1.8.3/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.2
+Version: 1.8.3
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.8.2/unigui.egg-info/SOURCES.txt` & `unigui-1.8.3/unigui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 unigui/__init__.py
+unigui/autotest.py
 unigui/guielements.py
 unigui/reloader.py
 unigui/server.py
 unigui/users.py
 unigui/utils.py
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/423.a6a82bd4.css
+unigui/web/css/310.054e803c.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,11 +29,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/423.0ad6769b.js
+unigui/web/js/310.1f9849f3.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.eb412190.js
-unigui/web/js/vendor.e1e2597e.js
+unigui/web/js/app.8ade4146.js
+unigui/web/js/vendor.f354d0dd.js
```

