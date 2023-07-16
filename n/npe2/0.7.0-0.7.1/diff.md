# Comparing `tmp/npe2-0.7.0.tar.gz` & `tmp/npe2-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npe2-0.7.0.tar", last modified: Fri Apr 14 13:05:40 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `npe2-0.7.0.tar` & `npe2-0.7.1.tar`

### file list

```diff
@@ -1,122 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/test_all_plugins.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/test_conversion.yml
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-14 13:05:24.000000 npe2-0.7.0/.github/workflows/update_changelog.yml
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-14 13:05:24.000000 npe2-0.7.0/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-14 13:05:24.000000 npe2-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 13:05:24.000000 npe2-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    25594 2023-04-14 13:05:24.000000 npe2-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 13:05:24.000000 npe2-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 13:05:24.000000 npe2-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-14 13:05:24.000000 npe2-0.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-14 13:05:40.288337 npe2-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-14 13:05:24.000000 npe2-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-14 13:05:24.000000 npe2-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:05:40.288337 npe2-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.276337 npe2-0.7.0/src/npe2/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_command_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_dynamic_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.276337 npe2-0.7.0/src/npe2/_inspection/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_from_npe1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_full_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_setuputils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_inspection/_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/_setuptools_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16066 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/implements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/implements.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/io_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.280337 npe2-0.7.0/src/npe2/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_bases.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_npe1_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.280337 npe2-0.7.0/src/npe2/manifest/contributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_contributions.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_icon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_keybindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_menus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_submenu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/contributions/_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/menus.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    20080 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/manifest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-14 13:05:24.000000 npe2-0.7.0/src/npe2/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.276337 npe2-0.7.0/src/npe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 13:05:40.000000 npe2-0.7.0/src/npe2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.272337 npe2-0.7.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/fixtures/my-compiled-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_a.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_b.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/fixtures/my-compiled-plugin/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/npe1-plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/METADATA
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.284337 npe2-0.7.0/tests/npe1-plugin/npe1_module/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/npe1_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/npe1-plugin/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/tests/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/_with_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/tests/sample/my_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:05:40.288337 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/METADATA
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/sample/my_plugin-1.2.3.dist-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test__io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_all_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_config_contribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_contributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_npe1_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_package_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_pm_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_setuptools_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_tmp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-14 13:05:24.000000 npe2-0.7.0/tests/test_validations.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 npe2-0.7.1/.github_changelog_generator
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 npe2-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    27359 2020-02-02 00:00:00.000000 npe2-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 npe2-0.7.1/Makefile
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 npe2-0.7.1/codecov.yml
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 npe2-0.7.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 npe2-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 npe2-0.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 npe2-0.7.1/.github/workflows/test_all_plugins.yml
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 npe2-0.7.1/.github/workflows/test_conversion.yml
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 npe2-0.7.1/.github/workflows/update_changelog.yml
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/example_manifest.yaml
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/render.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/example_plugin/__init__.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/example_plugin/some_module.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/templates/_npe2_contributions.md.jinja
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/templates/_npe2_manifest.md.jinja
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/templates/_npe2_readers_guide.md.jinja
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/templates/_npe2_sample_data_guide.md.jinja
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/templates/_npe2_widgets_guide.md.jinja
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 npe2-0.7.1/_docs/templates/_npe2_writers_guide.md.jinja
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 npe2-0.7.1/docs/_config.yml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 npe2-0.7.1/docs/_toc.yml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 npe2-0.7.1/docs/index.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 npe2-0.7.1/docs/requirements.txt
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/__init__.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_command_registry.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_dynamic_plugin.py
+-rw-r--r--   0        0        0    28875 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_plugin_manager.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_pytest_plugin.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_setuptools_plugin.py
+-rw-r--r--   0        0        0    16066 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/cli.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/implements.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/implements.pyi
+-rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/io_utils.py
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/plugin_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/py.typed
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/types.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/__init__.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/_compile.py
+-rw-r--r--   0        0        0    15273 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/_fetch.py
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/_from_npe1.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/_full_install.py
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/_setuputils.py
+-rw-r--r--   0        0        0    19738 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/_inspection/_visitors.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/__init__.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/_bases.py
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/_npe1_adapter.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/_package_metadata.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/_validators.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/menus.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/package_metadata.py
+-rw-r--r--   0        0        0    20116 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/schema.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/utils.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/__init__.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_commands.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_configuration.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_contributions.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_icon.py
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_json_schema.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_keybindings.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_menus.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_readers.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_sample_data.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_submenu.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_themes.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_widgets.py
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 npe2-0.7.1/src/npe2/manifest/contributions/_writers.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     7145 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test__io_utils.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_all_plugins.py
+-rw-r--r--   0        0        0     8339 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_compile.py
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_config_contribution.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_contributions.py
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_conversion.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_docs.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_fetch.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_implements.py
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_manifest.py
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_npe1_adapter.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_package_meta.py
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_plugin_manager.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_pm_module.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_setuptools_plugin.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_tmp_plugin.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_utils.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/test_validations.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/fixtures/my-compiled-plugin/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/fixtures/my-compiled-plugin/my_module/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/fixtures/my-compiled-plugin/my_module/_a.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/fixtures/my-compiled-plugin/my_module/_b.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/npe1-plugin/setup.cfg
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/npe1-plugin/npe1-plugin-0.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/npe1-plugin/npe1_module/__init__.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/sample/_with_decorators.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/sample/my_plugin/__init__.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/sample/my_plugin/napari.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/sample/my_plugin-1.2.3.dist-info/METADATA
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/sample/my_plugin-1.2.3.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 npe2-0.7.1/tests/sample/my_plugin-1.2.3.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 npe2-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 npe2-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 npe2-0.7.1/README.md
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 npe2-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 npe2-0.7.1/PKG-INFO
```

