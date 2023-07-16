# Comparing `tmp/understar-0.2.3.tar.gz` & `tmp/understar-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-0.2.3.tar", last modified: Thu Jul 13 00:38:08 2023, max compression
+gzip compressed data, was "understar-0.2.4.tar", last modified: Sun Jul 16 05:00:25 2023, max compression
```

## Comparing `understar-0.2.3.tar` & `understar-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.267398 understar-0.2.3/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-0.2.3/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-13 00:38:08.267279 understar-0.2.3/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-0.2.3/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-13 00:38:08.267448 understar-0.2.3/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1222 2023-07-13 00:34:17.000000 understar-0.2.3/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.263443 understar-0.2.3/understar/
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-12 03:28:50.000000 understar-0.2.3/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.264497 understar-0.2.3/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       17 2023-07-12 03:20:28.000000 understar-0.2.3/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.266995 understar-0.2.3/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-0.2.3/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5614 2023-07-12 03:35:46.000000 understar-0.2.3/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-0.2.3/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-0.2.3/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-0.2.3/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2402 2023-06-25 03:39:17.000000 understar-0.2.3/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-0.2.3/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     4978 2023-07-12 03:07:24.000000 understar-0.2.3/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    30889 2023-07-12 09:33:55.000000 understar-0.2.3/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-13 00:38:08.264336 understar-0.2.3/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      505 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-13 00:38:08.000000 understar-0.2.3/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.122559 understar-0.2.4/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-0.2.4/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-16 05:00:25.122293 understar-0.2.4/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-0.2.4/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-16 05:00:25.122615 understar-0.2.4/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1222 2023-07-16 04:54:52.000000 understar-0.2.4/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.114992 understar-0.2.4/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-12 03:28:50.000000 understar-0.2.4/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116239 understar-0.2.4/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-0.2.4/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116561 understar-0.2.4/understar/system/app/
+-rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-0.2.4/understar/system/app/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116900 understar-0.2.4/understar/system/app/config/
+-rw-r--r--   0 maxence    (501) staff       (20)    19996 2023-07-16 04:54:09.000000 understar-0.2.4/understar/system/app/config/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.117883 understar-0.2.4/understar/system/app/config/apt/
+-rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-0.2.4/understar/system/app/config/apt/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-16 04:54:11.000000 understar-0.2.4/understar/system/app/config/apt/install.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-16 04:54:12.000000 understar-0.2.4/understar/system/app/config/apt/uninstall.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.118108 understar-0.2.4/understar/system/app/maintenance/
+-rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-16 04:54:14.000000 understar-0.2.4/understar/system/app/maintenance/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.121731 understar-0.2.4/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-0.2.4/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5512 2023-07-13 02:32:11.000000 understar-0.2.4/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-0.2.4/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-0.2.4/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-0.2.4/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2402 2023-06-25 03:39:17.000000 understar-0.2.4/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-0.2.4/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     4978 2023-07-12 03:07:24.000000 understar-0.2.4/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    31301 2023-07-16 04:52:59.000000 understar-0.2.4/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116111 understar-0.2.4/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      755 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/top_level.txt
```

### Comparing `understar-0.2.3/LICENSE.md` & `understar-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-0.2.3/PKG-INFO` & `understar-0.2.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 0.2.3
+Version: 0.2.4
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-0.2.3/setup.py` & `understar-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='understar',
-    version="0.2.3",
+    version="0.2.4",
     url='https://github.com/GalTechDev/UnderStar-OS',
     download_url='https://github.com/GalTechDev/UnderStar-OS/tarball/master',
     license='MIT',
     author='GalTech',
     author_email='poussigalitv@gmail.com',
     description='A discord bot framewrok',
     long_description=long_description,
```

### Comparing `understar-0.2.3/understar/system/lib/app.py` & `understar-0.2.4/understar/system/lib/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,20 +95,17 @@
         else:
             raise Exception
 
     async def change_presence(self, activity, status):
         """"""
         await self.client.change_presence(activity=activity, status=status)
         
-    def get_apps(self, sys: bool = False) -> dict:
+    def get_apps(self) -> dict:
         """"""
-        if sys:
-            all_app=import_module("system.app")
-        else: 
-            all_app=import_module("app")
+        all_app=import_module("app")
         return all_app
 
 class App:
     """"""
     def __init__(self) -> None:
         self.commands = []
         self.slashs = []
```

### Comparing `understar-0.2.3/understar/system/lib/com.py` & `understar-0.2.4/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.3/understar/system/lib/event.py` & `understar-0.2.4/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.3/understar/system/lib/save.py` & `understar-0.2.4/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.3/understar/system/lib/store.py` & `understar-0.2.4/understar/system/lib/store.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.3/understar/system/lib/utils.py` & `understar-0.2.4/understar/system/lib/utils.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.3/understar/understar.py` & `understar-0.2.4/understar/understar.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from itertools import cycle
 from pathlib import Path
 import os
 import discord
 import time
 import sys
 from .system.lib import *
+from .system import app as sys_app
 import asyncio
 import json
 
 DOWNLOAD_FOLDER = "download"
 SYS_FOLDER = "system"
 TOKEN_FOLDER = "token"
 SAVE_FOLDER = "save"
