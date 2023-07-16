# Comparing `tmp/promptlink-0.1.1.tar.gz` & `tmp/promptlink-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlink-0.1.1.tar", max compression
+gzip compressed data, was "promptlink-0.1.2.tar", max compression
```

## Comparing `promptlink-0.1.1.tar` & `promptlink-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-05-21 09:40:36.941479 promptlink-0.1.1/LICENSE
--rw-r--r--   0        0        0     2005 2023-06-16 01:33:31.452109 promptlink-0.1.1/README.md
--rw-r--r--   0        0        0     4233 2023-06-17 13:13:21.712262 promptlink-0.1.1/promptlink/__init__.py
--rw-r--r--   0        0        0     2773 2023-06-13 13:09:03.424069 promptlink-0.1.1/promptlink/main.py
--rw-r--r--   0        0        0    36606 2023-06-11 12:58:40.938629 promptlink-0.1.1/promptlink/requirements.txt
--rw-r--r--   0        0        0     2466 2023-06-15 23:31:12.296018 promptlink-0.1.1/promptlink/static/index.html
--rw-r--r--   0        0        0      514 2023-06-17 13:13:47.876698 promptlink-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 promptlink-0.1.1/setup.py
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 promptlink-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-21 09:40:36.941479 promptlink-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2151 2023-07-16 17:56:34.247746 promptlink-0.1.2/README.md
+-rw-r--r--   0        0        0     4344 2023-07-16 17:55:31.364000 promptlink-0.1.2/promptlink/__init__.py
+-rw-r--r--   0        0        0     2773 2023-06-13 13:09:03.424069 promptlink-0.1.2/promptlink/main.py
+-rw-r--r--   0        0        0    36606 2023-06-11 12:58:40.938629 promptlink-0.1.2/promptlink/requirements.txt
+-rw-r--r--   0        0        0     2466 2023-06-15 23:31:12.296018 promptlink-0.1.2/promptlink/static/index.html
+-rw-r--r--   0        0        0      514 2023-07-16 17:56:06.911856 promptlink-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 promptlink-0.1.2/setup.py
+-rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 promptlink-0.1.2/PKG-INFO
```

### Comparing `promptlink-0.1.1/LICENSE` & `promptlink-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.1/README.md` & `promptlink-0.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,35 @@
-# PromptLink
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-[![PyPI version](https://badge.fury.io/py/promptlink.svg)](https://badge.fury.io/py/promptlink)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+packages = \
+['promptlink']
 
-Simplify user authentication and secure access from anywhere with temporary links.
+package_data = \
+{'': ['*'], 'promptlink': ['static/*']}
 
-PromptLink is a Python package that allows you to streamline user authentication and enable secure access to your application from anywhere. It provides a seamless way to generate temporary links for user authentication, without relying on specific web frameworks. A Google Cloud Function is set up to ensure a secure temporary link for authentication.
+install_requires = \
+['Jinja2',
+ 'functions-framework',
+ 'google-cloud-functions',
+ 'google-cloud-pubsub',
+ 'google-cloud-storage',
+ 'pyyaml']
+
+setup_kwargs = {
+    'name': 'promptlink',
+    'version': '0.1.2',
+    'description': 'Simplify user authentication and secure access from anywhere with customizable prompts and temporary links.',
+    'long_description': '# PromptLink\n\n[![PyPI version](https://badge.fury.io/py/promptlink.svg)](https://badge.fury.io/py/promptlink)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n\nSimplify user authentication and secure access from anywhere with temporary links.\n\nPromptLink is a Python package that allows you to streamline user authentication and enable secure access to your application from anywhere. It provides a seamless way to generate temporary links for user authentication, without relying on specific web frameworks. A Google Cloud Function is set up to ensure a secure temporary link for authentication.\n\n## Key Features\n\n- **Easy and secure**: Generate secure temporary links to enable easy secure access from anywhere.\n- **Versatile Integration**: Works across various application types, not limited to web applications.\n\n## Installation\n\nYou can install PromptLink using pip:\n```shell\npip install promptlink\n```\nAlternatively, if you are using Poetry (recommended), you can install it as follows:\n```shell\npoetry add promptlink\n```\n\n## Usage\n\nHere\'s a basic example of using PromptLink:\n\n```python\nfrom promptlink import Authenticator\n\n\nwith Authenticator(send_link_callback=lambda l: print(f"URL: {l}")) as authenticator:\n    # The code in this block is executed after the link has been accessed \n    # in order to avoid authentication timeouts\n    print("Setting up authentication...")\n    authenticator.authenticate(lambda s: s == "12345678")\n    # Below statements will be reached after \'12345678\' was input on the webpage prompt\n    print("Finished")\n```\n\n## GCP permission requirements\nThe following permissions are needed for this library:\n- Permissions to create Storage buckets and objects\n- Permissions to set up a Pub/Sub topic and subscriptions\n- Permissions to deploy a Cloud Function  \n\nThe library will attempt to use the default service account.\nAny resources created will be named \'promptlink-\' followed by a random UUID, so that collision with existing resources is extremely unlikely.\n\n## License\nThis project is licensed under the MIT License. See the LICENSE file for details.\n',
+    'author': 'Stéphane Thibaud',
+    'author_email': 'snthibaud@gmail.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.9,<4.0',
+}
 
-## Key Features
 
-- **Easy and secure**: Generate secure temporary links to enable easy secure access from anywhere.
-- **Versatile Integration**: Works across various application types, not limited to web applications.
-
-## Installation
-
-You can install PromptLink using pip:
-```shell
-pip install promptlink
-```
-Alternatively, if you are using Poetry (recommended), you can install it as follows:
-```shell
-poetry add promptlink
-```
-
-## Usage
-
-Here's a basic example of using PromptLink:
-
-```python
-from promptlink import Authenticator
-
-
-with Authenticator(send_link_callback=lambda l: print(f"URL: {l}")) as authenticator:
-    # The code in this block is executed after the link has been accessed 
-    # in order to avoid authentication timeouts
-    print("Setting up authentication...")
-    authenticator.authenticate(lambda s: s == "12345678")
-    # Below statements will be reached after '12345678' was input on the webpage prompt
-    print("Finished")
-```
-
-## GCP permission requirements
-The following permissions are needed for this library:
-- Permissions to create Storage buckets and objects
-- Permissions to set up a Pub/Sub topic and subscriptions
-- Permissions to deploy a Cloud Function
-The library will attempt to use the default service account.
-
-## License
-This project is licensed under the MIT License. See the LICENSE file for details.
+setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `promptlink-0.1.1/promptlink/__init__.py` & `promptlink-0.1.2/promptlink/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,24 @@
     _status_relayed: Event = Event()
     _input_queue = SimpleQueue()
     _publisher: PublisherClient = PublisherClient()
     _subscriber: SubscriberClient = SubscriberClient()
 
     def _deploy_cloud_function(self) -> str:
         self._function_name = f"promptlink-{self._authentication_id}"
-        return safe_load(run(
+        output = run(
             f"gcloud functions deploy {self._function_name} --gen2 "
             f"--region={self.gcp_region} --runtime=python39 "
             f"--source=\"{Path(__file__).resolve().parent}\" --entry-point=entrypoint --trigger-http "
-            f"--allow-unauthenticated", capture_output=True, text=True, shell=True).stdout)["serviceConfig"]["uri"]
+            f"--allow-unauthenticated", capture_output=True, text=True, shell=True).stdout
+        try:
+            return safe_load(output)["serviceConfig"]["uri"]
+        except TypeError:
+            print(output)
+            raise
 
     def _remove_cloud_function(self):
         print(run(f"gcloud functions delete {self._function_name} --quiet",
                   capture_output=True, text=True, shell=True).stdout)
 
     def _handle_message(self, message: Message):
         message.ack()
```

### Comparing `promptlink-0.1.1/promptlink/main.py` & `promptlink-0.1.2/promptlink/main.py`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.1/promptlink/requirements.txt` & `promptlink-0.1.2/promptlink/requirements.txt`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.1/promptlink/static/index.html` & `promptlink-0.1.2/promptlink/static/index.html`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.1/pyproject.toml` & `promptlink-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptlink"
-version = "0.1.1"
+version = "0.1.2"
 description = "Simplify user authentication and secure access from anywhere with customizable prompts and temporary links."
 authors = ["Stéphane Thibaud <snthibaud@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 functions-framework = "*"
```

### Comparing `promptlink-0.1.1/PKG-INFO` & `promptlink-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlink
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simplify user authentication and secure access from anywhere with customizable prompts and temporary links.
 Author: Stéphane Thibaud
 Author-email: snthibaud@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -59,12 +59,15 @@
     print("Finished")
 ```
 
 ## GCP permission requirements
 The following permissions are needed for this library:
 - Permissions to create Storage buckets and objects
 - Permissions to set up a Pub/Sub topic and subscriptions
-- Permissions to deploy a Cloud Function
+- Permissions to deploy a Cloud Function  
+
 The library will attempt to use the default service account.
+Any resources created will be named 'promptlink-' followed by a random UUID, so that collision with existing resources is extremely unlikely.
 
 ## License
 This project is licensed under the MIT License. See the LICENSE file for details.
+
```

