# Comparing `tmp/htagweb-0.3.0.tar.gz` & `tmp/htagweb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.3.0.tar", max compression
+gzip compressed data, was "htagweb-0.3.1.tar", max compression
```

## Comparing `htagweb-0.3.0.tar` & `htagweb-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-14 07:56:28.840930 htagweb-0.3.0/LICENSE
--rw-r--r--   0        0        0     2985 2023-07-14 07:56:28.840930 htagweb-0.3.0/README.md
--rw-r--r--   0        0        0     9938 2023-07-14 07:56:29.124932 htagweb-0.3.0/htagweb/__init__.py
--rw-r--r--   0        0        0     2225 2023-07-14 07:56:28.840930 htagweb-0.3.0/htagweb/crypto.py
--rw-r--r--   0        0        0     3732 2023-07-14 07:56:28.840930 htagweb-0.3.0/htagweb/manager.py
--rw-r--r--   0        0        0     5078 2023-07-14 07:56:28.840930 htagweb-0.3.0/htagweb/uidprocess.py
--rw-r--r--   0        0        0     1124 2023-07-14 07:56:29.124932 htagweb-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4187 1970-01-01 00:00:00.000000 htagweb-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-16 16:23:13.148472 htagweb-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3148 2023-07-16 16:23:13.148472 htagweb-0.3.1/README.md
+-rw-r--r--   0        0        0     9938 2023-07-16 16:23:13.520501 htagweb-0.3.1/htagweb/__init__.py
+-rw-r--r--   0        0        0     2225 2023-07-16 16:23:13.148472 htagweb-0.3.1/htagweb/crypto.py
+-rw-r--r--   0        0        0     3732 2023-07-16 16:23:13.148472 htagweb-0.3.1/htagweb/manager.py
+-rw-r--r--   0        0        0     5152 2023-07-16 16:23:13.148472 htagweb-0.3.1/htagweb/uidprocess.py
+-rw-r--r--   0        0        0     1124 2023-07-16 16:23:13.520501 htagweb-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 htagweb-0.3.1/PKG-INFO
```

### Comparing `htagweb-0.3.0/LICENSE` & `htagweb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.0/README.md` & `htagweb-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,18 @@
 
 The concepts are the same :
 
  - one user can run only one instance of an htag app at one time (like in desktop mode).
  - All user processes are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
  - the "session" live as long as the server live (may not be a problem on many hosting service (where they shutdown the server after inactivities))
 
+## architecture
+
+Here is a rapid [map](https://www.tldraw.com/s/v2_c_0z8CUdwoKgrIjBa29yeO7?viewport=228%2C-15%2C1920%2C976&page=page%3AlnBx9GrxTdcdrdgOk-s83) ;-)
+
 ## Roadmap / futur
 
 - ? replace starlette by fastapi ?
 - better logging !!!!
 - more parameters (session size, etc ...)
 - parano mode
 - perhaps a bi-modal version (use ws, and fallback to http when ws com error)
```

### Comparing `htagweb-0.3.0/htagweb/__init__.py` & `htagweb-0.3.1/htagweb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.3.0" # auto updated
+__version__ = "0.3.1" # auto updated
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
 - concept of an htag app application server (manager), which communicate with child process, with queue
 - Htag Apps runned in a process, per user (real isolation!)
```

### Comparing `htagweb-0.3.0/htagweb/crypto.py` & `htagweb-0.3.1/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.0/htagweb/manager.py` & `htagweb-0.3.1/htagweb/manager.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.3.0/htagweb/uidprocess.py` & `htagweb-0.3.1/htagweb/uidprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,27 @@
         #==========================================================
         async def ht_create(self, fqn,js,init_params=None,renew=False):        # -> str
         #==========================================================
             """ HRenderer creator """
             session["ht_create"]="here"
             if init_params is None : init_params=((),{})
 
-            #--------------------------- fqn -> module, name
-            names = fqn.split(".")
-            modulename,name=".".join(names[:-1]), names[-1]
-            module=importlib.import_module(modulename)
-            #---------------------------
-            htClass = getattr(module,name)
-
             hr=HTS.get(fqn)
             if renew or (hr is None) or str(init_params)!=str(hr.init):
                 ##HRenderer(tagClass: type, js:str, exit_callback:Optional[Callable]=None, init= ((),{}), fullerror=False, statics=[], session=None ):
+
+                #--------------------------- fqn -> module, name
+                names = fqn.split(".")
+                modulename,name=".".join(names[:-1]), names[-1]
+                module=importlib.import_module(modulename)
+                module=importlib.reload(module)
+                #---------------------------
+                htClass = getattr(module,name)
+
+
                 hr=HRenderer( htClass,
                         js=js,
                         session=session,
                         init= init_params,
                 )
                 HTS[fqn] = hr
             return str(hr)
```

### Comparing `htagweb-0.3.0/pyproject.toml` & `htagweb-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.3.0" # auto-updated
+version = "0.3.1" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.3.0/PKG-INFO` & `htagweb-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.3.0
+Version: 0.3.1
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -60,14 +60,18 @@
 
 The concepts are the same :
 
  - one user can run only one instance of an htag app at one time (like in desktop mode).
  - All user processes are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
  - the "session" live as long as the server live (may not be a problem on many hosting service (where they shutdown the server after inactivities))
 
+## architecture
+
+Here is a rapid [map](https://www.tldraw.com/s/v2_c_0z8CUdwoKgrIjBa29yeO7?viewport=228%2C-15%2C1920%2C976&page=page%3AlnBx9GrxTdcdrdgOk-s83) ;-)
+
 ## Roadmap / futur
 
 - ? replace starlette by fastapi ?
 - better logging !!!!
 - more parameters (session size, etc ...)
 - parano mode
 - perhaps a bi-modal version (use ws, and fallback to http when ws com error)
```

