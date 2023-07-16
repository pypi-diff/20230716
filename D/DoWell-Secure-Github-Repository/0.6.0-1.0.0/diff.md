# Comparing `tmp/Dowell secure github repository-0.6.0.tar.gz` & `tmp/DoWell Secure Github Repository-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dowell secure github repository-0.6.0.tar", last modified: Sun Jul 16 18:53:24 2023, max compression
+gzip compressed data, was "DoWell Secure Github Repository-1.0.0.tar", last modified: Sun Jul 16 19:21:49 2023, max compression
```

## Comparing `Dowell secure github repository-0.6.0.tar` & `DoWell Secure Github Repository-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 18:53:24.458109 Dowell secure github repository-0.6.0/
-drwxrwxrwx   0        0        0        0 2023-07-16 18:53:24.423600 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/
--rw-rw-rw-   0        0        0     5041 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-07-16 18:53:24.000000 Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5041 2023-07-16 18:53:24.455752 Dowell secure github repository-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4731 2023-07-16 18:52:54.000000 Dowell secure github repository-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 18:53:24.452157 Dowell secure github repository-0.6.0/doWellSecureGithubRepository/
--rw-rw-rw-   0        0        0       70 2023-07-16 18:29:09.000000 Dowell secure github repository-0.6.0/doWellSecureGithubRepository/__init__.py
--rw-rw-rw-   0        0        0     3463 2023-07-16 18:52:30.000000 Dowell secure github repository-0.6.0/doWellSecureGithubRepository/doWellSecureGithubRepository.py
--rw-rw-rw-   0        0        0       42 2023-07-16 18:53:24.459111 Dowell secure github repository-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      753 2023-07-16 18:52:44.000000 Dowell secure github repository-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:49.551843 DoWell Secure Github Repository-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:49.545439 DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/
+-rw-rw-rw-   0        0        0     5150 2023-07-16 19:21:49.000000 DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-16 19:21:49.000000 DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 19:21:49.000000 DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 19:21:49.000000 DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-07-16 19:21:49.000000 DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5150 2023-07-16 19:21:49.550471 DoWell Secure Github Repository-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4830 2023-07-16 19:21:32.000000 DoWell Secure Github Repository-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 19:21:49.546947 DoWell Secure Github Repository-1.0.0/doWellSecureGithubRepository/
+-rw-rw-rw-   0        0        0       70 2023-07-16 18:29:09.000000 DoWell Secure Github Repository-1.0.0/doWellSecureGithubRepository/__init__.py
+-rw-rw-rw-   0        0        0     3463 2023-07-16 18:52:30.000000 DoWell Secure Github Repository-1.0.0/doWellSecureGithubRepository/doWellSecureGithubRepository.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 19:21:49.551843 DoWell Secure Github Repository-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-16 19:21:38.000000 DoWell Secure Github Repository-1.0.0/setup.py
```

### Comparing `Dowell secure github repository-0.6.0/Dowell_secure_github_repository.egg-info/PKG-INFO` & `DoWell Secure Github Repository-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: Dowell-secure-github-repository
-Version: 0.6.0
+Name: DoWell Secure Github Repository
+Version: 1.0.0
 Summary: Dowell secure github repository from DoWell
-Author: uxlivinglab
+Author: DoWell UX Living Lab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
-# Version: 0.6.0
+# DoWell Secure Github Repository 
+# Version: 1.0.0
 # Description:
 This Package seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The Package offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository Package ensures the integrity and availability of your code backups.
 
-The Secure Repository Package offers a range of powerful features to enhance code backup:
+The  DoWell Secure Github Repository Package offers a range of powerful features to enhance code backup:
 
-- Repository Clone: The Package enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
+- Repository Clone: The Package enables easy cloning of public repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
 - Webhooks Integration: With seamless integration with Github's webhooks, the Package automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the Package captures these changes in real-time, ensuring that your backups are always up to date.
-- Backup Reports: The Secure Repository Package generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
+- Backup Reports: The  DoWell Secure Github Repository Package generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
 - Repository Reports: In addition to backup reports, the Package also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
 # Installation:
 - Install the package using pip: 
 ```python
 pip install Dowell-secure-github-repository
 ```
         
@@ -36,57 +37,58 @@
     - `get_repository_reports()`: Retrieves repository reports.
     - `__init__(self, api_key)`
         
         Description: Initializes an instance of the doWellSecureGithubRepository class.
         
         Parameters:
         
-        - `api_key` (str): The API key required for authentication with the Secure Repository API.
+        - `api_key` (str): The API key required for authentication with the DoWell Secure Github Repository.
     - `clone_repository(self, repository_url)`
         
-        Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
+        Description: Clones a GitHub repository.
         
         Parameters:
         
         - `repository_url` (str): The URL of the GitHub repository to clone.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
     - `get_backup_reports(self)`
         
