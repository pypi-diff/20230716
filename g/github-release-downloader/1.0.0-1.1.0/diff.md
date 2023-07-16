# Comparing `tmp/github_release_downloader-1.0.0.tar.gz` & `tmp/github_release_downloader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_release_downloader-1.0.0.tar", last modified: Sat Jul 15 20:25:28 2023, max compression
+gzip compressed data, was "github_release_downloader-1.1.0.tar", last modified: Sun Jul 16 19:55:53 2023, max compression
```

## Comparing `github_release_downloader-1.0.0.tar` & `github_release_downloader-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:25:28.984020 github_release_downloader-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-15 20:25:28.984020 github_release_downloader-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:25:28.984020 github_release_downloader-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:25:28.980019 github_release_downloader-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:25:28.980019 github_release_downloader-1.0.0/src/github_release_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/src/github_release_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/src/github_release_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/src/github_release_downloader/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/src/github_release_downloader/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/src/github_release_downloader/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-15 20:25:16.000000 github_release_downloader-1.0.0/src/github_release_downloader/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:25:28.984020 github_release_downloader-1.0.0/src/github_release_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-15 20:25:28.000000 github_release_downloader-1.0.0/src/github_release_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-15 20:25:28.000000 github_release_downloader-1.0.0/src/github_release_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:25:28.000000 github_release_downloader-1.0.0/src/github_release_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-15 20:25:28.000000 github_release_downloader-1.0.0/src/github_release_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 20:25:28.000000 github_release_downloader-1.0.0/src/github_release_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:55:53.608814 github_release_downloader-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-16 19:55:53.608814 github_release_downloader-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 19:55:53.608814 github_release_downloader-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:55:53.608814 github_release_downloader-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:55:53.608814 github_release_downloader-1.1.0/src/github_release_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/src/github_release_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/src/github_release_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/src/github_release_downloader/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/src/github_release_downloader/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/src/github_release_downloader/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-16 19:55:42.000000 github_release_downloader-1.1.0/src/github_release_downloader/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:55:53.608814 github_release_downloader-1.1.0/src/github_release_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-16 19:55:53.000000 github_release_downloader-1.1.0/src/github_release_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-16 19:55:53.000000 github_release_downloader-1.1.0/src/github_release_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:55:53.000000 github_release_downloader-1.1.0/src/github_release_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 19:55:53.000000 github_release_downloader-1.1.0/src/github_release_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 19:55:53.000000 github_release_downloader-1.1.0/src/github_release_downloader.egg-info/top_level.txt
```

### Comparing `github_release_downloader-1.0.0/LICENSE.md` & `github_release_downloader-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `github_release_downloader-1.0.0/PKG-INFO` & `github_release_downloader-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: github_release_downloader
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package to download any release assets from the latest compatible version
 Author: MaxBQb
 License: MIT license
+Project-URL: Homepage, https://github.com/MBQbUtils/GithubReleaseDownloader
+Project-URL: Bug Tracker, https://github.com/MBQbUtils/GithubReleaseDownloader/issues
 Keywords: github,release,download,asset,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -17,22 +19,22 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # GitHub Release Downloader
 [![PyPI version shields.io](https://img.shields.io/pypi/v/github_release_downloader.svg)](https://pypi.org/project/github_release_downloader/)
-[![GitHub license](https://img.shields.io/github/license/MBQbUtils/github_release_downloader.svg)](https://github.com/MaxBQb/github_release_downloader/blob/master/LICENSE.md)
+[![GitHub license](https://img.shields.io/github/license/MBQbUtils/GithubReleaseDownloader.svg)](https://github.com/MaxBQb/github_release_downloader/blob/master/LICENSE.md)
 ![Python versions](https://img.shields.io/pypi/pyversions/github_release_downloader.svg)
 ---
 Python package to download/filter any release assets from the latest compatible version.
 
 ## Installation
 ```cmd
-pip install github_release_downloader
+pip install github-release-downloader
 ```
 
 ## Usage
 
 This tool can be used as library:
 ```py
 from semantic_version import SimpleSpec
@@ -50,15 +52,15 @@
 ```
 Or either it can be used as cli-tool:
 ```cmd
 python -m github_release_downloader -u OwnerName -n RepoName -r ~1.1 -m .*\.exe -o .\downloads
 ```
 
 ## Features
-1. Downloads only compatible releases
+1. Downloads compatible releases (or latest if no requirements set)
 2. Filters assets using regex
 3. Has optional download_callback
 4. CLI tool can be used in CI
 5. Handles token from GITHUB_TOKEN env
 6. Loads updates only when it's needed (caches last version used)
 7. Loggs own actions
 8. Uses only few GitHub API endpoints (don't download code, you've never needed)
```

