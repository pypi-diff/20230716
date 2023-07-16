# Comparing `tmp/secret_checker-1.0.2.tar.gz` & `tmp/secret_checker-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_checker-1.0.2.tar", last modified: Sat Jul 15 18:30:25 2023, max compression
+gzip compressed data, was "secret_checker-1.0.3.tar", last modified: Sun Jul 16 17:31:51 2023, max compression
```

## Comparing `secret_checker-1.0.2.tar` & `secret_checker-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:25.644316 secret_checker-1.0.2/
--rw-rw-rw-   0        0        0      242 2023-07-15 18:30:25.644316 secret_checker-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-15 01:11:16.000000 secret_checker-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:25.628683 secret_checker-1.0.2/secret_checker/
--rw-rw-rw-   0        0        0        2 2023-07-15 18:14:03.000000 secret_checker-1.0.2/secret_checker/__init__.py
--rw-rw-rw-   0        0        0     3545 2023-07-15 18:10:55.000000 secret_checker-1.0.2/secret_checker/check_var.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:30:25.644316 secret_checker-1.0.2/secret_checker.egg-info/
--rw-rw-rw-   0        0        0      242 2023-07-15 18:30:25.000000 secret_checker-1.0.2/secret_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-15 18:30:25.000000 secret_checker-1.0.2/secret_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 18:30:25.000000 secret_checker-1.0.2/secret_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-15 18:30:25.000000 secret_checker-1.0.2/secret_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 18:30:25.644316 secret_checker-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      356 2023-07-15 18:29:59.000000 secret_checker-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:31:51.970001 secret_checker-1.0.3/
+-rw-rw-rw-   0        0        0      242 2023-07-16 17:31:51.969000 secret_checker-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-15 01:11:16.000000 secret_checker-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 17:31:51.947938 secret_checker-1.0.3/secret_checker/
+-rw-rw-rw-   0        0        0        2 2023-07-15 18:14:03.000000 secret_checker-1.0.3/secret_checker/__init__.py
+-rw-rw-rw-   0        0        0     3862 2023-07-16 17:29:06.000000 secret_checker-1.0.3/secret_checker/check_var.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:31:51.967994 secret_checker-1.0.3/secret_checker.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-16 17:31:51.000000 secret_checker-1.0.3/secret_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 17:31:51.970001 secret_checker-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      356 2023-07-16 17:31:26.000000 secret_checker-1.0.3/setup.py
```

### Comparing `secret_checker-1.0.2/secret_checker/check_var.py` & `secret_checker-1.0.3/secret_checker/check_var.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 import sys
 import inspect
 import pymsgbox as msgbox
 
 
 class SecretChecker:
 
-    def __init__(self, file_path=None, folder_name="app" , env_list=["prod", "production"], env_key_list = ["env", "environment"], button_values = ["OK", "Cancel"]):
+    def __init__(self, file_path=None, folder_name="" , env_list=["prod", "production"], env_key_list = ["env", "environment"], button_values = ["OK", "Cancel"]):
 
         # if the environment is prod / production then we don't need to show the pop-up 
         # self.env_key_list = env_key_list 
         
         self.file_path = file_path
         self.env_list = env_list
         self.button_display_options = button_values
 
         # print("file path : ", self.file_path)
 
-        if self.file_path:
+        if self.file_path and not folder_name:
             self._check_secrets_with_specific_values()
-        elif folder_name and folder_name == "app": 
-            # print("need to fetch all the files in the current directory")
+        elif not folder_name: 
+            print("need to fetch all the files in the current directory")
             self._fetch_all_files_in_same_directory()
         else:
+            print("need to fetch all files of a specific folder : ", folder_name)
             self._fetch_all_files_in_folder(folder_name)
     
 
     def _fetch_all_files_in_same_directory(self):
         
         current_directory = os.getcwd()
         files_list = [os.path.join(current_directory, file) for file in os.listdir(current_directory) if os.path.isfile(os.path.join(current_directory, file))]
@@ -35,57 +36,64 @@
         # print("files list : ", files_list)
 
         self._iterate_through_files(files_list)
     
 
     def _fetch_all_files_in_folder(self, folder_name="app"):
         
-        folder = folder_name # Specify the folder path within the project directory
-
-        # print("folder : ", folder)
+        current_directory = os.getcwd()
         
-        current_file = inspect.getframeinfo(inspect.currentframe()).filename
-        project_directory = os.path.dirname(os.path.abspath(current_file))
-        folder_path = os.path.join(project_directory, folder)
-
         files_list = []
-        for root, dirs, files in os.walk(folder_path):
+
+        self.file_path = os.path.join(current_directory, folder_name)
+
+        print("file path to traverse : ", self.file_path)
+
+        for root, dirs, files in os.walk(self.file_path):
             if "__pycache__" in dirs:
                 dirs.remove("__pycache__")  # Skip files in the __pycache__ directory
             for file in files:
                 file_path = os.path.join(root, file)
                 files_list.append(file_path)
-
+        
+        print("files list ", files_list)
         self._iterate_through_files(files_list)
 
     
     def _iterate_through_files(self, files):
 
+        print("files : ", files)
+        print("total files which need to be calculated : ", len(files))
         # Print all file paths
         for file in files:
             self.file_path = file
             # print("==== ", file)
             self._check_secrets_with_specific_values()
 
 
     def _check_secrets_with_specific_values(self):
         
         with open(self.file_path, 'r') as file:
+            print(self.file_path)
             tree = ast.parse(file.read())
 
             constants = []
 
             for node in ast.walk(tree):
 
                 if isinstance(node, ast.Assign) and len(node.targets) == 1:
                     target = node.targets[0]
                     
                     if isinstance(target, ast.Name) and target.id.isupper():
 
-                        secret_val = ast.literal_eval(node.value)
+                        print("value of node is : ", node.value, target.id)
+                        try:
+                            secret_val = ast.literal_eval(node.value)
+                        except Exception as e:
+                            secret_val = node.value
 
                         if any(word in str(secret_val).lower() for word in self.env_list):
                             button_val = msgbox.confirm(f"SECRET {target.id} = {secret_val} found in {self.file_path}. Do you wish to continue?", "Trying to access prod resource", buttons=self.button_display_options)
                             
                             if button_val in ["No", "Cancel"]:
                                 sys.exit(1)
```

