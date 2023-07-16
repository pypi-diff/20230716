# Comparing `tmp/cf_xarray-0.8.3.tar.gz` & `tmp/cf_xarray-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_xarray-0.8.3.tar", last modified: Thu Jul  6 04:01:59 2023, max compression
+gzip compressed data, was "cf_xarray-0.8.4.tar", last modified: Sun Jul 16 16:04:34 2023, max compression
```

## Comparing `cf_xarray-0.8.3.tar` & `cf_xarray-0.8.4.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.448005 cf_xarray-0.8.3/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.448005 cf_xarray-0.8.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.448005 cf_xarray-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/.tributors
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 04:01:58.000000 cf_xarray-0.8.3/cf_xarray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   100886 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    23849 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/scripts/make_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/scripts/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/sgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63717 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/cf_xarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/cf_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 04:01:59.000000 cf_xarray-0.8.3/cf_xarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.452005 cf_xarray-0.8.3/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/environment-no-optional-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/ci/upstream-dev-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/2D_bounds_averaged.png
--rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/2D_bounds_error.png
--rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/2D_bounds_nonunique.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/dataset-diagram-logo.tex
--rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/full-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/rich-repr-example.png
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/bounds.md
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/cartopy_rotated_pole.png
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/coding.md
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/coord_axes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/custom-criteria.md
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/dsg.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/flags.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/geometry.md
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/grid_mappings.md
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/howtouse.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/parametricz.md
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/plotting.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/provenance.md
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/selecting.md
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/sgrid_ugrid.md
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/units.md
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/doc/whats-new.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-06 04:01:27.000000 cf_xarray-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:01:59.460006 cf_xarray-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.582867 cf_xarray-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.554865 cf_xarray-0.8.4/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.554865 cf_xarray-0.8.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.554865 cf_xarray-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.github/workflows/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/.tributors
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-07-16 16:04:34.578867 cf_xarray-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.558865 cf_xarray-0.8.4/cf_xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 16:04:34.000000 cf_xarray-0.8.4/cf_xarray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101014 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23849 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.562865 cf_xarray-0.8.4/cf_xarray/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/scripts/make_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/scripts/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/sgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.566866 cf_xarray-0.8.4/cf_xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64097 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/cf_xarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.562865 cf_xarray-0.8.4/cf_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-07-16 16:04:34.000000 cf_xarray-0.8.4/cf_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-16 16:04:34.000000 cf_xarray-0.8.4/cf_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:04:34.000000 cf_xarray-0.8.4/cf_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 16:04:34.000000 cf_xarray-0.8.4/cf_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 16:04:34.000000 cf_xarray-0.8.4/cf_xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.566866 cf_xarray-0.8.4/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/ci/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/ci/environment-no-optional-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/ci/upstream-dev-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.578867 cf_xarray-0.8.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/2D_bounds_averaged.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/2D_bounds_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/2D_bounds_nonunique.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.578867 cf_xarray-0.8.4/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/_static/dataset-diagram-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/_static/full-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/_static/rich-repr-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/bounds.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/cartopy_rotated_pole.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/coding.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/coord_axes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/custom-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/dsg.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:04:34.578867 cf_xarray-0.8.4/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/flags.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/geometry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/grid_mappings.md
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/howtouse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/parametricz.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/provenance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/selecting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/sgrid_ugrid.md
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/units.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/doc/whats-new.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-16 16:04:02.000000 cf_xarray-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:04:34.582867 cf_xarray-0.8.4/setup.cfg
```

### Comparing `cf_xarray-0.8.3/.github/workflows/ci.yaml` & `cf_xarray-0.8.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.github/workflows/parse_logs.py` & `cf_xarray-0.8.4/.github/workflows/parse_logs.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.github/workflows/pypi.yaml` & `cf_xarray-0.8.4/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.github/workflows/testpypi-release.yaml` & `cf_xarray-0.8.4/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.github/workflows/upstream-dev-ci.yaml` & `cf_xarray-0.8.4/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.gitignore` & `cf_xarray-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.pre-commit-config.yaml` & `cf_xarray-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/.tributors` & `cf_xarray-0.8.4/.tributors`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/CITATION.cff` & `cf_xarray-0.8.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/LICENSE` & `cf_xarray-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/PKG-INFO` & `cf_xarray-0.8.4/cf_xarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cf_xarray
-Version: 0.8.3
+Name: cf-xarray
+Version: 0.8.4
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.3/README.rst` & `cf_xarray-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/accessor.py` & `cf_xarray-0.8.4/cf_xarray/accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2733,15 +2733,19 @@
         da = self._obj
 
         attrs_or_encoding = ChainMap(da.attrs, da.encoding)
         grid_mapping = attrs_or_encoding.get("grid_mapping", None)
         if not grid_mapping:
             raise ValueError("No 'grid_mapping' attribute present.")
 
+        if grid_mapping not in da._coords:
+            raise ValueError(f"Grid Mapping variable {grid_mapping} not present.")
+
         grid_mapping_var = da[grid_mapping]
+
         return grid_mapping_var.attrs["grid_mapping_name"]
 
     def __getitem__(self, key: Hashable | Iterable[Hashable]) -> DataArray:
         """
         Index into a DataArray making use of CF attributes.
 
         Parameters
```