-        Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
+        Description: Retrieves backup reports from the DoWell Secure Github Repository.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
     - `get_repository_reports(self)`
         
-        Description: Retrieves repository reports from the Secure Repository API by making a GET request.
+        Description: Retrieves repository reports from the DoWell Secure Github Repository.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
 # Example:
     
 ```python
 from doWellSecureGithubRepository import doWellSecureGithubRepository
-
 api = doWellSecureGithubRepository(api_key)
 api.clone_repository(repository_url)
 api.get_backup_reports()
 api.get_repository_reports()
 ```
     
-# API Reference:
+# Library Reference:
 - `doWellSecureGithubRepository` class:
     - `__init__(api_key)`: Initializes the `doWellSecureGithubRepository` object with the API key.
     - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
     - `get_backup_reports()`: Retrieves backup reports.
     - `get_repository_reports()`: Retrieves repository reports.
 # Configuration:
 - The package requires a valid API key for authentication.
 # Dependencies:
 - requests: Required for making HTTP requests.
 - json: Required for parsing JSON data.
 # Support:
 - For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
-- If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
+- If you encounter any issues, have questions, or need assistance with the  DoWell Secure Github Repository library, please contact our support team.
 # License:
-- Apache License 2.0
+- Apache License 2.0
+
+# Powered by [DoWell UX Living Lab](https://uxlivinglab.com/en/)
```

### Comparing `Dowell secure github repository-0.6.0/PKG-INFO` & `DoWell Secure Github Repository-1.0.0/DoWell_Secure_Github_Repository.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
-Name: Dowell secure github repository
-Version: 0.6.0
+Name: DoWell-Secure-Github-Repository
+Version: 1.0.0
 Summary: Dowell secure github repository from DoWell
-Author: uxlivinglab
+Author: DoWell UX Living Lab
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 
-# Version: 0.6.0
+# DoWell Secure Github Repository 
+# Version: 1.0.0
 # Description:
 This Package seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The Package offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository Package ensures the integrity and availability of your code backups.
 
-The Secure Repository Package offers a range of powerful features to enhance code backup:
+The  DoWell Secure Github Repository Package offers a range of powerful features to enhance code backup:
 
-- Repository Clone: The Package enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
+- Repository Clone: The Package enables easy cloning of public repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
 - Webhooks Integration: With seamless integration with Github's webhooks, the Package automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the Package captures these changes in real-time, ensuring that your backups are always up to date.
-- Backup Reports: The Secure Repository Package generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
+- Backup Reports: The  DoWell Secure Github Repository Package generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
 - Repository Reports: In addition to backup reports, the Package also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
 # Installation:
 - Install the package using pip: 
 ```python
 pip install Dowell-secure-github-repository
 ```
         
@@ -36,57 +37,58 @@
     - `get_repository_reports()`: Retrieves repository reports.
     - `__init__(self, api_key)`
         
         Description: Initializes an instance of the doWellSecureGithubRepository class.
         
         Parameters:
         
-        - `api_key` (str): The API key required for authentication with the Secure Repository API.
+        - `api_key` (str): The API key required for authentication with the DoWell Secure Github Repository.
     - `clone_repository(self, repository_url)`
         
-        Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
+        Description: Clones a GitHub repository.
         
         Parameters:
         
         - `repository_url` (str): The URL of the GitHub repository to clone.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
     - `get_backup_reports(self)`
         
-        Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
+        Description: Retrieves backup reports from the DoWell Secure Github Repository.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
     - `get_repository_reports(self)`
         
-        Description: Retrieves repository reports from the Secure Repository API by making a GET request.
+        Description: Retrieves repository reports from the DoWell Secure Github Repository.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
 # Example:
     
 ```python
 from doWellSecureGithubRepository import doWellSecureGithubRepository
-
 api = doWellSecureGithubRepository(api_key)
 api.clone_repository(repository_url)
 api.get_backup_reports()
 api.get_repository_reports()
 ```
     
-# API Reference:
+# Library Reference:
 - `doWellSecureGithubRepository` class:
     - `__init__(api_key)`: Initializes the `doWellSecureGithubRepository` object with the API key.
     - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
     - `get_backup_reports()`: Retrieves backup reports.
     - `get_repository_reports()`: Retrieves repository reports.
 # Configuration:
 - The package requires a valid API key for authentication.
 # Dependencies:
 - requests: Required for making HTTP requests.
 - json: Required for parsing JSON data.
 # Support:
 - For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
-- If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
+- If you encounter any issues, have questions, or need assistance with the  DoWell Secure Github Repository library, please contact our support team.
 # License:
