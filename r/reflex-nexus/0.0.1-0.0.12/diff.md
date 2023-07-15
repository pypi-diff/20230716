# Comparing `tmp/reflex_nexus-0.0.1.tar.gz` & `tmp/reflex_nexus-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_nexus-0.0.1.tar", max compression
+gzip compressed data, was "reflex_nexus-0.0.12.tar", max compression
```

## Comparing `reflex_nexus-0.0.1.tar` & `reflex_nexus-0.0.12.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0     1066 2023-07-15 18:27:12.733718 reflex_nexus-0.0.1/LICENSE
--rw-r--r--   0        0        0     5530 2023-07-15 18:27:12.733718 reflex_nexus-0.0.1/README.md
--rw-r--r--   0        0        0     1565 2023-07-15 18:27:12.733718 reflex_nexus-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      885 2023-07-15 18:27:12.733718 reflex_nexus-0.0.1/reflex_nexus.py
--rw-r--r--   0        0        0     6334 1970-01-01 00:00:00.000000 reflex_nexus-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-15 22:14:30.756497 reflex_nexus-0.0.12/LICENSE
+-rw-r--r--   0        0        0     5656 2023-07-15 22:14:30.756497 reflex_nexus-0.0.12/README.md
+-rw-r--r--   0        0        0     1564 2023-07-15 22:14:30.756497 reflex_nexus-0.0.12/pyproject.toml
+-rw-r--r--   0        0        0     1150 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/application.py
+-rw-r--r--   0        0        0        0 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/device_registry.py
+-rw-r--r--   0        0        0      541 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/logger.py
+-rw-r--r--   0        0        0      732 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/main_window.py
+-rw-r--r--   0        0        0      931 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/menu_bar.py
+-rw-r--r--   0        0        0      369 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/stylesheet.qss
+-rw-r--r--   0        0        0      938 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/app/widget_registry.py
+-rw-r--r--   0        0        0     1327 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/devices/reflex_v2.py
+-rw-r--r--   0        0        0      117 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/drivers/usb_hid.py
+-rw-r--r--   0        0        0      380 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/widgets/log_viewer.py
+-rw-r--r--   0        0        0      883 2023-07-15 22:14:30.760497 reflex_nexus-0.0.12/src/widgets/pad_interface.py
+-rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 reflex_nexus-0.0.12/PKG-INFO
```

### Comparing `reflex_nexus-0.0.1/LICENSE` & `reflex_nexus-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_nexus-0.0.1/README.md` & `reflex_nexus-0.0.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [![][linux-badge]][Releases] [![][macos-badge]][Releases]
 [![][windows-badge]][Releases] [![][pypi-badge]][pypi]
 [![][docs-badge]][Documentation] [![][lint-badge]][lint]
 [![][test-badge]][test] [![][coverage-badge]][coverage]
 [![][license-badge]][LICENSE] [![][tag-badge]][tag]
 [![][discord-badge]][discord]
 
+__Note: This is a work in progress project. References made in the readme__
+__and documentation are currently unfulfilled.__
+
 # RE:Flex Nexus - Universal Dance Pad Utilities
 
 RE:Flex Nexus aims to provide a comprehensive collection of PC software
 utilities for dance pads. The interface specification is flexible, allowing
 any dance pad to be quickly integrated and begin using available software
 features.
 
@@ -18,17 +21,17 @@
 will hopefully inspire creativity/freedom, while letting dance gamers share
 technology together.
 
 ## Installation
 
 - The latest executable can be found on the [Releases] page
 - Download the application for your respective operating system
-- Download the `nexus_resources.zip` package and extract to the location
+- Download the `nexus-resources.zip` package and extract to the location
 you would like to store program data
-- Open the `reflex_nexus` application
+- Open the `reflex-nexus` application
 - You will be prompted to set up your program data folder, enter the directory
 of the folder that you just extracted
 
 ## Usage
 
 For details on usage, check out the [Documentation].
 
