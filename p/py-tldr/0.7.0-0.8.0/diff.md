# Comparing `tmp/py-tldr-0.7.0.tar.gz` & `tmp/py-tldr-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-tldr-0.7.0.tar", last modified: Fri Mar 10 03:56:13 2023, max compression
+gzip compressed data, was "py-tldr-0.8.0.tar", last modified: Sun Jul 16 04:54:53 2023, max compression
```

## Comparing `py-tldr-0.7.0.tar` & `py-tldr-0.8.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:56:13.932835 py-tldr-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-10 03:56:03.000000 py-tldr-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-10 03:56:13.928835 py-tldr-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-10 03:56:03.000000 py-tldr-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-10 03:56:03.000000 py-tldr-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 03:56:13.932835 py-tldr-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:56:13.928835 py-tldr-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:56:13.928835 py-tldr-0.7.0/src/py_tldr/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-10 03:56:03.000000 py-tldr-0.7.0/src/py_tldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-03-10 03:56:03.000000 py-tldr-0.7.0/src/py_tldr/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-03-10 03:56:03.000000 py-tldr-0.7.0/src/py_tldr/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:56:13.928835 py-tldr-0.7.0/src/py_tldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-10 03:56:13.000000 py-tldr-0.7.0/src/py_tldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-10 03:56:13.000000 py-tldr-0.7.0/src/py_tldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 03:56:13.000000 py-tldr-0.7.0/src/py_tldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-10 03:56:13.000000 py-tldr-0.7.0/src/py_tldr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-10 03:56:13.000000 py-tldr-0.7.0/src/py_tldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-10 03:56:13.000000 py-tldr-0.7.0/src/py_tldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 03:56:13.928835 py-tldr-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-03-10 03:56:03.000000 py-tldr-0.7.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 04:54:42.000000 py-tldr-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-16 04:54:53.535751 py-tldr-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-16 04:54:42.000000 py-tldr-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-16 04:54:42.000000 py-tldr-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:54:53.535751 py-tldr-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.531751 py-tldr-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/src/py_tldr/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-16 04:54:42.000000 py-tldr-0.8.0/src/py_tldr/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/src/py_tldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 04:54:53.000000 py-tldr-0.8.0/src/py_tldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:54:53.535751 py-tldr-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-16 04:54:42.000000 py-tldr-0.8.0/tests/test_cli.py
```

### Comparing `py-tldr-0.7.0/PKG-INFO` & `py-tldr-0.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tldr
-Version: 0.7.0
+Version: 0.8.0
 Summary: New Python client for tldr pages
 Author-email: iamgodot <xugodot@gmail.com>
 License: MIT
 Project-URL: Issue Tracker, https://github.com/iamgodot/py-tldr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Py-tldr
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
-[![test](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml)
+[![test](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml)
 
 Py-tldr is a new Python client for [tldr pages](https://github.com/tldr-pages/tldr) based on [Click](https://github.com/pallets/click).
 
 ![](images/demo.gif)
 
 ## Installation
 
@@ -53,20 +53,21 @@
 ```
 
 Config file should be located as `~/.config/tldr/config.toml`, you can use `--edit-config` to create a default one, which will contain the following content:
 
 ```toml
 page_source = "https://raw.githubusercontent.com/tldr-pages/tldr/main/pages"
 language = "en"
+platform = 'linux'
 proxy_url = ""
 
 [cache]
 enabled = true
 timeout = 24
-download_url = "https://tldr-pages.github.io/assets/tldr.zip"
+download_url = "https://tldr.sh/assets/tldr.zip"
 ```
 
 Cache is enabled implicitly, with 24 hours as expiration time by default.
 
 A proxy url can be set for convenience, proxy envs such as `HTTP_PROXY` will also work.
 
 ## Support
@@ -81,8 +82,8 @@
 
 ## License
 
 [MIT](docs/LICENSE)
 
 ## Credits
 
-This package was created with [cookiecutter](https://github.com/audreyr/cookiecutter) and [iamgodot/gen-pyckage](https://github.com/iamgodot/gen-pyckage) project template.
+This package was created with [cookiecutter](https://github.com/audreyr/cookiecutter) and [iamgodot/create-python-app](https://github.com/iamgodot/create-python-app) project template.
```

### Comparing `py-tldr-0.7.0/README.md` & `py-tldr-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Py-tldr
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
-[![test](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml)
+[![test](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml)
 
 Py-tldr is a new Python client for [tldr pages](https://github.com/tldr-pages/tldr) based on [Click](https://github.com/pallets/click).
 
 ![](images/demo.gif)
 
 ## Installation
 
@@ -38,20 +38,21 @@
 ```
 
 Config file should be located as `~/.config/tldr/config.toml`, you can use `--edit-config` to create a default one, which will contain the following content:
 
 ```toml
 page_source = "https://raw.githubusercontent.com/tldr-pages/tldr/main/pages"
 language = "en"
+platform = 'linux'
 proxy_url = ""
 
 [cache]
 enabled = true
 timeout = 24
-download_url = "https://tldr-pages.github.io/assets/tldr.zip"
+download_url = "https://tldr.sh/assets/tldr.zip"
 ```
 
 Cache is enabled implicitly, with 24 hours as expiration time by default.
 
 A proxy url can be set for convenience, proxy envs such as `HTTP_PROXY` will also work.
 
 ## Support
@@ -66,8 +67,8 @@
 
 ## License
 
 [MIT](docs/LICENSE)
 
 ## Credits
 
-This package was created with [cookiecutter](https://github.com/audreyr/cookiecutter) and [iamgodot/gen-pyckage](https://github.com/iamgodot/gen-pyckage) project template.
+This package was created with [cookiecutter](https://github.com/audreyr/cookiecutter) and [iamgodot/create-python-app](https://github.com/iamgodot/create-python-app) project template.
```

### Comparing `py-tldr-0.7.0/pyproject.toml` & `py-tldr-0.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+[tool.pyright]
+extraPaths = ["__pypackages__/3.11/lib/"]
+
 [tool.pdm]
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.2.1",
     "pytest-mock>=3.10.0",
     "pytest-cov>=4.0.0",
-    "flake8>=5.0.4",
-    "tox>=3.28.0",
+    "black",
+    "ruff",
 ]
 
 [project]
 name = "py-tldr"
 description = "New Python client for tldr pages"
 readme = "README.md"
 license = {text = "MIT"}
@@ -48,29 +51,27 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["py_tldr", "tests"]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-envlist = py{37,38,39}
-isolated_build = True
-[testenv]
-passenv = PYTHONPATH
-deps = pdm
-commands = 
-    pdm install --dev
-    make clean
-	  pdm run flake8 --format=pylint --count
-    pdm run pytest -v --cov={envsitepackagesdir}/py_tldr tests/unit
-allowlist_externals = make
-"""
+[tool.black]
+line-length = 88
+include = '\.pyi?$'
+
+[tool.ruff]
+select = ["E", "F", "I"]
+exclude = [".git", ".tox", "venv", "build", "__pypackages__"]
+line-length = 88
+per-file-ignores = {"src/py_tldr/__init__.py" = ["F401"]}
+src = ["src", "tests"]
+
+[tool.ruff.isort]
+known-first-party = ["py_tldr"]
 
 [tool.tbump]
 github_url = "https://github.com/iamgodot/py-tldr"
 
 [tool.tbump.version]
 current = "0.7.0"
 
@@ -87,8 +88,8 @@
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
 src = "src/py_tldr/__init__.py"
 
 [[tool.tbump.before_commit]]
 name = "Check changelog"
-cmd = "grep -q {new_version} docs/CHANGELOG.md"
+cmd = "grep -q {new_version} docs/CHANGELOG.md"
```

### Comparing `py-tldr-0.7.0/src/py_tldr/core.py` & `py-tldr-0.8.0/src/py_tldr/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-import platform as platform_
 import subprocess
 import sys
+from copy import deepcopy
 from functools import partial
 from os import environ
 from pathlib import Path as LibPath
-from typing import List
 
 import toml
-from click import Choice, argument
+from click import Choice, argument, option, pass_context, secho
 from click import command as command_
-from click import option, pass_context, secho
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
 from .page import DownloadError, PageFinder, PageFormatter
+from .parse import parse_command, parse_language, parse_platform
 
 try:
     from importlib.metadata import version
 
     VERSION_CLI = version("py_tldr")
 except ModuleNotFoundError:
-    from pkg_resources import get_distribution
+    try:
+        from pkg_resources import get_distribution
 
-    VERSION_CLI = get_distribution("py_tldr").version
+        VERSION_CLI = get_distribution("py_tldr").version
+    except ModuleNotFoundError:
+        VERSION_CLI = ""
 
 VERSION_CLIENT_SPEC = "1.5"
 DEFAULT_CACHE_HOURS = 24
 DEFAULT_CONFIG = {
     "page_source": "https://raw.githubusercontent.com/tldr-pages/tldr/main/pages",
     "language": "",
+    "platform": "",
     "cache": {
         "enabled": True,
         "timeout": DEFAULT_CACHE_HOURS,
-        "download_url": "https://tldr-pages.github.io/assets/tldr.zip",
+        "download_url": "https://tldr.sh/assets/tldr.zip",
     },
     "proxy_url": "",
 }
 DEFAULT_CONFIG_EDITOR = "vi"
-DEFAULT_CONFIG_FILE = LibPath.home() / ".config/tldr/config.toml"
+DEFAULT_CONFIG_DIR = LibPath.home() / ".config" / "tldr"
+DEFAULT_CONFIG_FILE = DEFAULT_CONFIG_DIR / "config.toml"
 DEFAULT_CACHE_DIR = LibPath.home() / ".cache" / "tldr"
 
+DEFAULT_CONFIG_DIR.mkdir(parents=True, exist_ok=True)
+DEFAULT_CACHE_DIR.mkdir(parents=True, exist_ok=True)
+
 info = partial(secho, bold=True, fg="green")
 warn = partial(secho, bold=True, fg="yellow")
 
 
 def print_version(ctx, param, value):  # pylint: disable=unused-argument
     if not value or ctx.resilient_parsing:
         return
@@ -71,15 +78,15 @@
 def setup_config():  # pylint: disable=unused-argument
     """Build a config dict from config file on top of default settings.
 
     Note `toml` should used as file format.
     Raises:
       SystemExit: if merged config checking failed.
     """
-    config = DEFAULT_CONFIG
+    config = deepcopy(DEFAULT_CONFIG)
     config_file = DEFAULT_CONFIG_FILE
     if config_file.exists():
         warn(f"Found config file: {config_file}")
         with open(config_file, encoding="utf8") as f:
             config.update(toml.load(f))
     cache = config.get("cache")
     if not config.get("page_source") or not cache or not cache.get("download_url"):
@@ -105,59 +112,59 @@
     is_eager=True,
     expose_value=False,
     help="Open config file with an editor.",
 )
 @option(
     "-p",
     "--platform",
-    type=Choice(["android", "common", "linux", "osx", "sunos", "windows"]),
-    help="Override current operating system.",
+    type=Choice(["android", "linux", "macos", "osx", "sunos", "windows"]),
+    default="linux",
+    help="Specify searching platform(macos as an alias of osx).",
 )
 @option(
     "-L",
     "--language",
-    help="Specify language of the page(with no fallbacks), e.g. `en`.",
+    default="en",
+    help="Specify searching language(with no fallbacks), e.g. `en`.",
 )
 @option("-u", "--update", is_flag=True, help="Update local cache with all pages.")
 @argument("command", nargs=-1)
 @pass_context
 def cli(ctx, command, platform, language, update):
     """Collaborative cheatsheets for console commands.
 
     For subcommands such as `git commit`, just keep as it is:
 
         tldr git commit
     """
     config = setup_config()
     page_finder = make_page_finder(config)
 
+    languages = parse_language(language, config)
     if update:
         with yaspin(Spinners.arc, text="Downloading pages...") as sp:
             try:
-                page_finder.sync()
+                page_finder.sync(languages[0])
             except DownloadError:
                 sp.write("> Sync failed, check your network and try again.")
                 sys.exit(1)
             sp.write("> Download complete.")
         info("All caches updated.")
 
     if not command:
         if not update:
             secho(ctx.get_help())
         return
-    else:
-        command = "-".join(command)
 
+    command = parse_command(command)
+    platform = parse_platform(platform, config)
     content = None
-    languages = get_languages(language)
     with yaspin(Spinners.arc, text="Searching pages...") as sp:
         try:
-            content = page_finder.find(
-                command, platform or guess_os(), languages=languages
-            )
+            content = page_finder.find(command, platform, languages=languages)
         except DownloadError:
             sp.write("> Search failed, check your network and try again.")
             sys.exit(1)
         if content:
             sp.write("> Page found.")
         else:
             sp.write("> No result.")
@@ -184,45 +191,7 @@
         source_url,
         cache_timeout,
         cache_location,
         cache_download_url,
         cache_enabled,
         proxy_url,
     )
-
-
-def get_languages(language: str) -> List[str]:
-    """Return language list for page matching.
-
-    If language specified, use it with no fallbacks.
-    Otherwise make the list based on env `LANG` and
-    `LANGUAGE`.
-    # pylint: disable=line-too-long
-    For detailed logic, see https://github.com/tldr-pages/tldr/blob/main/CLIENT-SPECIFICATION.md#language  # noqa
-    """
-    if language:
-        return [language]
-
-    def extractor(x):
-        return x.split("_", maxsplit=1)[0]
-
-    lang = extractor(environ.get("LANG", ""))
-    if not lang:
-        return ["en"]
-    languages = [
-        extractor(item) for item in environ.get("LANGUAGE", "").split(":") if item
-    ]
-    if lang not in languages:
-        languages.append(lang)
-    if "en" not in languages:
-        languages.append("en")
-    return languages
-
-
-def guess_os():
-    system_to_platform = {
-        "Linux": "linux",
-        "Darwin": "osx",
-        "Java": "sunos",
-        "Windows": "windows",
-    }
-    return system_to_platform.get(platform_.system(), "linux")
```

### Comparing `py-tldr-0.7.0/src/py_tldr/page.py` & `py-tldr-0.8.0/src/py_tldr/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+import json
 from datetime import datetime
 from http import HTTPStatus
+from logging import getLogger
 from pathlib import Path as LibPath
-from typing import List
+from shutil import rmtree
+from typing import Dict, List, Tuple
 from zipfile import ZipFile
 
 import requests
 from click import style
 from requests.exceptions import ConnectionError as ConnectionError_
 from requests.exceptions import HTTPError, Timeout
 
+LOGGER = getLogger(__name__)
+
 
 class PageCache:
     """PageCache intends to manage local cache data.
 
     It provides instant search among downloaded page files, while
     should not have direct interactions with PageFinder.
 
@@ -57,29 +62,55 @@
 
     def set(self, name: str, platform: str, content: str, language: str = "en"):
         (self.location / platform).mkdir(parents=True, exist_ok=True)
         page_file = self._make_page_file(platform, name, language)
         with open(page_file, "w", encoding="utf8") as f:
             f.write(content)
 
-    def update(self):
-        """Download all latest pages."""
+    def update(self, language: str):
+        """Download pages for specified language."""
+        LOGGER.debug("Update cache for language: %s", language)
         data = download_data(self.download_url, proxies={"https": self.proxy_url})
         tldr_zip = self.location_base / "tldr.zip"
         with open(tldr_zip, "wb") as f:
             f.write(data)
 
         with ZipFile(tldr_zip, "r") as f:
             f.extractall(self.location_base)
 
         # Remove non-page files, such as tldr.zip, index.json and LICENSE.md
+        # Also remove page dirs of other languages
         tldr_zip.unlink()
+        dir_to_reserve = "pages" if language == "en" else f"pages.{language}"
         for item in self.location_base.iterdir():
             if item.is_file():
                 item.unlink()
+            elif item.name != dir_to_reserve:
+                rmtree(item)
+
+    @property
+    def index_file(self) -> LibPath:
+        return LibPath(self.location_base) / "index.json"
+
+    def check_index(self) -> bool:
+        return self._validate_page_file(self.index_file)
+
+    def update_index(self) -> None:
+        """Download newest index.json and restructure it for better searching."""
+        data = download_data(
+            "https://tldr.sh/assets/index.json", proxies={"https": self.proxy_url}
+        )
+        index, index_compact = json.loads(data), {}
+        for command in index["commands"]:
+            index_compact[command["name"]] = {
+                "platforms": command["platform"],
+                "languages": command["language"],
+            }
+        with open(self.index_file, "w") as f:
+            json.dump(index_compact, f)
 
 
 class DownloadError(Exception):
     def __init__(self, *args, status_code: int = 0, **kwargs):
         self.status_code = status_code
         super().__init__(*args, **kwargs)
 
@@ -128,52 +159,69 @@
 
     def _make_page_url(self, name: str, platform: str, language: str) -> str:
         postfix_lang = f".{language}" if language != "en" else ""
         return "/".join([self.source_url + postfix_lang, platform, name + ".md"])
 
     def _query(self, url: str) -> str:
         try:
+            LOGGER.debug("Query URL: %s", url)
             data = download_data(url, proxies={"https": self.proxy_url})
         except DownloadError as exc:
             if exc.status_code == HTTPStatus.NOT_FOUND:
                 return ""
             raise exc
         return data.decode(encoding="utf8")
 
     def find(self, name: str, platform: str = "", languages: List[str] = None) -> str:
-        """Find named page based on given platform and language list.
-
-        Tldr merges shared entries under `common` folder, so it's added
-        as a fallback for platform.
-        For each combination of platform and language, following steps
-        will be applied to perform matching:
-
-            1. Query cache if enabled, return if result found.
-            2. Query source.
-            3. If matched, set cache if enabled, and simply return.
-            4. Otherwise try next combination.
-        """
-        platform = platform or "common"
-        platforms = [platform, "common"] if platform != "common" else [platform]
-        languages = languages or ["en"]
-        for pf in platforms:
-            for lang in languages:
-                if self.cache_enabled:
-                    content = self.cache.get(name, pf, language=lang)
-                    if content:
-                        return content
-                content = self._query(self._make_page_url(name, pf, lang))
-                if content:
-                    if self.cache_enabled:
-                        self.cache.set(name, pf, content, language=lang)
-                    return content
-        return ""
-
-    def sync(self) -> None:
-        self.cache.update()
+        """Find page content via local cache and source."""
+        if not self.cache.check_index():
+            self.cache.update_index()
+        LOGGER.debug("Page find for: %s, %s, %s", name, platform, languages)
+        name, platform, language = self.search(name, platform, languages)
+        if not name or not platform or not language:
+            return ""
+        LOGGER.debug("Search result: %s, %s, %s", name, platform, language)
+        if self.cache_enabled:
+            content = self.cache.get(name, platform, language=language)
+            if content:
+                LOGGER.debug("Cache enabled and hit!")
+                return content
+        content = self._query(self._make_page_url(name, platform, language)) or ""
+        if content and self.cache_enabled:
+            self.cache.set(name, platform, content, language=language)
+        return content
+
+    def get_index(self) -> Dict:
+        with open(self.cache.index_file) as f:
+            return json.load(f)
+
+    def search(
+        self, name: str, platform: str = "", languages: List[str] = None
+    ) -> Tuple[str, str, str]:
+        """Search index for the best platform and language for the command."""
+        index = self.get_index()
+        info = index.get(name)
+        if not info:
+            return "", "", ""
+
+        platforms = info["platforms"]
+        if platform not in platforms:
+            platform = "common" if "common" in platforms else platforms[0]
+
+        language = ""
+        languages_info = info["languages"]
+        for lang in languages:
+            if lang in languages_info:
+                language = lang
+                break
+        return name, platform, language
+
+    def sync(self, language: str) -> None:
+        self.cache.update(language)
+        self.cache.update_index()
 
 
 class Formatter:
     """Formatter decides how text contents are displayed.
 
     Methods:
         format: This should be the only method to use a formatter. To each line
```

### Comparing `py-tldr-0.7.0/src/py_tldr.egg-info/PKG-INFO` & `py-tldr-0.8.0/src/py_tldr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tldr
-Version: 0.7.0
+Version: 0.8.0
 Summary: New Python client for tldr pages
 Author-email: iamgodot <xugodot@gmail.com>
 License: MIT
 Project-URL: Issue Tracker, https://github.com/iamgodot/py-tldr/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Py-tldr
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
-[![test](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml)
+[![test](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/iamgodot/py-tldr/actions/workflows/test.yml)
 
 Py-tldr is a new Python client for [tldr pages](https://github.com/tldr-pages/tldr) based on [Click](https://github.com/pallets/click).
 
 ![](images/demo.gif)
 
 ## Installation
 
@@ -53,20 +53,21 @@
 ```
 
 Config file should be located as `~/.config/tldr/config.toml`, you can use `--edit-config` to create a default one, which will contain the following content:
 
 ```toml
 page_source = "https://raw.githubusercontent.com/tldr-pages/tldr/main/pages"
 language = "en"
+platform = 'linux'
 proxy_url = ""
 
 [cache]
 enabled = true
 timeout = 24
-download_url = "https://tldr-pages.github.io/assets/tldr.zip"
+download_url = "https://tldr.sh/assets/tldr.zip"
 ```
 
 Cache is enabled implicitly, with 24 hours as expiration time by default.
 
 A proxy url can be set for convenience, proxy envs such as `HTTP_PROXY` will also work.
 
 ## Support
@@ -81,8 +82,8 @@
 
 ## License
 
 [MIT](docs/LICENSE)
 
 ## Credits
 
-This package was created with [cookiecutter](https://github.com/audreyr/cookiecutter) and [iamgodot/gen-pyckage](https://github.com/iamgodot/gen-pyckage) project template.
+This package was created with [cookiecutter](https://github.com/audreyr/cookiecutter) and [iamgodot/create-python-app](https://github.com/iamgodot/create-python-app) project template.
```

