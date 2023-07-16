# Comparing `tmp/revealjs-0.0.7.tar.gz` & `tmp/revealjs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revealjs-0.0.7.tar", last modified: Sun Jul 16 05:24:20 2023, max compression
+gzip compressed data, was "revealjs-0.0.8.tar", last modified: Sun Jul 16 05:46:53 2023, max compression
```

## Comparing `revealjs-0.0.7.tar` & `revealjs-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:24:20.776866 revealjs-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 05:24:20.776866 revealjs-0.0.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:24:20.776866 revealjs-0.0.7/revealjs/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-16 04:40:54.000000 revealjs-0.0.7/revealjs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      231 2023-07-16 05:22:56.000000 revealjs-0.0.7/revealjs/interface.py
--rw-rw-r--   0 root         (0) root         (0)    17579 2023-07-16 05:22:16.000000 revealjs-0.0.7/revealjs/reveal_js.py
--rw-rw-r--   0 root         (0) root         (0)     4536 2023-07-16 05:23:37.000000 revealjs-0.0.7/revealjs/slide.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:24:20.776866 revealjs-0.0.7/revealjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 05:24:20.000000 revealjs-0.0.7/revealjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-16 05:24:20.000000 revealjs-0.0.7/revealjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 05:24:20.000000 revealjs-0.0.7/revealjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 05:24:20.000000 revealjs-0.0.7/revealjs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-16 05:24:20.000000 revealjs-0.0.7/revealjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 05:24:20.000000 revealjs-0.0.7/revealjs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 05:24:20.776866 revealjs-0.0.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      562 2023-07-16 05:12:07.000000 revealjs-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:46:53.539635 revealjs-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 05:46:53.539635 revealjs-0.0.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:46:53.539635 revealjs-0.0.8/revealjs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-16 05:43:02.000000 revealjs-0.0.8/revealjs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      186 2023-07-16 05:43:02.000000 revealjs-0.0.8/revealjs/interface.py
+-rw-rw-r--   0 root         (0) root         (0)    17704 2023-07-16 05:43:02.000000 revealjs-0.0.8/revealjs/reveal_js.py
+-rw-rw-r--   0 root         (0) root         (0)     4526 2023-07-16 05:43:02.000000 revealjs-0.0.8/revealjs/slide.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 05:46:53.539635 revealjs-0.0.8/revealjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-07-16 05:46:53.000000 revealjs-0.0.8/revealjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-16 05:46:53.000000 revealjs-0.0.8/revealjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 05:46:53.000000 revealjs-0.0.8/revealjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-16 05:46:53.000000 revealjs-0.0.8/revealjs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-16 05:46:53.000000 revealjs-0.0.8/revealjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-16 05:46:53.000000 revealjs-0.0.8/revealjs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 05:46:53.539635 revealjs-0.0.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2023-07-16 05:12:07.000000 revealjs-0.0.8/setup.py
```

### Comparing `revealjs-0.0.7/PKG-INFO` & `revealjs-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Reveal.js Presentation Builder Inspired By revealjs
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.7/README.md` & `revealjs-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.7/revealjs/reveal_js.py` & `revealjs-0.0.8/revealjs/reveal_js.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,27 +186,31 @@
                             lambda file_ext: file_ext in str(answers.get(question)),
                             [".md", ".adoc", ".asciidoc"],
                         )
                     )
                 )
                 >= 1
             ):
-                create_file(get_sample_adocfile(), file_path=answers.get(question))
+                file_path = os.path.join(project_name, answers.get(question))
+                create_file(
+                    get_sample_adocfile(),
+                    file_path=file_path,
+                )
         if question == "plugins":
             value = answers.get(question)
             if value == "all":
                 USER_PLUGIN_CONFIG = USER_PLUGIN_CONFIG[:-2]
             else:
                 # USER_PLUGIN_CONFIG.append(value)
                 pass
 
         else:
-            for _, value in answers.items():
+            for key, value in answers.items():
                 if value == "yes":
-                    os.makedirs(os.path.join(project_name, value), exist_ok=True)
+                    os.makedirs(os.path.join(project_name, key), exist_ok=True)
 
             return
 
 
 def install_script(command):
     try:
         return run(command, shell=True)
```

### Comparing `revealjs-0.0.7/revealjs/slide.adoc` & `revealjs-0.0.8/revealjs/slide.adoc`

 * *Files 2% similar despite different names*

```diff
@@ -292,8 +292,8 @@
 
 === Genarate as pdf 
 
 Please Press ctrl + p
 
 === Bye Go through the link i have previous given.
 
-    Buy Me Coffee (:) link::gunag5127@gmail.com[guna]
+* Buy Me Coffee :)  **gunag5127@gmail.com**
```

### Comparing `revealjs-0.0.7/revealjs.egg-info/PKG-INFO` & `revealjs-0.0.8/revealjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Reveal.js Presentation Builder Inspired By revealjs
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.7/setup.py` & `revealjs-0.0.8/setup.py`

 * *Files identical despite different names*

