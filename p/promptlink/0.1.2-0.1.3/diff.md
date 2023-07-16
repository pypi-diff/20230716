# Comparing `tmp/promptlink-0.1.2.tar.gz` & `tmp/promptlink-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlink-0.1.2.tar", max compression
+gzip compressed data, was "promptlink-0.1.3.tar", max compression
```

## Comparing `promptlink-0.1.2.tar` & `promptlink-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-05-21 09:40:36.941479 promptlink-0.1.2/LICENSE
--rw-r--r--   0        0        0     2151 2023-07-16 17:56:34.247746 promptlink-0.1.2/README.md
--rw-r--r--   0        0        0     4344 2023-07-16 17:55:31.364000 promptlink-0.1.2/promptlink/__init__.py
--rw-r--r--   0        0        0     2773 2023-06-13 13:09:03.424069 promptlink-0.1.2/promptlink/main.py
--rw-r--r--   0        0        0    36606 2023-06-11 12:58:40.938629 promptlink-0.1.2/promptlink/requirements.txt
--rw-r--r--   0        0        0     2466 2023-06-15 23:31:12.296018 promptlink-0.1.2/promptlink/static/index.html
--rw-r--r--   0        0        0      514 2023-07-16 17:56:06.911856 promptlink-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 promptlink-0.1.2/setup.py
--rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 promptlink-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-21 09:40:36.941479 promptlink-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2151 2023-07-16 17:56:34.247746 promptlink-0.1.3/README.md
+-rw-r--r--   0        0        0     4351 2023-07-16 18:13:45.743786 promptlink-0.1.3/promptlink/__init__.py
+-rw-r--r--   0        0        0     2773 2023-06-13 13:09:03.424069 promptlink-0.1.3/promptlink/main.py
+-rw-r--r--   0        0        0    36606 2023-06-11 12:58:40.938629 promptlink-0.1.3/promptlink/requirements.txt
+-rw-r--r--   0        0        0     2466 2023-06-15 23:31:12.296018 promptlink-0.1.3/promptlink/static/index.html
+-rw-r--r--   0        0        0      514 2023-07-16 18:13:45.819786 promptlink-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 promptlink-0.1.3/setup.py
+-rw-r--r--   0        0        0     2840 1970-01-01 00:00:00.000000 promptlink-0.1.3/PKG-INFO
```

### Comparing `promptlink-0.1.2/LICENSE` & `promptlink-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.2/README.md` & `promptlink-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.2/promptlink/__init__.py` & `promptlink-0.1.3/promptlink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
     def _deploy_cloud_function(self) -> str:
         self._function_name = f"promptlink-{self._authentication_id}"
         output = run(
             f"gcloud functions deploy {self._function_name} --gen2 "
             f"--region={self.gcp_region} --runtime=python39 "
             f"--source=\"{Path(__file__).resolve().parent}\" --entry-point=entrypoint --trigger-http "
-            f"--allow-unauthenticated", capture_output=True, text=True, shell=True).stdout
+            f"--allow-unauthenticated", capture_output=True, text=True, shell=True)
         try:
-            return safe_load(output)["serviceConfig"]["uri"]
+            return safe_load(output.stdout)["serviceConfig"]["uri"]
         except TypeError:
-            print(output)
+            print(output.stderr)
             raise
 
     def _remove_cloud_function(self):
         print(run(f"gcloud functions delete {self._function_name} --quiet",
                   capture_output=True, text=True, shell=True).stdout)
 
     def _handle_message(self, message: Message):
```

### Comparing `promptlink-0.1.2/promptlink/main.py` & `promptlink-0.1.3/promptlink/main.py`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.2/promptlink/requirements.txt` & `promptlink-0.1.3/promptlink/requirements.txt`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.2/promptlink/static/index.html` & `promptlink-0.1.3/promptlink/static/index.html`

 * *Files identical despite different names*

### Comparing `promptlink-0.1.2/pyproject.toml` & `promptlink-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promptlink"
-version = "0.1.2"
+version = "0.1.3"
 description = "Simplify user authentication and secure access from anywhere with customizable prompts and temporary links."
 authors = ["Stéphane Thibaud <snthibaud@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 functions-framework = "*"
```

### Comparing `promptlink-0.1.2/setup.py` & `promptlink-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'google-cloud-functions',
  'google-cloud-pubsub',
  'google-cloud-storage',
  'pyyaml']
 
 setup_kwargs = {
     'name': 'promptlink',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Simplify user authentication and secure access from anywhere with customizable prompts and temporary links.',
     'long_description': '# PromptLink\n\n[![PyPI version](https://badge.fury.io/py/promptlink.svg)](https://badge.fury.io/py/promptlink)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n\nSimplify user authentication and secure access from anywhere with temporary links.\n\nPromptLink is a Python package that allows you to streamline user authentication and enable secure access to your application from anywhere. It provides a seamless way to generate temporary links for user authentication, without relying on specific web frameworks. A Google Cloud Function is set up to ensure a secure temporary link for authentication.\n\n## Key Features\n\n- **Easy and secure**: Generate secure temporary links to enable easy secure access from anywhere.\n- **Versatile Integration**: Works across various application types, not limited to web applications.\n\n## Installation\n\nYou can install PromptLink using pip:\n```shell\npip install promptlink\n```\nAlternatively, if you are using Poetry (recommended), you can install it as follows:\n```shell\npoetry add promptlink\n```\n\n## Usage\n\nHere\'s a basic example of using PromptLink:\n\n```python\nfrom promptlink import Authenticator\n\n\nwith Authenticator(send_link_callback=lambda l: print(f"URL: {l}")) as authenticator:\n    # The code in this block is executed after the link has been accessed \n    # in order to avoid authentication timeouts\n    print("Setting up authentication...")\n    authenticator.authenticate(lambda s: s == "12345678")\n    # Below statements will be reached after \'12345678\' was input on the webpage prompt\n    print("Finished")\n```\n\n## GCP permission requirements\nThe following permissions are needed for this library:\n- Permissions to create Storage buckets and objects\n- Permissions to set up a Pub/Sub topic and subscriptions\n- Permissions to deploy a Cloud Function  \n\nThe library will attempt to use the default service account.\nAny resources created will be named \'promptlink-\' followed by a random UUID, so that collision with existing resources is extremely unlikely.\n\n## License\nThis project is licensed under the MIT License. See the LICENSE file for details.\n',
     'author': 'Stéphane Thibaud',
     'author_email': 'snthibaud@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `promptlink-0.1.2/PKG-INFO` & `promptlink-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlink
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simplify user authentication and secure access from anywhere with customizable prompts and temporary links.
 Author: Stéphane Thibaud
 Author-email: snthibaud@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

