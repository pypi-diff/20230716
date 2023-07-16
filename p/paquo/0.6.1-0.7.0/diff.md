# Comparing `tmp/paquo-0.6.1.tar.gz` & `tmp/paquo-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paquo-0.6.1.tar", last modified: Wed Mar  1 22:14:19 2023, max compression
+gzip compressed data, was "paquo-0.7.0.tar", last modified: Sun Jul 16 19:25:50 2023, max compression
```

## Comparing `paquo-0.6.1.tar` & `paquo-0.7.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.043298 paquo-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-01 22:14:13.000000 paquo-0.6.1/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-01 22:14:13.000000 paquo-0.6.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-01 22:14:13.000000 paquo-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-01 22:14:13.000000 paquo-0.6.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-01 22:14:13.000000 paquo-0.6.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-01 22:14:13.000000 paquo-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-01 22:14:13.000000 paquo-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-01 22:14:13.000000 paquo-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-03-01 22:14:19.043298 paquo-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-03-01 22:14:13.000000 paquo-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.035298 paquo-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.035298 paquo-0.6.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.035298 paquo-0.6.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   308228 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/_static/screenshot_example_05.png
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-03-01 22:14:13.000000 paquo-0.6.1/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-01 22:14:13.000000 paquo-0.6.1/environment.devenv.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.039298 paquo-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/example_01_read_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/example_02_add_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/example_03_project_with_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/example_04_project_with_image_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/example_05_draw_tiles_on_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-01 22:14:13.000000 paquo-0.6.1/examples/prepare_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.039298 paquo-0.6.1/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-01 22:14:13.000000 paquo-0.6.1/extras/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.039298 paquo-0.6.1/extras/osx_app_shim/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-01 22:14:13.000000 paquo-0.6.1/extras/osx_app_shim/PaquoOpenQpZip.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-01 22:14:13.000000 paquo-0.6.1/extras/osx_app_shim/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.039298 paquo-0.6.1/paquo/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/.paquo.defaults.toml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-01 22:14:18.000000 paquo-0.6.1/paquo/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    25066 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/java.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/jpype_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/pathobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.043298 paquo-0.6.1/paquo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_jpype_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_pathobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_readonly.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-01 22:14:13.000000 paquo-0.6.1/paquo/tests/test_repr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 22:14:19.043298 paquo-0.6.1/paquo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-03-01 22:14:18.000000 paquo-0.6.1/paquo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-01 22:14:19.000000 paquo-0.6.1/paquo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 22:14:18.000000 paquo-0.6.1/paquo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-01 22:14:18.000000 paquo-0.6.1/paquo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-01 22:14:18.000000 paquo-0.6.1/paquo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-01 22:14:18.000000 paquo-0.6.1/paquo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-01 22:14:13.000000 paquo-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-01 22:14:19.043298 paquo-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-16 19:25:43.000000 paquo-0.7.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-16 19:25:43.000000 paquo-0.7.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 19:25:43.000000 paquo-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-16 19:25:43.000000 paquo-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 19:25:43.000000 paquo-0.7.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-16 19:25:43.000000 paquo-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 19:25:43.000000 paquo-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-16 19:25:43.000000 paquo-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-16 19:25:50.647502 paquo-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-16 19:25:43.000000 paquo-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.639502 paquo-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   308228 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/_static/screenshot_example_05.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-16 19:25:43.000000 paquo-0.7.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-16 19:25:43.000000 paquo-0.7.0/environment.devenv.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_01_read_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_02_add_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_03_project_with_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_04_project_with_image_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/example_05_draw_tiles_on_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-16 19:25:43.000000 paquo-0.7.0/examples/prepare_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-16 19:25:43.000000 paquo-0.7.0/extras/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.643502 paquo-0.7.0/extras/osx_app_shim/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-16 19:25:43.000000 paquo-0.7.0/extras/osx_app_shim/PaquoOpenQpZip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-16 19:25:43.000000 paquo-0.7.0/extras/osx_app_shim/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/paquo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/.paquo.defaults.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25808 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/jpype_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/pathobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/paquo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_jpype_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_pathobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_readonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-16 19:25:43.000000 paquo-0.7.0/paquo/tests/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:25:50.647502 paquo-0.7.0/paquo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 19:25:50.000000 paquo-0.7.0/paquo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-16 19:25:43.000000 paquo-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-16 19:25:50.651502 paquo-0.7.0/setup.cfg
```

### Comparing `paquo-0.6.1/.pre-commit-config.yaml` & `paquo-0.7.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-added-large-files
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.9.0
   hooks:
   - id: pyupgrade
