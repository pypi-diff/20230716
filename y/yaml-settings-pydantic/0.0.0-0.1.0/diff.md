# Comparing `tmp/yaml-settings-pydantic-0.0.0.tar.gz` & `tmp/yaml-settings-pydantic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-settings-pydantic-0.0.0.tar", last modified: Tue Dec 20 17:31:38 2022, max compression
+gzip compressed data, was "yaml-settings-pydantic-0.1.0.tar", last modified: Sat Jul 15 23:41:44 2023, max compression
```

## Comparing `yaml-settings-pydantic-0.0.0.tar` & `yaml-settings-pydantic-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2022-12-20 17:31:38.930230 yaml-settings-pydantic-0.0.0/
--rw-r--r--   0 dev       (1000) dev       (1000)     5230 2022-12-20 17:31:38.930230 yaml-settings-pydantic-0.0.0/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)     3918 2022-12-20 17:25:15.000000 yaml-settings-pydantic-0.0.0/README.rst
--rw-r--r--   0 dev       (1000) dev       (1000)     2765 2022-12-20 17:31:25.000000 yaml-settings-pydantic-0.0.0/pyproject.toml
--rw-r--r--   0 dev       (1000) dev       (1000)      421 2022-12-20 17:31:38.930230 yaml-settings-pydantic-0.0.0/setup.cfg
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2022-12-20 17:31:38.930230 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic/
--rw-r--r--   0 dev       (1000) dev       (1000)     6727 2022-12-20 17:00:00.000000 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic/__init__.py
-drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2022-12-20 17:31:38.930230 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic.egg-info/
--rw-r--r--   0 dev       (1000) dev       (1000)     5230 2022-12-20 17:31:38.000000 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) dev       (1000)      299 2022-12-20 17:31:38.000000 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) dev       (1000)        1 2022-12-20 17:31:38.000000 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       80 2022-12-20 17:31:38.000000 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) dev       (1000)       23 2022-12-20 17:31:38.000000 yaml-settings-pydantic-0.0.0/yaml_settings_pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-07-15 23:41:44.845814 yaml-settings-pydantic-0.1.0/
+-rw-r--r--   0 dev       (1000) dev       (1000)     1311 2023-07-15 23:41:44.845814 yaml-settings-pydantic-0.1.0/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3632 2023-07-15 23:14:54.000000 yaml-settings-pydantic-0.1.0/README.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2754 2023-07-15 23:41:17.000000 yaml-settings-pydantic-0.1.0/pyproject.toml
+-rw-rw-r--   0 dev       (1000) dev       (1000)      421 2023-07-15 23:41:44.845814 yaml-settings-pydantic-0.1.0/setup.cfg
+drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-07-15 23:41:44.845814 yaml-settings-pydantic-0.1.0/tests/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     7010 2023-07-15 22:45:37.000000 yaml-settings-pydantic-0.1.0/tests/test_everything.py
+drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-07-15 23:41:44.845814 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     6706 2023-07-15 23:38:57.000000 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic/__init__.py
+drwxr-xr-x   0 dev       (1000) dev       (1000)        0 2023-07-15 23:41:44.845814 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic.egg-info/
+-rw-r--r--   0 dev       (1000) dev       (1000)     1311 2023-07-15 23:41:44.000000 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) dev       (1000)      324 2023-07-15 23:41:44.000000 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)        1 2023-07-15 23:41:44.000000 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       90 2023-07-15 23:41:44.000000 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) dev       (1000)       23 2023-07-15 23:41:44.000000 yaml-settings-pydantic-0.1.0/yaml_settings_pydantic.egg-info/top_level.txt
```

### Comparing `yaml-settings-pydantic-0.0.0/README.rst` & `yaml-settings-pydantic-0.1.0/README.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 Why Should I Use This?
 ================================================================
 
