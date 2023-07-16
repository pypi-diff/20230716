# Comparing `tmp/qalita-1.0.5.tar.gz` & `tmp/qalita-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.5.tar", max compression
+gzip compressed data, was "qalita-1.0.6.tar", max compression
```

## Comparing `qalita-1.0.5.tar` & `qalita-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-14 13:56:05.343383 qalita-1.0.5/LICENSE
--rw-r--r--   0        0        0      416 2023-07-14 13:56:05.343383 qalita-1.0.5/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-14 13:56:16.418554 qalita-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 13:56:05.366383 qalita-1.0.5/qalita/__init__.py
--rw-r--r--   0        0        0     4189 2023-07-14 13:56:16.419471 qalita-1.0.5/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-14 13:56:05.366383 qalita-1.0.5/qalita/commands/__init__.py
--rw-r--r--   0        0        0    18029 2023-07-14 13:56:05.344384 qalita-1.0.5/qalita/commands/agent.py
--rw-r--r--   0        0        0    14531 2023-07-14 13:56:05.344384 qalita-1.0.5/qalita/commands/pack.py
--rw-r--r--   0        0        0     9756 2023-07-14 13:56:05.344384 qalita-1.0.5/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-14 13:56:05.366383 qalita-1.0.5/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-14 13:56:05.344384 qalita-1.0.5/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-14 13:56:05.344384 qalita-1.0.5/qalita/internal/utils.py
--rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 qalita-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-16 19:00:31.187323 qalita-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1942 2023-07-16 19:00:31.187323 qalita-1.0.6/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-16 19:00:41.128159 qalita-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 19:00:31.209323 qalita-1.0.6/qalita/__init__.py
+-rw-r--r--   0        0        0     4189 2023-07-16 19:00:41.129159 qalita-1.0.6/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:00:31.209323 qalita-1.0.6/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    19666 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14531 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9756 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:00:31.209323 qalita-1.0.6/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/internal/utils.py
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.6/PKG-INFO
```

### Comparing `qalita-1.0.5/LICENSE` & `qalita-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.5/pyproject.toml` & `qalita-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.5"
+version = "1.0.6"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `qalita-1.0.5/qalita/cli.py` & `qalita-1.0.6/qalita/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @pass_config
 def version(config):
     """
     Display the version of the cli
     """
     logger.info("------------- QALITA CLI Version -------------")
-    logger.info(f"Version : 1.0.5")
+    logger.info(f"Version : 1.0.6")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.5/qalita/commands/agent.py` & `qalita-1.0.6/qalita/commands/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import random
 import string
 import tarfile
 from datetime import datetime
 from shutil import copy2
 import json
 import select
-
+import logging
 
 @click.group()
 @click.option(
     "-n",
     "--name",
     help="The name of the agent, it will be used to identify the agent in the qalita platform",
     envvar="QALITA_AGENT_NAME",
@@ -301,28 +301,28 @@
                     mode="get",
                 )
                 if check_job.status_code == 200:
                     job = check_job.json()
                     source = job["source"]
                     pack = job["pack"]
                     job_run(source, pack)
-                    time.sleep(10)
                 else:
                     time.sleep(10)
         except KeyboardInterrupt:
             logger.warning("KILLSIG detected. Gracefully exiting the program.")
             logger.error("Set Agent OFFLINE...")
             send_alive(config_file=agent_conf, status="offline")
             logger.error("Exit")
 
     else:
         logger.error("Agent mode not supported : <worker/job>")
         sys.exit(1)
 
 def pull_pack(pack_id, pack_version=None):
+    logger.info("------------- Pack Pull -------------")
     # Fetch the pack data from api
     response_pack = send_api_request(f"/assets/{pack_id}", "get")
     if response_pack.status_code == 200:
         # The request was successful
         response_pack = response_pack.json()
     else:
         # The request failed
@@ -364,32 +364,57 @@
     # Système de caching, on regarde si le pack est déjà présent dans le cache sinon on le télécharge
     file_name = pack_url.split("/")[-1]
     bucket_name = pack_url.split("/")[3]
     s3_folder = "/".join(pack_url.split("/")[4:-1])
     local_path = f"./agent_run_temp/{bucket_name}/{s3_folder}/{file_name}"
 
     if os.path.exists(local_path):
+        logger.info(f"Using CACHED Pack at : {local_path}")
         return local_path
     if not os.path.exists(f"./agent_run_temp/{bucket_name}/{s3_folder}"):
         os.makedirs(f"./agent_run_temp/{bucket_name}/{s3_folder}")
 
     # Fetch the pack from api
     response = send_api_request(f"/assets/{pack_id}/fetch/{pack_version_id}", "get")
 
     if response.status_code == 200:
         # The request was successful
         with open(local_path, "wb") as file:
             file.write(response.content)
         logger.info(f"Pack fetched successfully")
         return local_path
     else:
-        logger.error(f"Failed to fetch pack. Status code: {response.status_code}")
+        logger.error(f"Failed to fetch pack : {response.text}")
+        sys.exit(1)
 
 
 def run_pack(pack_file_path):
+    logger = logging.getLogger(__name__)
+    logger.setLevel(logging.INFO)
+
+    # create a file handler
+    handler = logging.FileHandler(os.path.join(pack_file_path, 'logs.txt'))
+    handler.setLevel(logging.INFO)
+
+    # create a logging format
+    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+    handler.setFormatter(formatter)
+
+    # add the handlers to the logger
+    logger.addHandler(handler)
+
+    # create a stdout handler
+    stdout_handler = logging.StreamHandler()
+    stdout_handler.setLevel(logging.INFO)
+    stdout_handler.setFormatter(formatter)
+
+    # add the stdout handler to the logger
+    logger.addHandler(stdout_handler)
+
+
     logger.info("------------- Pack Run -------------")
     # Check if the run.sh file exists
     run_script = "run.sh"  # Only the script name is needed now
     if not os.path.isfile(os.path.join(pack_file_path, run_script)):
         logger.error(
             f"run.sh script does not exist in the package folder {pack_file_path}"
         )
@@ -417,31 +442,35 @@
             if fd == process.stderr.fileno():
                 read = process.stderr.readline().strip()
                 if read:  # Only print if there's output
                     logger.error(read)
 
     process.stdout.close()
     process.stderr.close()
-    logger.success("Pack run completed")
+    logger.info("Pack run completed")
     return 0
 
 
 @pass_config
 def job_run(config, source_id, source_version, pack_id, pack_version):
     logger.info("------------- Job Run -------------")
+    start_time = datetime.now()
+    logger.info(f"Start Time: {start_time.strftime('%Y-%m-%d %H:%M:%S')}")
+    logger.info(f"Source {source_id}:{source_version}")
+    logger.info(f"Pack {pack_id}:{pack_version}")
 
     """Runs a job"""
     agent_conf = config.load_agent_config()
     send_alive(config_file=agent_conf, mode="job", status="starting")
 
     pack_file_path = pull_pack(pack_id, pack_version)
     pack_folder = f"{pack_file_path.split('/')[-1].split('.')[0]}_pack"
 
     # Create a sub folder named with the current datetime and random generated seed
-    datetime_string = datetime.now().strftime("%Y%m%d%H%M%S")
+    datetime_string = start_time.strftime("%Y%m%d%H%M%S")
     random_seed = "".join(
         random.choice(string.ascii_lowercase + string.digits) for _ in range(5)
     )
     temp_folder_name = f"./agent_run_temp/{datetime_string}_{random_seed}"
     os.makedirs(temp_folder_name)
 
     # Copy the downloaded pack to the temp folder
@@ -485,18 +514,34 @@
         sys.exit(1)
 
     # save the source conf as a json file in the temp folder
     with open(os.path.join(temp_folder_name,pack_folder, "source_conf.json"), "w") as file:
         json.dump(source, file, indent=4)
 
     # run the job
-    run_pack(os.path.join(temp_folder_name,pack_folder))
-
-    logger.info(f"Sending data to Qalita Platform...")
-    # todo send the data to the qalita platform
+    send_alive(config_file=agent_conf, mode="job", status="running")
+    status = run_pack(os.path.join(temp_folder_name,pack_folder))
+    if status == 0:
+        send_alive(config_file=agent_conf, mode="job", status="succeded")
+    else:
+        send_alive(config_file=agent_conf, mode="job", status="failed")
+    post_run()
 
     logger.success(f"Job run finished")
+    end_time = datetime.now()
+    elapsed_time = end_time - start_time
+    logger.info(f"End Time: {end_time.strftime('%Y-%m-%d %H:%M:%S')}")
+    logger.info(f"Elapsed Time: {elapsed_time}")
+
+def post_run():
+    logger.info("------------- Job Post Run -------------")
+
+    logger.info(f"Uploading logs to Qalita Platform...")
+    # todo send the logs to the qalita platform
+
+    logger.info(f"Uploading results to Qalita Platform...")
+    # todo send the logs to the qalita platform
 
 
 @agent.group(help="Manage Agent Jobs")
 def jobs():
     """Jobs are the tasks that the agent will execute"""
```

### Comparing `qalita-1.0.5/qalita/commands/pack.py` & `qalita-1.0.6/qalita/commands/pack.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.5/qalita/commands/source.py` & `qalita-1.0.6/qalita/commands/source.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.5/qalita/internal/logger.py` & `qalita-1.0.6/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.5/qalita/internal/utils.py` & `qalita-1.0.6/qalita/internal/utils.py`

 * *Files identical despite different names*