@@ -96,15 +99,15 @@
 [coverage]: https://coveralls.io/github/ReflexCreations/Nexus
 [discord]: https://discord.gg/TCn3emnwZU
 [Documentation]: https://reflex-nexus.readthedocs.io/
 [Git]: https://git-scm.com/downloads/
 [LICENSE]: https://github.com/ReflexCreations/Nexus/LICENSE
 [lint]: https://github.com/ReflexCreations/Nexus/actions/workflows/lint.yml
 [Python]: https://python.org/downloads/
-[pypi]: https://pypi.org/project/reflex_nexus
+[pypi]: https://pypi.org/project/reflex-nexus
 [Releases]: https://github.com/ReflexCreations/Nexus/releases/
 [tag]: https://github.com/ReflexCreations/Nexus/tags
 [test]: https://github.com/ReflexCreations/Nexus/actions/workflows/test.yml
 
 <!--- Runtime dependency links -->
 
 [libusb-package]: https://pypi.org/project/libusb-package/
@@ -128,11 +131,11 @@
 [coverage-badge]: https://img.shields.io/coverallsCoverage/github/ReflexCreations/Nexus
 [discord-badge]: https://img.shields.io/discord/738700768147669088?label=discord
 [docs-badge]: https://img.shields.io/readthedocs/reflex-nexus
 [license-badge]: https://img.shields.io/github/license/ReflexCreations/Nexus
 [lint-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/lint.yml?label=linting
 [linux-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-linux.yml?label=linux%20build
 [macos-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-macos.yml?label=macos%20build
-[pypi-badge]: https://img.shields.io/pypi/v/reflex_nexus
+[pypi-badge]: https://img.shields.io/pypi/v/reflex-nexus
 [tag-badge]: https://img.shields.io/github/v/tag/ReflexCreations/Nexus
 [test-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/test.yml?label=tests
 [windows-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-windows.yml?label=windows%20build
```

### Comparing `reflex_nexus-0.0.1/pyproject.toml` & `reflex_nexus-0.0.12/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 
 [metadata]
 title = "RE:Flex Nexus"
 copyright = "2023, Impulse Creations, Ltd"
 logo = "assets/favicon.ico"
 
 [tool.poetry]
-name = "reflex_nexus"
-version = "0.0.1"
+name = "reflex-nexus"
+version = "0.0.12"
 description = "RE:Flex Nexus - Universal Dance Pad Utilities"
 authors = ["Brittany Barrett <brittany.l.barrett@gmail.com>"]
+packages = [{include = "src"}]
 license = "MIT"
 readme = "README.md"
 homepage = "https://reflex.dance"
 repository = "https://github.com/ReflexCreations/Nexus"
 documentation = "https://reflex-nexus.readthedocs.io"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.10, <3.11"
 libusb_package = "*"
 PySide6 = "*"
 pyusb = "*"
 pyqtdarktheme = "*"
 QtAwesome = "*"
 
 [tool.poetry.group.docs.dependencies]
@@ -38,19 +39,19 @@
 pyinstaller = "*"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-cov = "*"
 
 [tool.poetry.scripts]
-app = "reflex_nexus:app"
-build = "reflex_nexus:build"
-docs = "reflex_nexus:docs"
-lint = "reflex_nexus:lint"
-test = "reflex_nexus:test"
+app = "nexus:app"
+build = "nexus:build"
+docs = "nexus:docs"
+lint = "nexus:lint"
+test = "nexus:test"
 
 [tool.ruff]
 line-length = 79
 ignore = ["ANN101", "D203", "D212"]
 select = [
     "ANN",  # flake8-annotations
     "B",    # flake8-bugbear
```

### Comparing `reflex_nexus-0.0.1/PKG-INFO` & `reflex_nexus-0.0.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: reflex-nexus
-Version: 0.0.1
+Version: 0.0.12
 Summary: RE:Flex Nexus - Universal Dance Pad Utilities
 Home-page: https://reflex.dance
 License: MIT
 Author: Brittany Barrett
 Author-email: brittany.l.barrett@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PySide6
 Requires-Dist: QtAwesome
 Requires-Dist: libusb_package
 Requires-Dist: pyqtdarktheme
 Requires-Dist: pyusb
 Project-URL: Documentation, https://reflex-nexus.readthedocs.io
 Project-URL: Repository, https://github.com/ReflexCreations/Nexus
@@ -24,14 +22,17 @@
 [![][linux-badge]][Releases] [![][macos-badge]][Releases]
 [![][windows-badge]][Releases] [![][pypi-badge]][pypi]
 [![][docs-badge]][Documentation] [![][lint-badge]][lint]
 [![][test-badge]][test] [![][coverage-badge]][coverage]
 [![][license-badge]][LICENSE] [![][tag-badge]][tag]
 [![][discord-badge]][discord]
 
+__Note: This is a work in progress project. References made in the readme__
+__and documentation are currently unfulfilled.__
+
 # RE:Flex Nexus - Universal Dance Pad Utilities
 
 RE:Flex Nexus aims to provide a comprehensive collection of PC software
 utilities for dance pads. The interface specification is flexible, allowing
 any dance pad to be quickly integrated and begin using available software
 features.
 
@@ -41,17 +42,17 @@
 will hopefully inspire creativity/freedom, while letting dance gamers share
 technology together.
 
 ## Installation
 
 - The latest executable can be found on the [Releases] page
 - Download the application for your respective operating system
-- Download the `nexus_resources.zip` package and extract to the location
+- Download the `nexus-resources.zip` package and extract to the location
 you would like to store program data
-- Open the `reflex_nexus` application
+- Open the `reflex-nexus` application
 - You will be prompted to set up your program data folder, enter the directory
 of the folder that you just extracted
 
 ## Usage
 
 For details on usage, check out the [Documentation].
 
@@ -119,15 +120,15 @@
 [coverage]: https://coveralls.io/github/ReflexCreations/Nexus
 [discord]: https://discord.gg/TCn3emnwZU
 [Documentation]: https://reflex-nexus.readthedocs.io/
 [Git]: https://git-scm.com/downloads/
 [LICENSE]: https://github.com/ReflexCreations/Nexus/LICENSE
 [lint]: https://github.com/ReflexCreations/Nexus/actions/workflows/lint.yml
 [Python]: https://python.org/downloads/
-[pypi]: https://pypi.org/project/reflex_nexus
+[pypi]: https://pypi.org/project/reflex-nexus
 [Releases]: https://github.com/ReflexCreations/Nexus/releases/
 [tag]: https://github.com/ReflexCreations/Nexus/tags
 [test]: https://github.com/ReflexCreations/Nexus/actions/workflows/test.yml
 
 <!--- Runtime dependency links -->
 
 [libusb-package]: https://pypi.org/project/libusb-package/
@@ -151,12 +152,12 @@
 [coverage-badge]: https://img.shields.io/coverallsCoverage/github/ReflexCreations/Nexus
 [discord-badge]: https://img.shields.io/discord/738700768147669088?label=discord
 [docs-badge]: https://img.shields.io/readthedocs/reflex-nexus
 [license-badge]: https://img.shields.io/github/license/ReflexCreations/Nexus
 [lint-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/lint.yml?label=linting
 [linux-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-linux.yml?label=linux%20build
 [macos-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-macos.yml?label=macos%20build
-[pypi-badge]: https://img.shields.io/pypi/v/reflex_nexus
+[pypi-badge]: https://img.shields.io/pypi/v/reflex-nexus
 [tag-badge]: https://img.shields.io/github/v/tag/ReflexCreations/Nexus
 [test-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/test.yml?label=tests
 [windows-badge]: https://img.shields.io/github/actions/workflow/status/ReflexCreations/Nexus/build-windows.yml?label=windows%20build
```