-- Apache License 2.0
+- Apache License 2.0
+
+# Powered by [DoWell UX Living Lab](https://uxlivinglab.com/en/)
```

### Comparing `Dowell secure github repository-0.6.0/README.md` & `DoWell Secure Github Repository-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# Version: 0.6.0
+# DoWell Secure Github Repository 
+# Version: 1.0.0
 # Description:
 This Package seamlessly integrates with Github's webhooks, enabling automatic backups of code repositories. It provides real-time backups triggered by specified events, ensuring data protection. The Package offers customization options, allowing developers to define backup frequency and scope. With robust encryption and disaster recovery mechanisms, the Secure Repository Package ensures the integrity and availability of your code backups.
 
-The Secure Repository Package offers a range of powerful features to enhance code backup:
+The  DoWell Secure Github Repository Package offers a range of powerful features to enhance code backup:
 
-- Repository Clone: The Package enables easy cloning of repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
+- Repository Clone: The Package enables easy cloning of public repositories, allowing you to create copies of your codebase. This functionality ensures that you have a complete and up-to-date backup of your repositories, ready for immediate use or restoration.
 - Webhooks Integration: With seamless integration with Github's webhooks, the Package automatically triggers backups based on specified events. Whether it's a new commit, branch update, or pull request, the Package captures these changes in real-time, ensuring that your backups are always up to date.
-- Backup Reports: The Secure Repository Package generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
+- Backup Reports: The  DoWell Secure Github Repository Package generates comprehensive backup reports, providing valuable insights into the status and success of each backup operation. These reports include details such as backup timestamps, repository names, and any potential errors encountered during the backup process. These reports serve as a handy reference for tracking backup history and troubleshooting.
 - Repository Reports: In addition to backup reports, the Package also generates repository reports, offering an overview of each repository's status and health. These reports provide information such as the number of commits, branches, and contributors, giving you a clear snapshot of your codebase's activity and progress.
 # Installation:
 - Install the package using pip: 
 ```python
 pip install Dowell-secure-github-repository
 ```
         
@@ -28,57 +29,58 @@
     - `get_repository_reports()`: Retrieves repository reports.
     - `__init__(self, api_key)`
         
         Description: Initializes an instance of the doWellSecureGithubRepository class.
         
         Parameters:
         
-        - `api_key` (str): The API key required for authentication with the Secure Repository API.
+        - `api_key` (str): The API key required for authentication with the DoWell Secure Github Repository.
     - `clone_repository(self, repository_url)`
         
-        Description: Clones a GitHub repository by making a POST request to the Secure Repository API.
+        Description: Clones a GitHub repository.
         
         Parameters:
         
         - `repository_url` (str): The URL of the GitHub repository to clone.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
     - `get_backup_reports(self)`
         
-        Description: Retrieves backup reports from the Secure Repository API by making a      GET request.
+        Description: Retrieves backup reports from the DoWell Secure Github Repository.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
     - `get_repository_reports(self)`
         
-        Description: Retrieves repository reports from the Secure Repository API by making a GET request.
+        Description: Retrieves repository reports from the DoWell Secure Github Repository.
         
-        Returns: The response from the API as a JSON object.
+        Returns: The response from the library as a JSON object.
         
 # Example:
     
 ```python
 from doWellSecureGithubRepository import doWellSecureGithubRepository
-
 api = doWellSecureGithubRepository(api_key)
 api.clone_repository(repository_url)
 api.get_backup_reports()
 api.get_repository_reports()
 ```
     
-# API Reference:
+# Library Reference:
 - `doWellSecureGithubRepository` class:
     - `__init__(api_key)`: Initializes the `doWellSecureGithubRepository` object with the API key.
     - `clone_repository(repository_url)`: Clones a GitHub repository for backup.
     - `get_backup_reports()`: Retrieves backup reports.
     - `get_repository_reports()`: Retrieves repository reports.
 # Configuration:
 - The package requires a valid API key for authentication.
 # Dependencies:
 - requests: Required for making HTTP requests.
 - json: Required for parsing JSON data.
 # Support:
 - For detailed API documentation, including endpoint descriptions, request and response examples, and authentication details, please refer to the [API Documentation](https://github.com/DoWellUXLab).
-- If you encounter any issues, have questions, or need assistance with the Secure Repository API, please contact our support team.
+- If you encounter any issues, have questions, or need assistance with the  DoWell Secure Github Repository library, please contact our support team.
 # License:
-- Apache License 2.0
+- Apache License 2.0
+
+# Powered by [DoWell UX Living Lab](https://uxlivinglab.com/en/)
```

### Comparing `Dowell secure github repository-0.6.0/doWellSecureGithubRepository/doWellSecureGithubRepository.py` & `DoWell Secure Github Repository-1.0.0/doWellSecureGithubRepository/doWellSecureGithubRepository.py`

 * *Files identical despite different names*

