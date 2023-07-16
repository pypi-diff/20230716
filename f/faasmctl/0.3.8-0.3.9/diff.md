# Comparing `tmp/faasmctl-0.3.8.tar.gz` & `tmp/faasmctl-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.3.8.tar", last modified: Sun Jul 16 10:05:37 2023, max compression
+gzip compressed data, was "faasmctl-0.3.9.tar", last modified: Sun Jul 16 11:36:59 2023, max compression
```

## Comparing `faasmctl-0.3.8.tar` & `faasmctl-0.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:05:37.114893 faasmctl-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 10:03:07.000000 faasmctl-0.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-16 10:05:37.114893 faasmctl-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-16 10:03:07.000000 faasmctl-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:05:37.110893 faasmctl-0.3.8/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:05:37.110893 faasmctl-0.3.8/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:05:37.110893 faasmctl-0.3.8/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:05:37.110893 faasmctl-0.3.8/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-16 10:05:27.000000 faasmctl-0.3.8/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-16 10:05:27.000000 faasmctl-0.3.8/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-16 10:03:07.000000 faasmctl-0.3.8/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 10:05:37.110893 faasmctl-0.3.8/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-16 10:05:37.000000 faasmctl-0.3.8/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-16 10:05:37.000000 faasmctl-0.3.8/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 10:05:37.000000 faasmctl-0.3.8/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 10:05:37.000000 faasmctl-0.3.8/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 10:05:37.000000 faasmctl-0.3.8/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 10:05:37.000000 faasmctl-0.3.8/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-16 10:03:07.000000 faasmctl-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 10:05:37.114893 faasmctl-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.933112 faasmctl-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 11:34:09.000000 faasmctl-0.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-16 11:36:59.933112 faasmctl-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-16 11:34:09.000000 faasmctl-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.925111 faasmctl-0.3.9/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.929112 faasmctl-0.3.9/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.933112 faasmctl-0.3.9/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.933112 faasmctl-0.3.9/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-16 11:36:48.000000 faasmctl-0.3.9/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-16 11:36:48.000000 faasmctl-0.3.9/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-16 11:34:09.000000 faasmctl-0.3.9/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:36:59.929112 faasmctl-0.3.9/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-16 11:36:59.000000 faasmctl-0.3.9/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-16 11:34:09.000000 faasmctl-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-16 11:36:59.933112 faasmctl-0.3.9/setup.cfg
```

### Comparing `faasmctl-0.3.8/LICENSE.md` & `faasmctl-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/PKG-INFO` & `faasmctl-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.8
+Version: 0.3.9
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.8
+pip install faasmctl==0.3.9
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.8/README.md` & `faasmctl-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.8
+pip install faasmctl==0.3.9
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.8/faasmctl/tasks/cli.py` & `faasmctl-0.3.9/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/tasks/delete.py` & `faasmctl-0.3.9/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/tasks/deploy.py` & `faasmctl-0.3.9/faasmctl/tasks/deploy.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                 "WARNING: using the --clean flag with --mount_source "
                 "env. variable is disabled, as local changes could be "
                 "erased!"
             )
         faasm_checkout, faasm_ver = fetch_faasm_code(
             faasm_source=mount_source, force=False
         )
+        mount_source = True
     else:
         # Otherwise, we will check out the code in a faasmctl-specific working
         # directoy
         mount_source = False
         faasm_checkout, faasm_ver = fetch_faasm_code(force=clean)
 
     return deploy_compose_cluster(faasm_checkout, workers, mount_source, ini_file)
```

### Comparing `faasmctl-0.3.8/faasmctl/tasks/flush.py` & `faasmctl-0.3.9/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/tasks/invoke.py` & `faasmctl-0.3.9/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/tasks/logs.py` & `faasmctl-0.3.9/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/tasks/restart.py` & `faasmctl-0.3.9/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/tasks/status.py` & `faasmctl-0.3.9/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/compose.py` & `faasmctl-0.3.9/faasmctl/util/compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,20 +114,22 @@
 
     compose_cmd = [
         "docker compose",
         "-p {}".format(cluster_name),
         cmd,
     ]
     compose_cmd = " ".join(compose_cmd)
+
+    compose_env = get_compose_env_vars(work_dir, mount_source)
     run(
         compose_cmd,
         shell=True,
         check=True,
         cwd=work_dir,
-        env=get_compose_env_vars(work_dir, mount_source),
+        env=compose_env,
     )
 
 
 def wait_for_venv(ini_file, cli):
     """
     When executing a command in a CLI container, the first time we start it
     we may run into a race condition between:
```

### Comparing `faasmctl-0.3.8/faasmctl/util/config.py` & `faasmctl-0.3.9/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/deploy.py` & `faasmctl-0.3.9/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/docker.py` & `faasmctl-0.3.9/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/flush.py` & `faasmctl-0.3.9/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.3.9/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.3.9/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/invoke.py` & `faasmctl-0.3.9/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/planner.py` & `faasmctl-0.3.9/faasmctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl/util/upload.py` & `faasmctl-0.3.9/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.3.9/faasmctl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.3.8
+Version: 0.3.9
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.3.8
+pip install faasmctl==0.3.9
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.3.8/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.3.9/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.3.8/pyproject.toml` & `faasmctl-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

