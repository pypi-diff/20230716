# Comparing `tmp/Dowell secure github repository-0.5.0.tar.gz` & `tmp/Dowell secure github repository-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dowell secure github repository-0.5.0.tar", last modified: Sun Jul 16 18:36:23 2023, max compression
+gzip compressed data, was "Dowell secure github repository-0.6.0.tar", last modified: Sun Jul 16 18:53:24 2023, max compression
```

## Comparing `Dowell secure github repository-0.5.0.tar` & `Dowell secure github repository-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 18:36:23.459380 Dowell secure github repository-0.5.0/
-drwxrwxrwx   0        0        0        0 2023-07-16 18:36:23.425248 Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/
--rw-rw-rw-   0        0        0     5044 2023-07-16 18:36:23.000000 Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-16 18:36:23.000000 Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 18:36:23.000000 Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 18:36:23.000000 Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-16 18:36:23.000000 Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5044 2023-07-16 18:36:23.456440 Dowell secure github repository-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4733 2023-07-16 18:35:40.000000 Dowell secure github repository-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 18:36:23.452791 Dowell secure github repository-0.5.0/doWellSecureGithubRepository/
--rw-rw-rw-   0        0        0       70 2023-07-16 18:29:09.000000 Dowell secure github repository-0.5.0/doWellSecureGithubRepository/__init__.py
--rw-rw-rw-   0        0        0     5406 2023-07-16 18:29:35.000000 Dowell secure github repository-0.5.0/doWellSecureGithubRepository/doWellSecureGithubRepository.py
--rw-rw-rw-   0        0        0       42 2023-07-16 18:36:23.459380 Dowell secure github repository-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      753 2023-07-16 18:35:30.000000 Dowell secure github repository-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 18:53:24.458109 Dowell secure github repository-0.6.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 18:53:24.423600 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/
+-rw-rw-rw-   0        0        0     5041 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5041 2023-07-16 18:53:24.455752 Dowell secure github repository-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4731 2023-07-16 18:52:54.000000 Dowell secure github repository-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 18:53:24.452157 Dowell secure github repository-0.6.0/doWellSecureGithubRepository/
+-rw-rw-rw-   0        0        0       70 2023-07-16 18:29:09.000000 Dowell secure github repository-0.6.0/doWellSecureGithubRepository/__init__.py
+-rw-rw-rw-   0        0        0     3463 2023-07-16 18:52:30.000000 Dowell secure github repository-0.6.0/doWellSecureGithubRepository/doWellSecureGithubRepository.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 18:53:24.459111 Dowell secure github repository-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      753 2023-07-16 18:52:44.000000 Dowell secure github repository-0.6.0/setup.py
```

### Comparing `Dowell secure github repository-0.5.0/Dowell_secure_github_repository.egg-info/PKG-INFO` & `Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Dowell-secure-github-repository
-Version: 0.5.0
+Version: 0.6.0
 Summary: Dowell secure github repository from DoWell
 Author: uxlivinglab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
-# Version: 0.5.0
+# Version: 0.6.0
 # Description:
 This Package seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The Package offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository Package ensures the integrity and availability of your code backups.
 
 The Secure Repository Package offers a range of powerful features to enhance code backup:
 
 - Repository Clone: The Package enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
 - Webhooks Integration: With seamless integration with Github's webhooks, the Package automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the Package captures these changes in real-time, ensuring that your backups are always up to date.
@@ -23,15 +23,14 @@
 ```
         
 # Usage:
 - Import the package and create an instance of the `doWellSecureGithubRepository` class:
     
 ```python
 from doWellSecureGithubRepository import doWellSecureGithubRepository
-
 api = doWellSecureGithubRepository(api_key)
 ```
     
 - Available methods:
     - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
     - `get_backup_reports()`: Retrieves backup reports.
     - `get_repository_reports()`: Retrieves repository reports.
```

### Comparing `Dowell secure github repository-0.5.0/PKG-INFO` & `Dowell secure github repository-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Dowell secure github repository
-Version: 0.5.0
+Version: 0.6.0
 Summary: Dowell secure github repository from DoWell
 Author: uxlivinglab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
-# Version: 0.5.0
+# Version: 0.6.0
 # Description:
 This Package seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The Package offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository Package ensures the integrity and availability of your code backups.
 
 The Secure Repository Package offers a range of powerful features to enhance code backup:
 
 - Repository Clone: The Package enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
 - Webhooks Integration: With seamless integration with Github's webhooks, the Package automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the Package captures these changes in real-time, ensuring that your backups are always up to date.
@@ -23,15 +23,14 @@
 ```
         
 # Usage:
 - Import the package and create an instance of the `doWellSecureGithubRepository` class:
     
 ```python
 from doWellSecureGithubRepository import doWellSecureGithubRepository
-
 api = doWellSecureGithubRepository(api_key)
 ```
     
 - Available methods:
     - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
     - `get_backup_reports()`: Retrieves backup reports.
     - `get_repository_reports()`: Retrieves repository reports.
```

### Comparing `Dowell secure github repository-0.5.0/README.md` & `Dowell secure github repository-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Version: 0.5.0
+# Version: 0.6.0
 # Description:
 This Package seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The Package offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository Package ensures the integrity and availability of your code backups.
 
 The Secure Repository Package offers a range of powerful features to enhance code backup:
 
 - Repository Clone: The Package enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
 - Webhooks Integration: With seamless integration with Github's webhooks, the Package automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the Package captures these changes in real-time, ensuring that your backups are always up to date.
@@ -15,15 +15,14 @@
 ```
         
 # Usage:
 - Import the package and create an instance of the `doWellSecureGithubRepository` class:
     
 ```python
 from doWellSecureGithubRepository import doWellSecureGithubRepository
-
 api = doWellSecureGithubRepository(api_key)
 ```
     
 - Available methods:
     - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
     - `get_backup_reports()`: Retrieves backup reports.
     - `get_repository_reports()`: Retrieves repository reports.
```

### Comparing `Dowell secure github repository-0.5.0/setup.py` & `Dowell secure github repository-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name="Dowell secure github repository",
-    version="0.5.0",
+    version="0.6.0",
     description="Dowell secure github repository from DoWell",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='uxlivinglab',
     license="Apache License 2.0",
     packages=["doWellSecureGithubRepository"],
     include_package_data=True,
```