-    args: [--py37-plus]
+    args: [--py38-plus]
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
     exclude: ^examples|^extras|^docs|tests.*|setup.py
 # - repo: https://github.com/psf/black
 #   rev: 22.6.0
 #   hooks:
 #   - id: black
 #     language_version: python3
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: 'v1.0.0'
+  rev: 'v1.4.1'
   hooks:
   - id: mypy
     exclude: ^examples|^extras|^docs|tests.*
     additional_dependencies: [packaging, ome-types]
 - repo: https://github.com/PyCQA/flake8
   rev: '6.0.0'
   hooks:
   - id: flake8
     additional_dependencies:
     - flake8-typing-imports==1.12.0
     language_version: python3
     exclude: "^(build|docs|examples|extras|setup.py)|tests[/]"
 - repo: https://github.com/PyCQA/bandit
-  rev: '1.7.4'
+  rev: '1.7.5'
   hooks:
   - id: bandit
     args: ["-lll", "--ini", ".bandit"]
```

### Comparing `paquo-0.6.1/CHANGELOG.md` & `paquo-0.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,24 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
 ...
 
+## [0.7.0] - 2023-06-16
+### Changed
+- drop Python=3.7 support
+
+### Added
+- paquo: support for newer ome-types
+
+### Fixed
+- paquo: fixed deprecation warnings on py311
+
 ## [0.6.1] - 2023-03-01
 ### Fixed
 - paquo: fix saving manually updated measurements
 - paquo: prevent deprecation warnings with QuPath>=0.4.0
 - paquo: prevent deprecation warnings with shapely>=2
 
 ## [0.6.0] - 2022-11-21
@@ -127,15 +137,16 @@
 - `QuPathProject.add_image` is now calling `QuPathProject.save`
 
 ## [0.1.0] - 2020-08-12
 ### Added
 - initial release of paquo
 
 
