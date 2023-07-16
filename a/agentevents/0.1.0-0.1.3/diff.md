# Comparing `tmp/agentevents-0.1.0.tar.gz` & `tmp/agentevents-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentevents-0.1.0.tar", last modified: Sun Jul 16 02:46:53 2023, max compression
+gzip compressed data, was "agentevents-0.1.3.tar", last modified: Sun Jul 16 08:39:36 2023, max compression
```

## Comparing `agentevents-0.1.0.tar` & `agentevents-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:46:53.237284 agentevents-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 02:46:39.000000 agentevents-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-16 02:46:53.237284 agentevents-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-16 02:46:39.000000 agentevents-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:46:53.237284 agentevents-0.1.0/agentevents/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-16 02:46:39.000000 agentevents-0.1.0/agentevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-07-16 02:46:39.000000 agentevents-0.1.0/agentevents/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:46:53.237284 agentevents-0.1.0/agentevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-16 02:46:53.000000 agentevents-0.1.0/agentevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 02:46:53.000000 agentevents-0.1.0/agentevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:46:53.000000 agentevents-0.1.0/agentevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 02:46:53.000000 agentevents-0.1.0/agentevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 02:46:53.000000 agentevents-0.1.0/agentevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 02:46:53.237284 agentevents-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-16 02:46:39.000000 agentevents-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:39:36.069879 agentevents-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 08:39:24.000000 agentevents-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-16 08:39:36.069879 agentevents-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-07-16 08:39:24.000000 agentevents-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:39:36.069879 agentevents-0.1.3/agentevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-16 08:39:24.000000 agentevents-0.1.3/agentevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-07-16 08:39:24.000000 agentevents-0.1.3/agentevents/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:39:36.069879 agentevents-0.1.3/agentevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-16 08:39:36.000000 agentevents-0.1.3/agentevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 08:39:36.000000 agentevents-0.1.3/agentevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 08:39:36.000000 agentevents-0.1.3/agentevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 08:39:36.000000 agentevents-0.1.3/agentevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 08:39:36.000000 agentevents-0.1.3/agentevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 08:39:36.069879 agentevents-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-16 08:39:24.000000 agentevents-0.1.3/setup.py
```

### Comparing `agentevents-0.1.0/LICENSE` & `agentevents-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agentevents-0.1.0/agentevents/main.py` & `agentevents-0.1.3/agentevents/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,41 @@
     get_memories
 )
 
 dotenv.load_dotenv()
 
 console = Console()
 
+DEFAULT_TYPE_COLORS = {
+    "unknown": "white",
+    "error": "red",
+    "warning": "yellow",
+    "info": "blue",
+    "success": "green",
+    "debug": "magenta",
+    "critical": "red",
+    "start": "green",
+    "stop": "red",
+    "pause": "yellow",
+    "resume": "green",
+    "epoch": "blue",
+    "summary": "cyan",
+    "reasoning": "blue",
+    "action": "green",
+    "system": "magenta",
+}
+
 
 def create_event(
     content,
     type=None,
     subtype=None,
     creator=None,
     metadata={},
-    type_colors={},
+    type_colors=DEFAULT_TYPE_COLORS,
     panel=True,
 ):
     """
     Create an event with provided metadata and saves it to the event log file
 
     Parameters:
     - content: Content of the event
@@ -59,15 +78,15 @@
         "metadata": metadata,
     }
 
     event_string = event_to_string(event)
 
     create_memory("events", content, metadata=metadata)
     if panel:
-        panel = print(Panel(event_string, style=color))
+        console.print(Panel(event_string, style=color))
     else:
         console.print(event_string, style=color)
     write_to_log(f"{event_string}")
 
 
 def get_events(type=None, n_results=None, filter_metadata=None):
     """
```

### Comparing `agentevents-0.1.0/setup.py` & `agentevents-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = [line for line in readme if "<img" not in line]
     # now join all the lines back together
     readme = "\n".join(readme)
 
 
 setup(
     name="agentevents",
-    version="0.1.0",
+    version="0.1.3",
     description="Searchable events with colorful log output for agents.",
     long_description=readme,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/agentevents",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