@@ -19,14 +20,16 @@
 APP_FOLDER = "app"
 BOT_TOKEN_PATH = f"{TOKEN_FOLDER}/bot_token"
 PREFIX = "?"
 CODING = "utf-8"
 
 programmer = os.path.basename(sys.argv[0])
 
+
+
 class OS:
     
     Lib = App()
     vals = [DOWNLOAD_FOLDER, TOKEN_FOLDER, SAVE_FOLDER, SAVE_APP_FOLDER, APP_FOLDER]
     for name in vals:
         Path(name).mkdir(exist_ok=True)
         
@@ -42,15 +45,15 @@
     timer = time.time()
        
     def start(self):
         self.client.run(self.BOT_TOKEN)
          
     async def import_apps(self, sys :bool=False) -> None:
         """"""
-        for app_name,app in self.Lib.get_apps(sys).items():
+        for app_name,app in (self.Lib.get_apps().items() if not sys else sys_app.all_app.items()):
             print(f"\n * IMPORT {app_name}: ")
 
             app.Lib.init(self.client, discord_tasks)
             app.Lib.set_app_name(app_name)
             if not os.path.exists(os.path.join(app.Lib.save.save_path, app_name)):
                 os.mkdir(os.path.join(app.Lib.save.save_path, app_name))
 
@@ -78,15 +81,15 @@
                         error_lst.append(error)
             except Exception as error:
                 print(error)
 
             print(f" * - Task : {loaded} loaded | {errors} error : {error_lst}")
 
             # Command & Slash
-            if len(self.Lib.store.get_guilds_installed(app_name)) > 0 :
+            if len(self.Lib.store.get_guilds_installed(app_name)) > 0 or sys:
                 
                 # Command
                 loaded = 0
                 errors = 0
                 error_lst=[]    
 
                 for command in app.Lib.app.commands:
@@ -167,15 +170,15 @@
             embed.set_author(name=f"{ctx.user.name} use {ctx.command}", icon_url=ctx.user.avatar.url)
             embed.add_field(name="ctx info :", value=ctx.data.items())
         embed.add_field(name="error :", value=str(error))
         embed.add_field(name="error :", value=str(error))
         if self.client.owner_id==None:
             return
         user = await self.client.fetch_user(self.client.owner_id)
-        user.send(embed=embed)
+        await user.send(embed=embed)
         
     ################################################################
     #                             INIT                             #
     ################################################################
     
     def __init__(self, token: str=None) -> None:
         if not token:
@@ -224,19 +227,23 @@
         @client.command(name="os-help", aliases=["help"], help="Pour avoir ce message")
         async def help(ctx:discord_commands.context.Context,*args):
             if args==():
                 await ctx.send(embeds=self.get_help(ctx))
             else :
                 if args[0] in Lib.get_apps().keys():
                     sys_com = False
-                elif args[0] in Lib.get_apps(True).keys():
+                    com = Lib.get_apps()
+                elif args[0] in sys_app.all_app:
                     sys_com = True
+                    com = sys_app.all_app
+                else:
+                    return
                 if len(args)==1:
                     try:
-                        await Lib.get_apps(sys_com)[args[0]].Lib.help(ctx)
+                        await com[args[0]].Lib.help(ctx)
                     except Exception as error:
                         if types(error) == AttributeError:
                             await ctx.send(content=f"L'application `{args[0]}` n'a pas de fonction d'aide")
                         else:
                             await ctx.send(content=f"La fonction d'aide de l'application `{args[0]}` ne fonctionne pas. Merci de contacter son développeur.")
                 else:
                     if f"{args[0]}-{args[1]}" in client.all_commands.keys():
@@ -257,15 +264,15 @@
                     except Exception as error:
                         print(error)
 
         # ---------------------------------- EVENTS ------------------------------------
 
         #@terminal()
         async def manage_event(command, *args, **kwargs):
-            for app in list(Lib.get_apps().values()) + list(Lib.get_apps(True).values()):
+            for app in list(Lib.get_apps().values()) + list(sys_app.all_app.values()):
                 if app:
                     data = getattr(app.Lib.event, command)
                     await data(*args, **kwargs)
                     if app.Lib.app.fusioned:
                         for sub_app in app.Lib.app.fusioned_module:
                             data = getattr(sub_app.Lib.event, command)
                             await data(*args, **kwargs)
@@ -284,14 +291,18 @@
             await manage_event("on_app_command_error", ctx, error)
 
             if isinstance(error, discord.app_commands.CheckFailure):
                 await ctx.response.send_message('Tu ne remplis pas les conditions pour executer cette commande.', ephemeral=True)
             elif isinstance(error, discord.app_commands.BotMissingPermissions):
                 await ctx.response.send_message('Le bot ne peut pas executer cette commande car il lui manque des autorisations. Merci de contacter le STAFF', ephemeral=True)
             else:
+                try:
+                    await ctx.response.send_message(f"Data :\n{ctx.data}\nError :\n{error}", ephemeral = True)
+                except:
+                    print(f"Data :\n{ctx.data}\nError :\n{error}")
                 await self.send_error(ctx, error)
                 
 
         #AutoMod
         @client.event
         async def on_automod_rule_create(rule):
             await manage_event("on_automod_rule_create", rule)
```

### Comparing `understar-0.2.3/understar.egg-info/PKG-INFO` & `understar-0.2.4/understar.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 0.2.3
+Version: 0.2.4
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