### Comparing `npe2-0.7.0/.github/workflows/ci.yml` & `npe2-0.7.1/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
         platform: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
@@ -62,19 +62,19 @@
         with:
           repository: napari/napari
           path: napari-from-github
           fetch-depth: 0
 
       - uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: "3.10"
       - name: Install
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -e ./napari-from-github
+          python -m pip install -e ./napari-from-github -c "./napari-from-github/resources/constraints/constraints_py3.10.txt"
           python -m pip install -e .[json]
           # bare minimum required to test napari/plugins
           python -m pip install pytest scikit-image[data] zarr xarray hypothesis matplotlib
 
       - name: Run napari plugin headless tests
         run: pytest -W 'ignore::DeprecationWarning' napari/plugins napari/settings napari/layers napari/components
         working-directory: napari-from-github
```

### Comparing `npe2-0.7.0/.github/workflows/test_all_plugins.yml` & `npe2-0.7.1/.github/workflows/test_all_plugins.yml`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/.github/workflows/test_conversion.yml` & `npe2-0.7.1/.github/workflows/test_conversion.yml`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/.github/workflows/update_changelog.yml` & `npe2-0.7.1/.github/workflows/update_changelog.yml`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/.github_changelog_generator` & `npe2-0.7.1/.github_changelog_generator`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/.gitignore` & `npe2-0.7.1/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 parts/
 sdist/
 var/
 wheels/
 *.egg-info/
 .installed.cfg
 *.egg