-This project is very helpful for projects that have large 
+This project is very helpful for projects that have large
 configuration files, nested configuration files, or if you
 just don't like writing large ``.env`` files. It is also worth
 noting that due to the backwards compatability between ``YAML``
 and ``JSON`` that this will also parse ``JSON`` configuration.
 
-For instance, the following settings 
-
-..
-  .. literal_include:: ./examples/__init__.py
-
-  could parse the following ``YAML`` :
-
-  .. literal_include:: ./examples/example.yaml
-
-  or equivelently the less readable ``env`` file:
-
-  .. literal_include:: ./tests/example.env
-
-
-This can also be helpful when writing out (variables for ) helm 
-charts, pipelines of various sorts, and other ``YAML`` assets. 
-In such a context, it may be necessary to write an ``ENV`` file 
+This can also be helpful when writing out (variables for ) helm
+charts, pipelines of various sorts, and other ``YAML`` assets.
+In such a context, it may be necessary to write an ``ENV`` file
 in line with your continuous integration or deployment variables.
 However, this can be rather cumbersome due to escape sequences:
 
 .. code:: yaml
-
   # Example pipeline with env settings
   # The configuration built is compatable with ``./examples/__init__.py``
 
   ...
   pipelines:
     default:
       - step:
@@ -49,15 +34,15 @@
               }"
             - echo "MYFISTSETTING=$MYFISTSETTING" > .env
             - echo "MYDATABASESETTINGS=$MYDATABASESETTINGS" >> .env
           artifacts:
             - .env
 
 
-The script section of the above bitbucket pipeline may be 
+The script section of the above bitbucket pipeline may be
 replaced with something less horible to edit:
 
 .. code:: yaml
 
   ...
   script:
     - |
@@ -67,20 +52,20 @@
           host: localhost
           port: 27017
           username: some
           password: dude
       }"
     - echo $ENVYAMLCONTENT > .env
   ...
-  
 
-this may not make the strongest case due to the brevity of the 
+
+this may not make the strongest case due to the brevity of the
 settings themselves. But when the settings are many layers deep,
 it is clear that writing ``YAML`` is preferable.
-  
+
 
 Examples, Usage, and Installation
 ================================================================
 
 Install using ``pip``:
 
 .. code:: bash
@@ -129,20 +114,19 @@
 
 Finally it is useful to note that ``create_settings_yaml`` can accept
 multiple files as input (all such inputs must deserialize to ``dict``)
 and reload them on every call of ``env_settings_yaml`` or just on the
 origonal call using the ``reload`` parameter:
 
 .. code:: python
-
   ...
   env_settings_yaml = create_settings_yaml(
     "./path/to/yaml_1.yaml",
     "./path/to_my.yaml",
     reload = True
   )
   ...
 
-In this instance the values from ``./path/to_my.yaml`` will take 
+In this instance the values from ``./path/to_my.yaml`` will take
 precedence over the ``YAML`` provided earlier. That is, the
 later in the input list the path appears, the more its variables
 are prefered.
```

### Comparing `yaml-settings-pydantic-0.0.0/pyproject.toml` & `yaml-settings-pydantic-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 build-backend = "setuptools.build_meta"
 
 [black]
 
 [project]
 authors = [{name = "Adrian Cederberg", email = "adrn.cederberg123@gmail.com"}, ]
 name = "yaml-settings-pydantic"