-[Unreleased]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.1...HEAD
+[Unreleased]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.7.0...HEAD
+[0.7.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.1...v0.7.0
 [0.6.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.6.0...v0.6.1
 [0.6.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.2...v0.5.0
 [0.4.2]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.1...v0.4.2
 [0.4.1]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.4.0...v0.4.1
 [0.4.0]: https://github.com/bayer-science-for-a-better-life/paquo/compare/v0.3.1...v0.4.0
```

### Comparing `paquo-0.6.1/CONTRIBUTING.md` & `paquo-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/LICENSE` & `paquo-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/PKG-INFO` & `paquo-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: paquo
-Version: 0.6.1
+Version: 0.7.0
 Summary: library for interacting with QuPath
 Home-page: https://github.com/bayer-science-for-a-better-life/paquo
 Download-URL: https://github.com/bayer-science-for-a-better-life/paquo
 Author: Santiago Villalba, Andreas Poehlmann
 Author-email: santiago.villalba@bayer.com, andreas.poehlmann@bayer.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Java
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ome
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # PAQUO: PAthological QUpath Obsession
```

### Comparing `paquo-0.6.1/README.md` & `paquo-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/Makefile` & `paquo-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/_static/screenshot_example_05.png` & `paquo-0.7.0/docs/source/_static/screenshot_example_05.png`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/api.rst` & `paquo-0.7.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/conf.py` & `paquo-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/configuration.rst` & `paquo-0.7.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/index.rst` & `paquo-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/installation.rst` & `paquo-0.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/docs/source/quickstart.rst` & `paquo-0.7.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/environment.devenv.yml` & `paquo-0.7.0/environment.devenv.yml`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/README.md` & `paquo-0.7.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/example_01_read_annotations.py` & `paquo-0.7.0/examples/example_01_read_annotations.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/example_02_add_annotations.py` & `paquo-0.7.0/examples/example_02_add_annotations.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/example_03_project_with_classes.py` & `paquo-0.7.0/examples/example_03_project_with_classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/example_04_project_with_image_metadata.py` & `paquo-0.7.0/examples/example_04_project_with_image_metadata.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/example_05_draw_tiles_on_image.py` & `paquo-0.7.0/examples/example_05_draw_tiles_on_image.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/examples/prepare_resources.py` & `paquo-0.7.0/examples/prepare_resources.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/extras/README.md` & `paquo-0.7.0/extras/README.md`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/.paquo.defaults.toml` & `paquo-0.7.0/paquo/.paquo.defaults.toml`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/__main__.py` & `paquo-0.7.0/paquo/__main__.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/_cli.py` & `paquo-0.7.0/paquo/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,21 @@
     print("# ===========================")
     print("# format: TOML")
     print(to_toml(settings))
 
 
 def config_print_defaults():
     """print the default paquo configuration"""
-    from importlib.resources import read_text
+    if sys.version_info >= (3, 9):
+        from importlib.resources import files
+
+        def read_text(package, resource, encoding):
+            return files(package).joinpath(resource).read_text(encoding=encoding)
+    else:
+        from importlib.resources import read_text
 
     from paquo._config import settings
 
     output = read_text(
         "paquo",
         ".paquo.defaults.toml",
         encoding=settings.ENCODING_FOR_DYNACONF
```

### Comparing `paquo-0.6.1/paquo/_config.py` & `paquo-0.7.0/paquo/_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,32 @@
+import sys
 import tempfile
-from importlib.resources import path as importlib_resources_path
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 
 from dynaconf import Dynaconf
 from dynaconf import Validator
 from dynaconf import loaders
 from dynaconf.base import Settings
 from dynaconf.utils import files as _files
 from dynaconf.utils.boxing import DynaBox
 
+if sys.version_info >= (3, 9):
+    from importlib.resources import as_file
+    from importlib.resources import files
+
+    def importlib_resources_path(package, resource):
+        return as_file(files(package).joinpath(resource))
+
+else:
+    from importlib.resources import path as importlib_resources_path
+
+
 PAQUO_CONFIG_FILENAME = '.paquo.toml'
 
 _PAQUO_FIX_CONFIG_KEYS = {
     # recover prefixed keys due to dynaconf weirdness
     "_qupath_dir",
     "_qupath_search_dirs",
     "_qupath_search_dir_regex",
```

### Comparing `paquo-0.6.1/paquo/_logging.py` & `paquo-0.7.0/paquo/_logging.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/_repr.py` & `paquo-0.7.0/paquo/_repr.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/_utils.py` & `paquo-0.7.0/paquo/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import subprocess
 import sys
 import tarfile
 import tempfile
 import warnings
 import zipfile
 from datetime import datetime
+from functools import cached_property as _cached_property
 from functools import partial
 from functools import total_ordering
 from pathlib import Path
 from urllib.parse import urlsplit
 from urllib.request import urlopen
 from warnings import warn
 
@@ -25,45 +26,18 @@
     'QuPathVersion',
     'cached_property',
     'make_backup_filename',
     'load_json_from_path'
 ]
 
 
-if sys.version_info >= (3, 8):
-    from functools import cached_property as _cached_property
-
-    # noinspection PyPep8Naming
-    class cached_property(_cached_property):
-        def __set__(self, obj, value):
-            raise AttributeError(f"readonly attribute {self.attrname}")
-else:
-    # noinspection PyPep8Naming
-    class cached_property:
-        _NOCACHE = object()
-
-        def __init__(self, fget):
-            self.fget = fget
-            self.attrname = None
-            self.__doc__ = fget.__doc__
-
-        def __set_name__(self, owner, name):
-            self.attrname = name
-
-        def __get__(self, obj, objtype=None):
-            if obj is None:
-                return self  # pragma: no cover
-            cache = obj.__dict__
-            val = cache.get(self.attrname, self._NOCACHE)
-            if val is self._NOCACHE:
-                val = cache[self.attrname] = self.fget(obj)
-            return val
-
-        def __set__(self, obj, value):
-            raise AttributeError(f"readonly attribute {self.fget.__name__}")
+# noinspection PyPep8Naming
+class cached_property(_cached_property):
+    def __set__(self, obj, value):
+        raise AttributeError(f"readonly attribute {self.attrname}")
 
 
 @total_ordering
 class QuPathVersion:
     """Handle the QuPath version strings"""
     def __init__(self, version: str) -> None:
         self.origin = ver_str = str(version).strip()
@@ -220,15 +194,15 @@
         return qp_dst
 
     if system == "Linux":
         if not os.fspath(file).endswith(".tar.xz"):
             raise ValueError("file does not end with `.tar.xz`")
         with tempfile.TemporaryDirectory() as tmp_dir:
             with tarfile.open(file, mode="r:xz") as tf:
-                tf.extractall(tmp_dir)
+                tf.extractall(tmp_dir)  # nosec: B202
                 for name in os.listdir(tmp_dir):
                     pth = os.path.join(tmp_dir, name)
                     if name.startswith("QuPath") and os.path.isdir(pth):
                         break
                 else:
                     raise RuntimeError("no qupath extracted?")
             shutil.move(os.path.join(tmp_dir, name), qp_dst)
@@ -253,15 +227,15 @@
 
     elif system == "Windows":
         if not Path(file).suffix == ".zip":
             raise ValueError("file does not end with `.zip`")
 
         with tempfile.TemporaryDirectory() as tmp_dir:
             with zipfile.ZipFile(file, mode="r") as zf:
-                zf.extractall(tmp_dir)
+                zf.extractall(tmp_dir)  # nosec: B202
                 for name in os.listdir(tmp_dir):
                     pth = os.path.join(tmp_dir, name)
                     if name.startswith("QuPath") and os.path.isdir(pth):
                         break
                 else:
                     raise RuntimeError("no qupath extracted?")
             shutil.move(os.path.join(tmp_dir, name), qp_dst)
```

### Comparing `paquo-0.6.1/paquo/classes.py` & `paquo-0.7.0/paquo/classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/colors.py` & `paquo-0.7.0/paquo/colors.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/hierarchy.py` & `paquo-0.7.0/paquo/hierarchy.py`

 * *Files 2% similar despite different names*

```diff
@@ -505,18 +505,34 @@
             }
             if class_name:
                 _m[f"{prefix}:path_class"] = class_name
             if ao.name:
                 _m[f"{prefix}:name"] = ao.name
             for k, v in ao.measurements.items():
                 _m[f"{prefix}:measurement:{k}"] = v
-            map_annotation = MapAnnotation(value=Map(m=[
-                M(k=_key, value=str(_value))
-                for _key, _value in _m.items()
-            ]))
+
+            if "ms" in Map.__fields__:
+                map_annotation = MapAnnotation(  # type: ignore
+                    value=Map(
+                        ms=[
+                            M(k=_key, value=str(_value))
+                            for _key, _value in _m.items()
+                        ]
+                    )
+                )
+            else:
+                # ome-types < 0.4.0
+                map_annotation = MapAnnotation(  # type: ignore
+                    value=Map(
+                        m=[
+                            M(k=_key, value=str(_value))
+                            for _key, _value in _m.items()
+                        ]
+                    )
+                )
 
             # --- prepare common kwargs for ome Shape
 
             if ao.path_class and ao.path_class.color:
                 # https://www.openmicroscopy.org/Schemas/Documentation/Generated/OME-2016-06/ome_xsd.html#Color
                 r, g, b, a = ao.path_class.color.to_rgba()
                 stroke_color, = struct.unpack(">i", bytes([r, g, b, a]))
@@ -555,16 +571,20 @@
                 the_t=the_t,
                 the_z=the_z,
                 transform=None,
             )
 
             # --- create the roi
 
-            roi = ROI(name=class_name)
-            roi.annotation_ref.append(AnnotationRef(id=map_annotation.id))
+            roi = ROI(name=class_name)  # type: ignore
+            try:
+                roi.annotation_refs.append(AnnotationRef(id=map_annotation.id))  # type: ignore
+            except AttributeError:
+                # ome-types<0.4.0
+                roi.annotation_ref.append(AnnotationRef(id=map_annotation.id))
 
             # --- add the correct shape dependent on roi types
 
             ome_shape: Any
             if isinstance(qp_roi, (PolygonROI, GeometryROI)):
                 ome_shape = OmePolygon(
                     points=" ".join(f"{p.getX():f},{p.getY():f}" for p in qp_roi.getAllPoints()),
```

### Comparing `paquo-0.6.1/paquo/images.py` & `paquo-0.7.0/paquo/images.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/java.py` & `paquo-0.7.0/paquo/java.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/jpype_backend.py` & `paquo-0.7.0/paquo/jpype_backend.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/pathobjects.py` & `paquo-0.7.0/paquo/pathobjects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/projects.py` & `paquo-0.7.0/paquo/projects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import collections.abc as collections_abc
 import math
 import pathlib
 import re
 import shutil
-import sys
 from contextlib import contextmanager
 from contextlib import nullcontext
 from typing import Any
 from typing import Callable
 from typing import ContextManager
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
+from typing import Literal
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 from typing import overload
-from urllib.parse import urlsplit
-
-if sys.version_info >= (3, 8):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
 
 from paquo import settings
 from paquo._logging import get_logger
 from paquo._logging import redirect
 from paquo._utils import make_backup_filename
 from paquo.classes import QuPathPathClass
 from paquo.images import ImageProvider
```

### Comparing `paquo-0.6.1/paquo/tests/conftest.py` & `paquo-0.7.0/paquo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_classes.py` & `paquo-0.7.0/paquo/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_colors.py` & `paquo-0.7.0/paquo/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_config.py` & `paquo-0.7.0/paquo/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_hierarchy.py` & `paquo-0.7.0/paquo/tests/test_hierarchy.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,7 +384,15 @@
     with pytest.raises(TypeError):
         # noinspection PyTypeChecker
         empty_hierarchy.annotations.add("abc")
 
     with pytest.raises(TypeError):
         # noinspection PyTypeChecker
         empty_hierarchy.annotations.discard("abc")
+
+
+def test_serialize_to_ome(project_with_annotations):
+    pytest.importorskip("ome_types")
+    xml = project_with_annotations.images[0].hierarchy.to_ome_xml()
+
+    assert xml.startswith("<OME")
+    assert xml.strip().endswith("</OME>")
```

### Comparing `paquo-0.6.1/paquo/tests/test_images.py` & `paquo-0.7.0/paquo/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_jpype_backend.py` & `paquo-0.7.0/paquo/tests/test_jpype_backend.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_main.py` & `paquo-0.7.0/paquo/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_pathobjects.py` & `paquo-0.7.0/paquo/tests/test_pathobjects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_projects.py` & `paquo-0.7.0/paquo/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_readonly.py` & `paquo-0.7.0/paquo/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo/tests/test_repr.py` & `paquo-0.7.0/paquo/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/paquo.egg-info/PKG-INFO` & `paquo-0.7.0/paquo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: paquo
-Version: 0.6.1
+Version: 0.7.0
 Summary: library for interacting with QuPath
 Home-page: https://github.com/bayer-science-for-a-better-life/paquo
 Download-URL: https://github.com/bayer-science-for-a-better-life/paquo
 Author: Santiago Villalba, Andreas Poehlmann
 Author-email: santiago.villalba@bayer.com, andreas.poehlmann@bayer.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Java
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: ome
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # PAQUO: PAthological QUpath Obsession
```

### Comparing `paquo-0.6.1/paquo.egg-info/SOURCES.txt` & `paquo-0.7.0/paquo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/pyproject.toml` & `paquo-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `paquo-0.6.1/setup.cfg` & `paquo-0.7.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Programming Language :: Java
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Visualization
 	Topic :: Scientific/Engineering :: Information Analysis
@@ -29,21 +28,20 @@
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Operating System :: Unix
 	Operating System :: MacOS
 
 [options]
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	dynaconf>=3,!=3.1.0
 	JPype1>=1.0.1
 	shapely
 	packaging
-	typing_extensions; python_version < '3.8'
 
 [options.packages.find]
 exclude = 
 	*.tests
 
 [options.package_data]
 paquo = 
@@ -65,15 +63,16 @@
 	sphinx-autodoc-typehints
 
 [options.entry_points]
 console_scripts = 
 	paquo = paquo.__main__:main
 
 [mypy]
-python_version = 3.7
+python_version = 3.8
+plugins = pydantic.mypy
 warn_return_any = True
 warn_unused_configs = True
 exclude = ^examples|^extras|^docs|tests.*
 
 [mypy-jpype.*]
 ignore_missing_imports = True
```