+.DS_Store
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
@@ -96,14 +97,15 @@
 .ropeproject
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+.ruff_cache/
 
 # IDE settings
 .vscode/
 src/npe2/_version.py
 
 # ignore everything that gets rendered from _docs
 docs/plugins/*.md
```

### Comparing `npe2-0.7.0/.pre-commit-config.yaml` & `npe2-0.7.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.263
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies:
           - types-toml
           - types-PyYAML
         exclude: npe2/implements.pyi|_docs/render.py
```

### Comparing `npe2-0.7.0/CHANGELOG.md` & `npe2-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 # Changelog
 
+## [v0.7.1](https://github.com/napari/npe2/tree/v0.7.1) (2023-07-16)
+
+[Full Changelog](https://github.com/napari/npe2/compare/v0.7.0...v0.7.1)
+
+**Implemented enhancements:**
+
+- feat: support python3.11 [\#293](https://github.com/napari/npe2/pull/293) ([tlambert03](https://github.com/tlambert03))
+- add graph layer  [\#292](https://github.com/napari/npe2/pull/292) ([JoOkuma](https://github.com/JoOkuma))
+
+**Fixed bugs:**
+
+- fix: use constraints in napari tests [\#298](https://github.com/napari/npe2/pull/298) ([Czaki](https://github.com/Czaki))
+- Use full `plugin_name` when finding chosen `reader` rather than `startswith` [\#297](https://github.com/napari/npe2/pull/297) ([DragaDoncila](https://github.com/DragaDoncila))
+- Change ArrayLike type to use read only properties [\#289](https://github.com/napari/npe2/pull/289) ([andy-sweet](https://github.com/andy-sweet))
+- Bugfix: use .lower\(\) to make paths & pattern fnmatch case  insensitive [\#275](https://github.com/napari/npe2/pull/275) ([psobolewskiPhD](https://github.com/psobolewskiPhD))
+
+**Documentation:**
+
+- Fix typo in `DynamicPlugin` [\#304](https://github.com/napari/npe2/pull/304) ([lucyleeow](https://github.com/lucyleeow))
+- DOCS: Widget guide should consistently use parent=None kwarg in examples [\#302](https://github.com/napari/npe2/pull/302) ([GenevieveBuckley](https://github.com/GenevieveBuckley))
+
+**Merged pull requests:**
+
+- remove tomlpp [\#294](https://github.com/napari/npe2/pull/294) ([tlambert03](https://github.com/tlambert03))
+- Use hatchling as build backend [\#282](https://github.com/napari/npe2/pull/282) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.7.0](https://github.com/napari/npe2/tree/v0.7.0) (2023-04-14)
 
 [Full Changelog](https://github.com/napari/npe2/compare/v0.6.2...v0.7.0)
 
 **Fixed bugs:**
 
 - fix: pass command registry to rdr.exec in io\_utils.\_read [\#285](https://github.com/napari/npe2/pull/285) ([tlambert03](https://github.com/tlambert03))
@@ -22,14 +48,15 @@
 
 **Documentation:**
 
 - Fix link to magicgui objects.inv in intersphinx [\#270](https://github.com/napari/npe2/pull/270) ([melissawm](https://github.com/melissawm))
 
 **Merged pull requests:**
 
+- chore: changelog v0.7.0 [\#286](https://github.com/napari/npe2/pull/286) ([tlambert03](https://github.com/tlambert03))
 - ci\(dependabot\): bump peter-evans/create-pull-request from 4 to 5 [\#284](https://github.com/napari/npe2/pull/284) ([dependabot[bot]](https://github.com/apps/dependabot))
 - Pin pydantic bellow 2.0 [\#279](https://github.com/napari/npe2/pull/279) ([Czaki](https://github.com/Czaki))
 
 ## [v0.6.2](https://github.com/napari/npe2/tree/v0.6.2) (2023-01-12)
 
 [Full Changelog](https://github.com/napari/npe2/compare/v0.6.1...v0.6.2)
 
@@ -183,15 +210,15 @@
 
 **Fixed bugs:**
 
 - hide docs again in napari menus \(Fix napari docs build\) [\#178](https://github.com/napari/npe2/pull/178) ([tlambert03](https://github.com/tlambert03))
 
 ## [v0.4.0](https://github.com/napari/npe2/tree/v0.4.0) (2022-06-13)
 
-[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0...v0.4.0)
+[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0.rc0...v0.4.0)
 
 **Implemented enhancements:**
 
 - Turn menus contributions into dict of arbitrary key to list of MenuItems [\#175](https://github.com/napari/npe2/pull/175) ([tlambert03](https://github.com/tlambert03))
 - Add minor conveniences for DynamicPlugin [\#173](https://github.com/napari/npe2/pull/173) ([tlambert03](https://github.com/tlambert03))
 - Add `plugin_manager` module for global singleton convenience  [\#164](https://github.com/napari/npe2/pull/164) ([tlambert03](https://github.com/tlambert03))
 - Allow arbitrary menu locations in npe2 [\#160](https://github.com/napari/npe2/pull/160) ([sofroniewn](https://github.com/sofroniewn))
@@ -213,21 +240,21 @@
 - Push stack=... through all the reader internal API, take II [\#142](https://github.com/napari/npe2/pull/142) ([Carreau](https://github.com/Carreau))
 
 **Documentation:**
 
 - Add doc links to README [\#158](https://github.com/napari/npe2/pull/158) ([nclack](https://github.com/nclack))
 - Fix codeblock directive in docstring [\#156](https://github.com/napari/npe2/pull/156) ([melissawm](https://github.com/melissawm))
 
-## [v0.3.0](https://github.com/napari/npe2/tree/v0.3.0) (2022-04-05)
+## [v0.3.0.rc0](https://github.com/napari/npe2/tree/v0.3.0.rc0) (2022-04-05)
 
-[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0.rc0...v0.3.0)
+[Full Changelog](https://github.com/napari/npe2/compare/v0.3.0...v0.3.0.rc0)
 
-## [v0.3.0.rc0](https://github.com/napari/npe2/tree/v0.3.0.rc0) (2022-04-05)
+## [v0.3.0](https://github.com/napari/npe2/tree/v0.3.0) (2022-04-05)
 
-[Full Changelog](https://github.com/napari/npe2/compare/v0.2.2...v0.3.0.rc0)
+[Full Changelog](https://github.com/napari/npe2/compare/v0.2.2...v0.3.0)
 
 **Implemented enhancements:**
 
 - NPE1Adapter Part 3 - caching of adapter manifests [\#126](https://github.com/napari/npe2/pull/126) ([tlambert03](https://github.com/tlambert03))
 - NPE1Adapter Part 2 - adding the NPE1Adapter object. [\#125](https://github.com/napari/npe2/pull/125) ([tlambert03](https://github.com/tlambert03))
 - NPE1Adapter Part 1 - updated \_from\_npe1 conversion logic to prepare for locally defined objects [\#124](https://github.com/napari/npe2/pull/124) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `npe2-0.7.0/LICENSE` & `npe2-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/Makefile` & `npe2-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/README.md` & `npe2-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/pyproject.toml` & `npe2-0.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # pyproject.toml
 [build-system]
-requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
+
+[tool.hatch.version]
+source = "vcs"
 
 # https://peps.python.org/pep-0621/
 [project]
 name = "npe2"
 dynamic = ["version"]
 description = "napari plugin engine v2"
 readme = "README.md"
@@ -20,37 +23,39 @@
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = [
     "PyYAML",
     "appdirs",
     "build",
     "psygnal>=0.3.0",
     "pydantic<2",
-    "pytomlpp",
+    "tomli-w",
+    "tomli; python_version < '3.11'",
     "rich",
     "typer",
 ]
 
 [project.urls]
 homepage = "https://github.com/napari/npe2"
 repository = "https://github.com/napari/npe2"
 
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 testing = [
     "magicgui",
     "napari-plugin-engine",
-    "napari-svg",
+    "napari-svg==0.1.5",
     "numpy",
     "pytest",
     "pytest-cov",
     "jsonschema",
 ]
 dev = ["black", "ipython", "isort", "mypy", "pre-commit"]
 docs = ["Jinja2", "magicgui>=0.3.3"]
@@ -67,33 +72,17 @@
 
 [project.entry-points."pytest11"]
 npe2 = "npe2._pytest_plugin"
 
 [project.entry-points."setuptools.finalize_distribution_options"]
 finalize_npe2 = "npe2._setuptools_plugin:finalize_npe2"
 
-[tool.setuptools]
-package-dir = { "" = "src" }
-include-package-data = true
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.setuptools.package-data]
-"*" = ["*.pyi", "py.typed"]
-
-[tool.setuptools_scm]
-write_to = "src/npe2/_version.py"
 
 [tool.check-manifest]
-ignore = [
-    "src/npe2/_version.py",
-    ".pre-commit-config.yaml",
-    ".github_changelog_generator",
-]
+ignore = []
 
 [tool.pytest.ini_options]
 filterwarnings = ["error:::npe2"]
 addopts = "-m 'not github_main_only'"
 markers = [
     "github_main_only: Test to run only on github main (verify it does not break latest napari docs build)",
 ]
```

### Comparing `npe2-0.7.0/src/npe2/__init__.py` & `npe2-0.7.1/src/npe2/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from importlib.metadata import PackageNotFoundError, version
+
 try:
-    from ._version import version as __version__
-except ImportError:
+    __version__ = version("npe2")
+except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 __author__ = "Talley Lambert"
 __email__ = "talley.lambert@gmail.com"
 
 
 from ._dynamic_plugin import DynamicPlugin
 from ._inspection._fetch import fetch_manifest, get_manifest_from_wheel
```

### Comparing `npe2-0.7.0/src/npe2/_command_registry.py` & `npe2-0.7.1/src/npe2/_command_registry.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/_dynamic_plugin.py` & `npe2-0.7.1/src/npe2/_dynamic_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         return self.manifest.display_name
 
     def cleanup(self) -> None:
         """Remove this plugin from its plugin manager."""
         self.plugin_manager.unregister(self.manifest.name)
 
     def register(self) -> None:
-        """Remove this plugin from its plugin manager."""
+        """Register this plugin with its plugin manager."""
         self.plugin_manager.register(self.manifest)
 
     def clear(self) -> None:
         """Clear contributions."""
         self.plugin_manager.deactivate(self.manifest.name)
         self.plugin_manager._contrib.remove_contributions(self.manifest.name)
         self.manifest.contributions = ContributionPoints()
```

### Comparing `npe2-0.7.0/src/npe2/_inspection/_compile.py` & `npe2-0.7.1/src/npe2/_inspection/_compile.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/_inspection/_fetch.py` & `npe2-0.7.1/src/npe2/_inspection/_fetch.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/_inspection/_from_npe1.py` & `npe2-0.7.1/src/npe2/_inspection/_from_npe1.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/_inspection/_full_install.py` & `npe2-0.7.1/src/npe2/_inspection/_full_install.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/_inspection/_setuputils.py` & `npe2-0.7.1/src/npe2/_inspection/_setuputils.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,26 +82,14 @@
             for group, vals in visitor.get("entry_points", {}).items():
                 for val in vals if isinstance(vals, list) else [vals]:
                     name, _, value = val.partition("=")
                     info.entry_points.append(
                         EntryPoint(name.strip(), value.strip(), group)
                     )
 
-    # # check for pyproject.toml
-    # pyproject_toml = path / "pyproject.toml"
-    # if pyproject_toml.exists():
-    #     info.pyproject_toml = pyproject_toml
-    #     with open(pyproject_toml, "r") as f:
-    #         data = pytomlpp.load(f)
-    #     if project := data.get("project"):
-    #         info.package_name = project.get("name", "")
-    #         for group, ep in project.get('entry-points', {}).items():
-    #             for name, value in ep.items():
-    #                 info.entry_points.append(EntryPoint(name, value, group))
-
     return info
 
 
 class _SetupVisitor(ast.NodeVisitor):
     """Visitor to statically determine metadata from setup.py"""
 
     def __init__(self) -> None:
```

### Comparing `npe2-0.7.0/src/npe2/_inspection/_visitors.py` & `npe2-0.7.1/src/npe2/_inspection/_visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,14 +231,17 @@
         )
         self.contribution_points["readers"].append(rdr_contrib)
 
     def napari_get_writer(self, node: ast.FunctionDef):
         # we can't convert this to an npe2 command contribution
         pass  # pragma: no cover
 
+    def napari_write_graph(self, node: ast.FunctionDef):
+        self._parse_writer(node, "graph")  # pragma: no cover
+
     def napari_write_image(self, node: ast.FunctionDef):
         self._parse_writer(node, "image")
 
     def napari_write_labels(self, node: ast.FunctionDef):
         self._parse_writer(node, "labels")  # pragma: no cover
 
     def napari_write_points(self, node: ast.FunctionDef):
```

### Comparing `npe2-0.7.0/src/npe2/_plugin_manager.py` & `npe2-0.7.1/src/npe2/_plugin_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import contextlib
 import os
+import urllib
 import warnings
 from collections import Counter
 from fnmatch import fnmatch
 from importlib import metadata
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
@@ -134,19 +135,28 @@
         if not path:
             return
         assert isinstance(path, str)
 
         if os.path.isdir(path):
             yield from (r for pattern, r in self._readers if pattern == "")
         else:
+            # ensure not a URI
+            if not urllib.parse.urlparse(path).scheme:
+                # lower case the extension for checking manifest pattern
+                base = os.path.splitext(Path(path).stem)[0]
+                ext = "".join(Path(path).suffixes)
+                path = base + ext.lower()
             # not sure about the set logic as it won't be lazy anymore,
             # but would we yield duplicate anymore.
             # above does not have have the unseen check either.
             # it's easy to make an iterable version if we wish, or use more-itertools.
-            yield from {r for pattern, r in self._readers if fnmatch(path, pattern)}
+            # match against pattern.lower() to make matching case insensitive
+            yield from {
+                r for pattern, r in self._readers if fnmatch(path, pattern.lower())
+            }
 
     def iter_compatible_writers(
         self, layer_types: Sequence[str]
     ) -> Iterator[WriterContribution]:
         """Attempt to match writers that consume all layers."""
 
         if not layer_types:
```

### Comparing `npe2-0.7.0/src/npe2/_pytest_plugin.py` & `npe2-0.7.1/src/npe2/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/_setuptools_plugin.py` & `npe2-0.7.1/src/npe2/_setuptools_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,20 @@
 
 def trace(*k: object) -> None:
     if DEBUG:
         print(*k, file=sys.stderr, flush=True)
 
 
 def _lazy_tomli_load(data: str) -> dict[str, Any]:
-    from pytomlpp import loads
+    try:
+        import tomllib
+    except ImportError:
+        import tomli as tomllib  # type: ignore [no-redef]
 
-    return loads(data)
+    return tomllib.loads(data)
 
 
 def _read_dist_name_from_setup_cfg() -> str | None:
     # minimal effort to read dist_name off setup.cfg metadata
     import configparser
 
     parser = configparser.ConfigParser()
```

### Comparing `npe2-0.7.0/src/npe2/cli.py` & `npe2-0.7.1/src/npe2/cli.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/implements.py` & `npe2-0.7.1/src/npe2/implements.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/implements.pyi` & `npe2-0.7.1/src/npe2/implements.pyi`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/io_utils.py` & `npe2-0.7.1/src/npe2/io_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     _pm: Optional[PluginManager] = None,
 ) -> Union[Tuple[List[LayerData], ReaderContribution], List[LayerData]]:
     """Execute the `read...` functions above."""
     if _pm is None:
         _pm = PluginManager.instance()
 
     for rdr in _pm.iter_compatible_readers(paths):
-        if plugin_name and not rdr.command.startswith(plugin_name):
+        if plugin_name and rdr.plugin_name != plugin_name:
             continue
         read_func = rdr.exec(
             kwargs={"path": paths, "stack": stack, "_registry": _pm.commands}
         )
         if read_func is not None:
             # if the reader function raises an exception here, we don't try to catch it
             if layer_data := read_func(paths, stack=stack):
```

### Comparing `npe2-0.7.0/src/npe2/manifest/_bases.py` & `npe2-0.7.1/src/npe2/manifest/_bases.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Callable, Dict, Optional, Union
 
-import pytomlpp as toml
 import yaml
 from pydantic import BaseModel, PrivateAttr
 
 
 class ImportExportModel(BaseModel):
     """Model mixin/base class that provides read/write from toml/yaml/json.
 
@@ -26,18 +25,20 @@
         ----------
         pyproject : bool, optional
             If `True`, output will be in pyproject format, with all data under
             `tool.napari`, by default `False`.
         **kwargs
             passed to `BaseModel.json()`
         """
+        import tomli_w
+
         d = self._serialized_data(**kwargs)
         if pyproject:
             d = {"tool": {"napari": d}}
-        return toml.dumps(d)
+        return tomli_w.dumps(d)
 
     def yaml(self, **kwargs) -> str:
         """Generate serialized `yaml` string for this model.
 
         Parameters
         ----------
         **kwargs
@@ -70,21 +71,26 @@
         if not path.exists():
             raise FileNotFoundError(f"File not found: {path}")
 
         loader: Callable
         if path.suffix.lower() == ".json":
             loader = json.load
         elif path.suffix.lower() == ".toml":
-            loader = toml.load
+            try:
+                import tomllib
+            except ImportError:
+                import tomli as tomllib  # type: ignore [no-redef]
+
+            loader = tomllib.load
         elif path.suffix.lower() in (".yaml", ".yml"):
             loader = yaml.safe_load
         else:
             raise ValueError(f"unrecognized file extension: {path}")  # pragma: no cover
 
-        with open(path, encoding="utf-8") as f:
+        with open(path, mode="rb") as f:
             data = loader(f) or {}
 
         if path.name == "pyproject.toml":
             data = data["tool"]["napari"]
 
         obj = cls(**data)
         obj._source_file = Path(path).expanduser().absolute().resolve()
```

### Comparing `npe2-0.7.0/src/npe2/manifest/_npe1_adapter.py` & `npe2-0.7.1/src/npe2/manifest/_npe1_adapter.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/_package_metadata.py` & `npe2-0.7.1/src/npe2/manifest/_package_metadata.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/_validators.py` & `npe2-0.7.1/src/npe2/manifest/_validators.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/__init__.py` & `npe2-0.7.1/src/npe2/manifest/contributions/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_commands.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_commands.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_configuration.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_configuration.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_contributions.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_contributions.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_json_schema.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_json_schema.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_keybindings.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_keybindings.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_menus.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_menus.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_readers.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_readers.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_sample_data.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_sample_data.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_submenu.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_submenu.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_themes.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_themes.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_widgets.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_widgets.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/manifest/contributions/_writers.py` & `npe2-0.7.1/src/npe2/manifest/contributions/_writers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from pydantic import BaseModel, Extra, Field, validator
 
 from npe2.manifest.utils import Executable
 
 
 class LayerType(str, Enum):
+    graph = "graph"
     image = "image"
     labels = "labels"
     points = "points"
     shapes = "shapes"
     surface = "surface"
     tracks = "tracks"
     vectors = "vectors"
```

### Comparing `npe2-0.7.0/src/npe2/manifest/schema.py` & `npe2-0.7.1/src/npe2/manifest/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,16 +364,17 @@
                         dist.metadata["Name"],
                         dist.metadata["Name"],
                     )
                     yield DiscoverResults(None, dist, e)
 
                 except Exception as e:
                     logger.error(
-                        "%s -> %r could not be imported: %s"
-                        % (ENTRY_POINT, dist.metadata["Name"], e)
+                        "{} -> {!r} could not be imported: {}".format(
+                            ENTRY_POINT, dist.metadata["Name"], e
+                        )
                     )
                     yield DiscoverResults(None, dist, e)
 
     @classmethod
     def _from_entrypoint(
         cls,
         entry_point: metadata.EntryPoint,
```

### Comparing `npe2-0.7.0/src/npe2/manifest/utils.py` & `npe2-0.7.1/src/npe2/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/plugin_manager.py` & `npe2-0.7.1/src/npe2/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/src/npe2/types.py` & `npe2-0.7.1/src/npe2/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,24 +25,32 @@
 PathOrPaths = Union[PathLike, Sequence[PathLike]]
 PythonName = NewType("PythonName", str)
 
 # Layer-related types
 
 
 class ArrayLike(Protocol):
-    shape: Tuple[int, ...]
-    ndim: int
-    dtype: "np.dtype"
+    @property
+    def shape(self) -> Tuple[int, ...]:
+        ...
+
+    @property
+    def ndim(self) -> int:
+        ...
+
+    @property
+    def dtype(self) -> "np.dtype":
+        ...
 
     def __array__(self) -> "np.ndarray":
         ...  # pragma: no cover
 
 
 LayerName = Literal[
-    "image", "labels", "points", "shapes", "surface", "tracks", "vectors"
+    "graph", "image", "labels", "points", "shapes", "surface", "tracks", "vectors"
 ]
 Metadata = Dict
 DataType = Union[ArrayLike, Sequence[ArrayLike]]
 FullLayerData = Tuple[DataType, Metadata, LayerName]
 LayerData = Union[Tuple[DataType], Tuple[DataType, Metadata], FullLayerData]
 
 # ########################## CONTRIBUTIONS #################################
```

### Comparing `npe2-0.7.0/tests/conftest.py` & `npe2-0.7.1/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     from napari_plugin_engine import PluginManager, napari_hook_specification
 
     # fmt: off
     class HookSpecs:
         def napari_provide_sample_data(): ...  # type: ignore
         def napari_get_reader(path): ...
         def napari_get_writer(path, layer_types): ...
+        def napari_write_graph(path, data, meta): ...
         def napari_write_image(path, data, meta): ...
         def napari_write_labels(path, data, meta): ...
         def napari_write_points(path, data, meta): ...
         def napari_write_shapes(path, data, meta): ...
         def napari_write_surface(path, data, meta): ...
         def napari_write_vectors(path, data, meta): ...
         def napari_experimental_provide_function(): ...  # type: ignore
```

### Comparing `npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_a.py` & `npe2-0.7.1/tests/fixtures/my-compiled-plugin/my_module/_a.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/fixtures/my-compiled-plugin/my_module/_b.py` & `npe2-0.7.1/tests/fixtures/my-compiled-plugin/my_module/_b.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/npe1-plugin/npe1_module/__init__.py` & `npe2-0.7.1/tests/npe1-plugin/npe1_module/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/sample/_with_decorators.py` & `npe2-0.7.1/tests/sample/_with_decorators.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/sample/my_plugin/__init__.py` & `npe2-0.7.1/tests/sample/my_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/sample/my_plugin/napari.yaml` & `npe2-0.7.1/tests/sample/my_plugin/napari.yaml`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_all_plugins.py` & `npe2-0.7.1/tests/test_all_plugins.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_cli.py` & `npe2-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_compile.py` & `npe2-0.7.1/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_config_contribution.py` & `npe2-0.7.1/tests/test_config_contribution.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_contributions.py` & `npe2-0.7.1/tests/test_contributions.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_conversion.py` & `npe2-0.7.1/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_docs.py` & `npe2-0.7.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_fetch.py` & `npe2-0.7.1/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_implements.py` & `npe2-0.7.1/tests/test_implements.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_manifest.py` & `npe2-0.7.1/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_npe1_adapter.py` & `npe2-0.7.1/tests/test_npe1_adapter.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_package_meta.py` & `npe2-0.7.1/tests/test_package_meta.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_plugin_manager.py` & `npe2-0.7.1/tests/test_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_pm_module.py` & `npe2-0.7.1/tests/test_pm_module.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_pytest_plugin.py` & `npe2-0.7.1/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_setuptools_plugin.py` & `npe2-0.7.1/tests/test_setuptools_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_tmp_plugin.py` & `npe2-0.7.1/tests/test_tmp_plugin.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_utils.py` & `npe2-0.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `npe2-0.7.0/tests/test_validations.py` & `npe2-0.7.1/tests/test_validations.py`

 * *Files identical despite different names*