-version = "0.0.0"
+version = "0.1.0"
 description = "A tool to easily load (many) JSON/YAML files as pydantic settings."
 readme = "README.rst"
 keywords = ["env", "config", "pydantic", "settings", "pydantic-settings", "yaml", "json", "yaml-settings-pydantic"]
 #liscense = "Lisense :: OSI Approved :: MIT License"
 
 # The following were take directly from pyproject.toml in pydantic because I am lazy and the classifiers
 # are applicable here.
 classifiers = [
-    #'Development Status :: 1',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
@@ -37,28 +36,28 @@
     'Environment :: Console',
     'Environment :: MacOS X',
     'Framework :: Hypothesis',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 dependencies = [
-	"pydantic",
+	"pydantic>=1.9.1, <2",
 	"pyyaml",
 ]
 requires-python = ">=3.7" # because https://github.com/pydantic/pydantic/blob/main/pyproject.toml
 
 
 [project.optional-dependencies]
 ci = [
   "build",
   "twine",
 ]
 dev = [
-	"black", 
-	"flake8", 
+	"black",
+	"flake8",
 	"mypy",
 	"isort"
 ]
 test = [
 	"pytest",
 ]
 
@@ -85,18 +84,18 @@
 [tool.isort]
 
 
 [tool.mypy]
 
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "0.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"src/reader/__init__.py" = ["{version}"]
+"yaml_settings_pydantic/__init__.py" = ["{version}"]
```

### Comparing `yaml-settings-pydantic-0.0.0/yaml_settings_pydantic/__init__.py` & `yaml-settings-pydantic-0.1.0/yaml_settings_pydantic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from os import path
-from typing import (Any, Callable, Dict, Iterable, Iterator, List, Optional,
-                    Tuple, Union)
+from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 
 from pydantic import validate_arguments
 from pydantic.env_settings import BaseSettings, SettingsSourceCallable
 from yaml import safe_load
 
+__version__ = "0.1.0"
+
 
 class PydanticSettingsYamlError(Exception):
     ...
 
 
 def __recursive_merge(
     to_combine: Optional[Dict],
@@ -42,15 +43,14 @@
     out: Dict = {}
     _ = all(__recursive_merge(item, out) is None for item in items)
     return out
 
 
 @validate_arguments
 def _load_many(*filepaths: str) -> Dict[str, Any]:
-
     bad = tuple(fp for fp in filepaths if not path.isfile(fp))
     if bad:
         raise ValueError(f"The following paths are not files: ``{bad}``.")
 
     files = {filepath: open(filepath) for filepath in filepaths}
     loaded_files: Dict[str, Dict] = {
         file_name: safe_load(file) for file_name, file in files.items()
@@ -114,31 +114,30 @@
     """
 
     n = len(filepaths)
     if n == 0:
         raise ValueError("Atleast one file is required.")
 
     if not reload:
-
         loaded = yaml_loadmanyandvalidate(*filepaths)
 
         def yaml_settings(settings: Optional[SettingsSourceCallable]) -> Dict:
             """Yaml settings loader for a single file."""
             return loaded
 
         return yaml_settings
 
     def yaml_settings_reload(settings: Optional[SettingsSourceCallable]) -> Dict:
         """Yaml settings loader for many files."""
         return yaml_loadmanyandvalidate(*filepaths)
 
     return yaml_settings_reload
 
-class BaseYamlSettingsConfig:
 
+class BaseYamlSettingsConfig:
     # Use reload to determine if create_yaml_settings will
     # load and parse the provided files every time it is
     # called.
     env_yaml_settings_files: Tuple[str, ...]
     env_yaml_settings: SettingsSourceCallable
     env_yaml_settings_ignore_env_file: bool = True
     env_yaml_settings_reload: bool = True
@@ -173,15 +172,14 @@
     @classmethod
     def customise_sources(
         cls,
         init_settings: SettingsSourceCallable,
         env_settings: SettingsSourceCallable,
         file_secret_settings: SettingsSourceCallable,
     ):
-
         attrs = {
             f"env_yaml_settings{s}": getattr(cls, f"env_yaml_settings{s}", None)
             for s in (
                 "_files",
                 "",
                 "_ignore_env_file",
                 "_reload",
@@ -203,14 +201,9 @@
         )
         return (
             callables
             if attrs["env_yaml_settings_ignore_env_file"]
             else (*callables, env_settings)
         )
 
-__all__ = ( 
-    "yaml_loadmanyandvalidate", 
-    "create_yaml_settings", 
-    "BaseYamlSettingsConfig" 
-)
-
 
+__all__ = ("yaml_loadmanyandvalidate", "create_yaml_settings", "BaseYamlSettingsConfig")
```