### Comparing `cf_xarray-0.8.3/cf_xarray/coding.py` & `cf_xarray-0.8.4/cf_xarray/coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/criteria.py` & `cf_xarray-0.8.4/cf_xarray/criteria.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/datasets.py` & `cf_xarray-0.8.4/cf_xarray/datasets.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/formatting.py` & `cf_xarray-0.8.4/cf_xarray/formatting.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/geometry.py` & `cf_xarray-0.8.4/cf_xarray/geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/helpers.py` & `cf_xarray-0.8.4/cf_xarray/helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/options.py` & `cf_xarray-0.8.4/cf_xarray/options.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/scripts/make_doc.py` & `cf_xarray-0.8.4/cf_xarray/scripts/make_doc.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/sgrid.py` & `cf_xarray-0.8.4/cf_xarray/sgrid.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/__init__.py` & `cf_xarray-0.8.4/cf_xarray/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/test_accessor.py` & `cf_xarray-0.8.4/cf_xarray/tests/test_accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -997,14 +997,25 @@
 
     actual = ds.cf["temp"].coords["rotated_pole"].drop_vars("rotated_pole")
     assert_identical(actual, expected)
 
     actual = ds.cf["temp"].cf["rotated_latitude_longitude"]
     assert_identical(actual, expected)
 
+    # not properly propagated if grid mapping variable not in coords
+    with pytest.raises(
+        ValueError, match="Grid Mapping variable rotated_pole not present."
+    ):
+        ds.temp.cf.grid_mapping_name
+
+    # check for https://github.com/xarray-contrib/cf-xarray/issues/448
+    expected = ds.rlon
+    actual = rotds.temp.cf["X"]
+    assert_identical(expected, actual)
+
     # Test repr
     expected = """\
            Grid Mappings:   rotated_latitude_longitude: ['rotated_pole']"""
     assert dedent(expected) in ds.cf.__repr__()
     # assert dedent(expected) in ds.cf["temp"].cf.__repr__()
 
     # grid_mapping_name
```

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/test_coding.py` & `cf_xarray-0.8.4/cf_xarray/tests/test_coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/test_geometry.py` & `cf_xarray-0.8.4/cf_xarray/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/test_helpers.py` & `cf_xarray-0.8.4/cf_xarray/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/test_scripts.py` & `cf_xarray-0.8.4/cf_xarray/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/tests/test_units.py` & `cf_xarray-0.8.4/cf_xarray/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/units.py` & `cf_xarray-0.8.4/cf_xarray/units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray/utils.py` & `cf_xarray-0.8.4/cf_xarray/utils.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/cf_xarray.egg-info/PKG-INFO` & `cf_xarray-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cf-xarray
-Version: 0.8.3
+Name: cf_xarray
+Version: 0.8.4
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.3/cf_xarray.egg-info/SOURCES.txt` & `cf_xarray-0.8.4/cf_xarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/2D_bounds_averaged.png` & `cf_xarray-0.8.4/doc/2D_bounds_averaged.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/2D_bounds_error.png` & `cf_xarray-0.8.4/doc/2D_bounds_error.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/2D_bounds_nonunique.png` & `cf_xarray-0.8.4/doc/2D_bounds_nonunique.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/Makefile` & `cf_xarray-0.8.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/_static/dataset-diagram-logo.tex` & `cf_xarray-0.8.4/doc/_static/dataset-diagram-logo.tex`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/_static/full-logo.png` & `cf_xarray-0.8.4/doc/_static/full-logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/_static/logo.png` & `cf_xarray-0.8.4/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/_static/logo.svg` & `cf_xarray-0.8.4/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/_static/rich-repr-example.png` & `cf_xarray-0.8.4/doc/_static/rich-repr-example.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/api.rst` & `cf_xarray-0.8.4/doc/api.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/bounds.md` & `cf_xarray-0.8.4/doc/bounds.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/cartopy_rotated_pole.png` & `cf_xarray-0.8.4/doc/cartopy_rotated_pole.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/coding.md` & `cf_xarray-0.8.4/doc/coding.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/conf.py` & `cf_xarray-0.8.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/contributing.rst` & `cf_xarray-0.8.4/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/coord_axes.md` & `cf_xarray-0.8.4/doc/coord_axes.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/custom-criteria.md` & `cf_xarray-0.8.4/doc/custom-criteria.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/dsg.md` & `cf_xarray-0.8.4/doc/dsg.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/examples/introduction.ipynb` & `cf_xarray-0.8.4/doc/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/flags.md` & `cf_xarray-0.8.4/doc/flags.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/grid_mappings.md` & `cf_xarray-0.8.4/doc/grid_mappings.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/howtouse.md` & `cf_xarray-0.8.4/doc/howtouse.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/index.rst` & `cf_xarray-0.8.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/make.bat` & `cf_xarray-0.8.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/parametricz.md` & `cf_xarray-0.8.4/doc/parametricz.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/plotting.md` & `cf_xarray-0.8.4/doc/plotting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/provenance.md` & `cf_xarray-0.8.4/doc/provenance.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/quickstart.md` & `cf_xarray-0.8.4/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/roadmap.rst` & `cf_xarray-0.8.4/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/selecting.md` & `cf_xarray-0.8.4/doc/selecting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/sgrid_ugrid.md` & `cf_xarray-0.8.4/doc/sgrid_ugrid.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/units.md` & `cf_xarray-0.8.4/doc/units.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/doc/whats-new.rst` & `cf_xarray-0.8.4/doc/whats-new.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.3/pyproject.toml` & `cf_xarray-0.8.4/pyproject.toml`

 * *Files identical despite different names*

