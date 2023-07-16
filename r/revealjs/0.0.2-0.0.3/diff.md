# Comparing `tmp/revealjs-0.0.2.tar.gz` & `tmp/revealjs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revealjs-0.0.2.tar", last modified: Sat Jul 15 18:03:45 2023, max compression
+gzip compressed data, was "revealjs-0.0.3.tar", last modified: Sat Jul 15 18:19:30 2023, max compression
```

## Comparing `revealjs-0.0.2.tar` & `revealjs-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:03:45.106750 revealjs-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1429 2023-07-15 18:03:45.106750 revealjs-0.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:03:45.106750 revealjs-0.0.2/revealjs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-15 17:47:50.000000 revealjs-0.0.2/revealjs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15520 2023-07-15 17:47:50.000000 revealjs-0.0.2/revealjs/reveal_js.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:03:45.106750 revealjs-0.0.2/revealjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1429 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      255 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 18:03:45.106750 revealjs-0.0.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      482 2023-07-15 18:00:50.000000 revealjs-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:19:30.354524 revealjs-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-07-15 18:19:30.354524 revealjs-0.0.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:19:30.354524 revealjs-0.0.3/revealjs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-15 17:47:50.000000 revealjs-0.0.3/revealjs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15646 2023-07-15 18:12:02.000000 revealjs-0.0.3/revealjs/reveal_js.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:19:30.354524 revealjs-0.0.3/revealjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-07-15 18:19:30.000000 revealjs-0.0.3/revealjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-15 18:19:30.000000 revealjs-0.0.3/revealjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 18:19:30.000000 revealjs-0.0.3/revealjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-15 18:19:30.000000 revealjs-0.0.3/revealjs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-15 18:19:30.000000 revealjs-0.0.3/revealjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 18:19:30.000000 revealjs-0.0.3/revealjs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 18:19:30.354524 revealjs-0.0.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      482 2023-07-15 18:00:50.000000 revealjs-0.0.3/setup.py
```

### Comparing `revealjs-0.0.2/PKG-INFO` & `revealjs-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reveal.js Presentation
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.2/README.md` & `revealjs-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.2/revealjs/reveal_js.py` & `revealjs-0.0.3/revealjs/reveal_js.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     return False if "yes" == prompt(when_fails).get("status") else True
 
 
 def create_template(status: bool = True):
     project_name = sys.argv[2] or "revealjs"
     if project_name:
         try:
-            os.makedirs(os.path.realpath(".") + project_name, exist_ok=not status)
+            os.makedirs(os.path.realpath(".") + f"/{project_name}", exist_ok=not status)
         except FileExistsError as e:
             print(f"\n\t NOTE : \n\t\t {e.args}")
             create_template(run_when_fails())
 
     prompt_list = [
         Text(
             "slide_name",
@@ -462,24 +462,26 @@
     for file in sys.argv:
         if file.strip().split(".")[-1] in ["adoc", "asciidoc", "md", "markdown"]:
             rst_files.append(file)
     return rst_files
 
 
 def main():
-    ACTIONS = {"create": create_template, "build": build}
-    action_name = sys.argv[1]
-    if action_name in ACTIONS.keys():
-        ACTIONS.get(action_name)()
-        print(f"""{action_name} START'S""")
-    else:
-        print(
-            "\n \n AS OF NOW WE PROVIDING TWO DIFFERENT SERVICES  \n\n "
-            + "".join("*\t {}\n" for _ in ACTIONS.keys()).format(*ACTIONS.keys())
-        )
-
+    try:
+        ACTIONS = {"create": create_template, "build": build}
+        action_name = sys.argv[1]
+        if action_name in ACTIONS.keys():
+            ACTIONS.get(action_name)()
+            print(f"""{action_name} START'S""")
+        else:
+            print(
+                "\n \n AS OF NOW WE PROVIDING TWO DIFFERENT SERVICES  \n\n "
+                + "".join("*\t {}\n" for _ in ACTIONS.keys()).format(*ACTIONS.keys())
+            )
+    except Exception as e:
+        print(f" Went's Wrong ... {e.args}")
 
 if __name__ == "__main__":
     """
     creating the index.html file from your asciidoc file
     """
     main()
```

### Comparing `revealjs-0.0.2/revealjs.egg-info/PKG-INFO` & `revealjs-0.0.3/revealjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reveal.js Presentation
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