### Comparing `github_release_downloader-1.0.0/README.md` & `github_release_downloader-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # GitHub Release Downloader
 [![PyPI version shields.io](https://img.shields.io/pypi/v/github_release_downloader.svg)](https://pypi.org/project/github_release_downloader/)
-[![GitHub license](https://img.shields.io/github/license/MBQbUtils/github_release_downloader.svg)](https://github.com/MaxBQb/github_release_downloader/blob/master/LICENSE.md)
+[![GitHub license](https://img.shields.io/github/license/MBQbUtils/GithubReleaseDownloader.svg)](https://github.com/MaxBQb/github_release_downloader/blob/master/LICENSE.md)
 ![Python versions](https://img.shields.io/pypi/pyversions/github_release_downloader.svg)
 ---
 Python package to download/filter any release assets from the latest compatible version.
 
 ## Installation
 ```cmd
-pip install github_release_downloader
+pip install github-release-downloader
 ```
 
 ## Usage
 
 This tool can be used as library:
 ```py
 from semantic_version import SimpleSpec
@@ -29,15 +29,15 @@
 ```
 Or either it can be used as cli-tool:
 ```cmd
 python -m github_release_downloader -u OwnerName -n RepoName -r ~1.1 -m .*\.exe -o .\downloads
 ```
 
 ## Features
-1. Downloads only compatible releases
+1. Downloads compatible releases (or latest if no requirements set)
 2. Filters assets using regex
 3. Has optional download_callback
 4. CLI tool can be used in CI
 5. Handles token from GITHUB_TOKEN env
 6. Loads updates only when it's needed (caches last version used)
 7. Loggs own actions
 8. Uses only few GitHub API endpoints (don't download code, you've never needed)
```

### Comparing `github_release_downloader-1.0.0/pyproject.toml` & `github_release_downloader-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -19,12 +19,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
+[project.urls]
+"Homepage" = "https://github.com/MBQbUtils/GithubReleaseDownloader"
+"Bug Tracker" = "https://github.com/MBQbUtils/GithubReleaseDownloader/issues"
 [options.entry_points]
 console_scripts = {github_release_downloader = "github_release_downloader:__main__"}
 [tool.setuptools.dynamic]
 version = {attr = "github_release_downloader._meta.__version__"}
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `github_release_downloader-1.0.0/src/github_release_downloader/core.py` & `github_release_downloader-1.1.0/src/github_release_downloader/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,57 +39,69 @@
         format="[%(asctime)s][%(levelname)s] %(message)s",
         datefmt='%H:%M:%S',
         level=logging.INFO
     )
     args = get_args()
     check_and_download_updates(
         GitHubRepo(args.user, args.repo_name, args.token),
-        SimpleSpec(args.require),
+        SimpleSpec(args.require) if args.require else None,
         assets_mask=re.compile(args.mask),
         current_version=Version(args.current_version) if args.current_version else None,
         downloads_dir=Path(args.output_dir)
     )
 
 
 def check_and_download_updates(
     repo: GitHubRepo,
-    compatibility_spec: SimpleSpec,
+    compatibility_spec: SimpleSpec = None,
     current_version: Version = None,
     assets_mask=re.compile('.*'),
     downloads_dir=Path(),
     download_callback: Callable[[ReleaseAsset, int], None] = None
 ):
     if download_callback is None:
         download_callback = default_download_callback
     cache = Cache(f"repo-{repo.user}-{repo.repo}.cache")
     if current_version is None:
         current_version = cache.version
         if current_version is None:
             current_version = Version("0.0.0")
     AuthSession.init(repo)
-    logging.info(f"Compatibility requirement: '{compatibility_spec}'")
-
-    versions = list(sorted(compatibility_spec.filter(get_available_versions(repo)))[-10:])
-    if not versions:
-        logging.warning(f"No newer compatible versions available.")
+    if compatibility_spec is None:
+        logging.info(f"No compatibility requirements set")
+        download_version = get_latest_version(repo)
+    else:
+        logging.info(f"Compatibility requirement: '{compatibility_spec}'")
+        download_version = get_compatible_version(repo, compatibility_spec)
+
+    if download_version is None:
+        compatible = " compatible" if compatibility_spec is not None else ""
+        logging.warning(f"No newer{compatible} versions available.")
         return
-    logging.info(f"Available versions: {tuple(map(str, versions))}")
-    download_version = versions[-1]
+
     if is_already_installed(download_version, current_version, compatibility_spec):
         return
     tag_name = getattr(download_version, '_origin_tag_name', str(download_version))
     assets = get_assets(repo, tag_name, assets_mask)
     if not assets:
         logging.error(f"No assets found")
         return
     download_assets(assets, out_dir=downloads_dir, callback=download_callback)
     logging.info(f"Done!")
     cache.version = download_version
 
 
+def get_compatible_version(repo: GitHubRepo, compatibility_spec: SimpleSpec):
+    versions = sorted(compatibility_spec.filter(get_available_versions(repo)))[-10:]
+    if not versions:
+        return
+    logging.info(f"Available versions: {tuple(map(str, versions))}")
+    return versions[-1]
+
+
 def download_assets(
     assets: typing.Iterable[ReleaseAsset],
     out_dir=Path(),
     block_size=2**20,
     callback: Callable[[ReleaseAsset, int], None] = lambda _, __: None
 ):
     logging.info(f"Start downloading assets: {tuple(asset.name for asset in assets)}")
@@ -143,14 +155,30 @@
             yield version
         logging.info(f"Version's page#{i} loaded")
         if len(data) < page_size:
             logging.info(f"No more pages")
             break
 
 
+def get_latest_version(repo: GitHubRepo, process_tag: Callable[[str], Version] = None):
+    if process_tag is None:
+        process_tag = parse_tag
+    logging.info(f"Searching for latest release in 'https://github.com/{repo.user}/{repo.repo}/'...")
+    request_url = f"https://api.github.com/repos/{repo.user}/{repo.repo}/releases/latest"
+    data = json.loads(requests.get(request_url, headers=AuthSession.header).text)
+    if 'message' in data:
+        return
+    tag_name = data.get("tag_name")
+    if tag_name is None:
+        return
+    version = process_tag(tag_name)
+    version._origin_tag_name = tag_name
+    return version
+
+
 def parse_tag(tag_name: str):
     return Version(tag_name.lstrip("v").strip())
 
 
 def get_assets(repo: GitHubRepo, tag_name: str, assets_mask=re.compile('.*')):
     logging.info(f"Searching for assets by tag '{tag_name}' and mask: '{assets_mask.pattern}'")
     request_url = f"https://api.github.com/repos/{repo.user}/{repo.repo}/releases/tags/{tag_name}"
```

### Comparing `github_release_downloader-1.0.0/src/github_release_downloader/data.py` & `github_release_downloader-1.1.0/src/github_release_downloader/data.py`

 * *Files identical despite different names*

### Comparing `github_release_downloader-1.0.0/src/github_release_downloader.egg-info/PKG-INFO` & `github_release_downloader-1.1.0/src/github_release_downloader.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: github-release-downloader
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package to download any release assets from the latest compatible version
 Author: MaxBQb
 License: MIT license
+Project-URL: Homepage, https://github.com/MBQbUtils/GithubReleaseDownloader
+Project-URL: Bug Tracker, https://github.com/MBQbUtils/GithubReleaseDownloader/issues
 Keywords: github,release,download,asset,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -17,22 +19,22 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # GitHub Release Downloader
 [![PyPI version shields.io](https://img.shields.io/pypi/v/github_release_downloader.svg)](https://pypi.org/project/github_release_downloader/)
-[![GitHub license](https://img.shields.io/github/license/MBQbUtils/github_release_downloader.svg)](https://github.com/MaxBQb/github_release_downloader/blob/master/LICENSE.md)
+[![GitHub license](https://img.shields.io/github/license/MBQbUtils/GithubReleaseDownloader.svg)](https://github.com/MaxBQb/github_release_downloader/blob/master/LICENSE.md)
 ![Python versions](https://img.shields.io/pypi/pyversions/github_release_downloader.svg)
 ---
 Python package to download/filter any release assets from the latest compatible version.
 
 ## Installation
 ```cmd
-pip install github_release_downloader
+pip install github-release-downloader
 ```
 
 ## Usage
 
 This tool can be used as library:
 ```py
 from semantic_version import SimpleSpec
@@ -50,15 +52,15 @@
 ```
 Or either it can be used as cli-tool:
 ```cmd
 python -m github_release_downloader -u OwnerName -n RepoName -r ~1.1 -m .*\.exe -o .\downloads
 ```
 
 ## Features
-1. Downloads only compatible releases
+1. Downloads compatible releases (or latest if no requirements set)
 2. Filters assets using regex
 3. Has optional download_callback
 4. CLI tool can be used in CI
 5. Handles token from GITHUB_TOKEN env
 6. Loads updates only when it's needed (caches last version used)
 7. Loggs own actions
 8. Uses only few GitHub API endpoints (don't download code, you've never needed)
```

### Comparing `github_release_downloader-1.0.0/src/github_release_downloader.egg-info/SOURCES.txt` & `github_release_downloader-1.1.0/src/github_release_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

