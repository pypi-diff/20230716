# Comparing `tmp/wiliot-deployment-tools-4.0.7.tar.gz` & `tmp/wiliot-deployment-tools-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-deployment-tools-4.0.7.tar", last modified: Wed May 31 15:37:46 2023, max compression
+gzip compressed data, was "wiliot-deployment-tools-4.0.8.tar", last modified: Tue Jun 13 09:01:38 2023, max compression
```

## Comparing `wiliot-deployment-tools-4.0.7.tar` & `wiliot-deployment-tools-4.0.8.tar`

### file list

```diff
@@ -1,68 +1,73 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.424200 wiliot-deployment-tools-4.0.7/.devcontainer/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/.devcontainer/private/
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/.devcontainer/private/devcontainer.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/.devcontainer/public/
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/.devcontainer/public/devcontainer.json
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7396 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6905 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8812 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/ci.py
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/dep-tools-public.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/dep-tools.dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3457 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/unittests/
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_debug_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_extended_api_edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_extended_api_platform.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2710 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_slack_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.436200 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.440201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    43300 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/extended_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/gw_ssid.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15516 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     3178 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    68575 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/analysis_data_bricks.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     6004 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils_defines.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23066 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.444201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4653 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
--rw-rw-rw-   0 root         (0) root         (0)    28031 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.448201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6057 2023-05-31 15:37:20.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 15:37:46.440201 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7396 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      345 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      362 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-31 15:37:46.000000 wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.942140 wiliot-deployment-tools-4.0.8/.devcontainer/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.946140 wiliot-deployment-tools-4.0.8/.devcontainer/private/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/.devcontainer/private/devcontainer.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.946140 wiliot-deployment-tools-4.0.8/.devcontainer/public/
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/.devcontainer/public/devcontainer.json
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     8103 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7612 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8812 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2625 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/dep-tools-public.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      577 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/dep-tools.dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3599 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/unittests/
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_debug_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_extended_api_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_extended_api_platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2710 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_slack_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    45893 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/extended_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/gw_ssid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/s3_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15516 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     3178 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7926 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68575 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/analysis_data_bricks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     6004 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3135 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils_defines.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23066 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.954141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/log_viewer_cli.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py
+-rw-rw-rw-   0 root         (0) root         (0)    26356 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.958141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6057 2023-06-13 09:01:13.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 09:01:38.950141 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     8103 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2281 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-13 09:01:38.000000 wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/top_level.txt
```

### Comparing `wiliot-deployment-tools-4.0.7/.devcontainer/private/devcontainer.json` & `wiliot-deployment-tools-4.0.8/.devcontainer/private/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/.devcontainer/public/devcontainer.json` & `wiliot-deployment-tools-4.0.8/.devcontainer/public/devcontainer.json`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/LICENSE` & `wiliot-deployment-tools-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/PKG-INFO` & `wiliot-deployment-tools-4.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-Metadata-Version: 2.1
-Name: wiliot-deployment-tools
-Version: 4.0.7
-Summary: A library for interacting with Wiliot's Deployment Tools
-Home-page: 
-Author: Wiliot
-Author-email: support@wiliot.com
-License: MIT
-Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyWiliot: wiliot-deployment-tools #
 
 wiliot-deployment-tools is a python library for accessing Wiliot's Deployment and Automation Tools.
 This python package includes the following CLI utilities:
  - Automatic Configuration Tool (`wlt-config`)
  - Power Management Tool (`wlt-power-mgmt`)
+ - Calibration Management Tool (`wlt-clibration-mgmt`)
  - Firmware Update Tool (`wlt-firmware`)
  - Log Viewer (`wlt-log`)
 
 
 ## Installing wiliot-deployment-tools
 ````commandline
 pip install wiliot-deployment-tools
@@ -62,14 +47,31 @@
 usage: wlt-firmware -owner OWNER [-beta] versions
 
 optional arguments:
   -beta              show available beta versions / update to beta firmware
 
 example usage: wlt-firmware -o wiliot versions
 ```
+### Calibration Management
+Configure Wiliot Bridge calibration mode
+```
+usage: wlt-calibration-mgmt -owner OwnerID -brg BridgeID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
+
+required arguments:
+  -owner OWNER  Owner ID
+  -brg BRG      Bridge ID
+  -gw GW        GW ID to configure bridge
+  -mode Mode    CalibrationMode on of 3 options: 0-regular, 1-no ch37, 2-ch37 on data only
+
+optional arguments:
+
+  -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
+
+  example usage: wlt-calibration-mgmt -owner wiliot -brg 0123ABCD -gw AB1234CD -mode 1
+```
 
  #### Firmware Update
  Run OTA Process, first updating specified GWs to latest / specified FW version. Afterwards seuqentially update each specified Bridges / all Bridges to the same Firmware version.
  ```
 usage: wlt-firmware update -owner OWNER [-beta] [-version VERSION] [-gw GW [GW ...]] [-brg BRG [BRG ...]] [-all_brgs] [-ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]] [-action]
 
 optional arguments:
@@ -122,16 +124,17 @@
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
 example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
+
 ### Log Viewer
-View Wiliot Gatewa logs
+View Wiliot Gateway logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
 Log Viewer - CLI Tool to view Wiliot Gateway logs
 
 required arguments:
   -owner OWNER  Owner ID
@@ -141,14 +144,18 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.8:
+* Support for python 3.11
+* Added new calibration mgmt tool
+
 Version 4.0.7:
 * Android power management support
 * Bugfix when no gateway logs found
   
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
```

### Comparing `wiliot-deployment-tools-4.0.7/README.md` & `wiliot-deployment-tools-4.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,30 @@
+Metadata-Version: 2.1
+Name: wiliot-deployment-tools
+Version: 4.0.8
+Summary: A library for interacting with Wiliot's Deployment Tools
+Home-page: 
+Author: Wiliot
+Author-email: support@wiliot.com
+License: MIT
+Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyWiliot: wiliot-deployment-tools #
 
 wiliot-deployment-tools is a python library for accessing Wiliot's Deployment and Automation Tools.
 This python package includes the following CLI utilities:
  - Automatic Configuration Tool (`wlt-config`)
  - Power Management Tool (`wlt-power-mgmt`)
+ - Calibration Management Tool (`wlt-clibration-mgmt`)
  - Firmware Update Tool (`wlt-firmware`)
  - Log Viewer (`wlt-log`)
 
 
 ## Installing wiliot-deployment-tools
 ````commandline
 pip install wiliot-deployment-tools
@@ -46,14 +63,31 @@
 usage: wlt-firmware -owner OWNER [-beta] versions
 
 optional arguments:
   -beta              show available beta versions / update to beta firmware
 
 example usage: wlt-firmware -o wiliot versions
 ```
+### Calibration Management
+Configure Wiliot Bridge calibration mode
+```
+usage: wlt-calibration-mgmt -owner OwnerID -brg BridgeID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
+
+required arguments:
+  -owner OWNER  Owner ID
+  -brg BRG      Bridge ID
+  -gw GW        GW ID to configure bridge
+  -mode Mode    CalibrationMode on of 3 options: 0-regular, 1-no ch37, 2-ch37 on data only
+
+optional arguments:
+
+  -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
+
+  example usage: wlt-calibration-mgmt -owner wiliot -brg 0123ABCD -gw AB1234CD -mode 1
+```
 
  #### Firmware Update
  Run OTA Process, first updating specified GWs to latest / specified FW version. Afterwards seuqentially update each specified Bridges / all Bridges to the same Firmware version.
  ```
 usage: wlt-firmware update -owner OWNER [-beta] [-version VERSION] [-gw GW [GW ...]] [-brg BRG [BRG ...]] [-all_brgs] [-ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]] [-action]
 
 optional arguments:
@@ -106,16 +140,17 @@
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
 example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
+
 ### Log Viewer
-View Wiliot Gatewa logs
+View Wiliot Gateway logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
 Log Viewer - CLI Tool to view Wiliot Gateway logs
 
 required arguments:
   -owner OWNER  Owner ID
@@ -125,14 +160,18 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.8:
+* Support for python 3.11
+* Added new calibration mgmt tool
+
 Version 4.0.7:
 * Android power management support
 * Bugfix when no gateway logs found
   
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
```

### Comparing `wiliot-deployment-tools-4.0.7/bitbucket-pipelines.yml` & `wiliot-deployment-tools-4.0.8/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/ci.py` & `wiliot-deployment-tools-4.0.8/ci.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/dep-tools.dockerfile` & `wiliot-deployment-tools-4.0.8/dep-tools.dockerfile`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/setup.py` & `wiliot-deployment-tools-4.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,32 +43,33 @@
                      'wiliot-core==4.0.9',
                      'wiliot-api==4.1.2',
                      'bitstruct==8.17.0',
                      'bokeh==2.4.1',
                      'boto3==1.26.77',
                      'colorama==0.4.6',
                      'jsonpickle==3.0.1',
-                     'numpy==1.24.2',
+                     'numpy<=1.24.2',
                      'pandas==1.5.3',
                      'plotly==5.13.0',
                      'pytz==2022.7.1',
                      'requests==2.28.1',
                      'setuptools==65.6.3',
                      'setuptools_scm==7.1.0',
                      'tabulate==0.8.10',
-                     'backports.zoneinfo==0.2.1',
+                     'backports.zoneinfo==0.2.1; python_version < "3.9.0"',
                      'tinytuya==1.10.2',
                      'pyserial==3.5',
                      'GitPython==3.1.31',
                      'tzdata==2023.3'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                 #  include_package_data=False,
                 #  exclude_package_data={
                 #      "": ['*.internal.*', '*.internal', 'internal', 'internal.*']},
                  entry_points={'console_scripts': [
                      'wlt-firmware=wiliot_deployment_tools.firmware_update.firmware_update_cli:main_cli',
                      'wlt-power-mgmt=wiliot_deployment_tools.power_mgmt.power_mgmt_cli:main_cli',
+                     'wlt-calibration-mgmt=wiliot_deployment_tools.calibration_mgmt.calibration_mgmt_cli:main_cli',
                      'wlt-config=wiliot_deployment_tools.automatic_configuration_tool.configuration_tool_cli:main_cli',
                      'wlt-log=wiliot_deployment_tools.log_viewer.log_viewer_cli:main_cli']},
                  )
```

### Comparing `wiliot-deployment-tools-4.0.7/unittests/test_extended_api_edge.py` & `wiliot-deployment-tools-4.0.8/unittests/test_extended_api_edge.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/unittests/test_extended_api_platform.py` & `wiliot-deployment-tools-4.0.8/unittests/test_extended_api_platform.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/unittests/test_power_mgmt.py` & `wiliot-deployment-tools-4.0.8/unittests/test_power_mgmt.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/unittests/test_slack_alerts.py` & `wiliot-deployment-tools-4.0.8/unittests/test_slack_alerts.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/unittests/test_test_tool.py` & `wiliot-deployment-tools-4.0.8/unittests/test_test_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/unittests/test_utils.py` & `wiliot-deployment-tools-4.0.8/unittests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import unittest
-from backports.zoneinfo import ZoneInfo
+try:
+    from zoneinfo import ZoneInfo  # will run only in python 3.9+
+except ImportError:
+    from backports.zoneinfo import ZoneInfo  # backport to python < 3.9
 from wiliot_deployment_tools.common.utils import *
 
 class UtilsTest(unittest.TestCase):
 
     def test_convert_datetime_to_timestamp(self):
         now = datetime.datetime.now()
         timestamp = now.timestamp()
```

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/extended_api.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/extended_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 class BridgeThroughGatewayAction(Enum):
     REBOOT = '01'
     BLINK = '02'
     POWER_MGMT = '03'
     RESTORE_DEFAULTS = '04'
     SEND_HB = '05'
     PRODUCTION_MODE = '06'
+    SPARSE_37 = '07'
 
 
 class BoardTypes(Enum):
     ENERGOUS = 'Energous Dual-Band (v0)'
     FANSTEL_SINGLE = 'Fanstel Single-Band (v0)'
     FANSTEL_DUAL = 'Fanstel Dual-Band (v0)'
     MINEW_SINGLE = 'Minew Single-Band (v0)'
@@ -295,15 +296,14 @@
         assert action_type in BridgeThroughGatewayAction, 'Not valid action type'
         assert (bridge_id is not None and broadcast is False) or (bridge_id is None and broadcast is True), \
             'Must supply bridgeId / set broadcast to True'
         assert reps > 0, 'Repetitions must be a positive value!'
         assert ms_to_send > 0, 'Milliseconds to send must be a positive value!'
         assert len(bridge_id) == 12
         payload = str(payload).ljust(28, '0')
-
         # Packet Header: 0-5 ADVA, 6 Length, 7 AD Type, 8-9 UUID, 10-12 Group ID, 13 MSG type, 14 API Ver.
         header = '1E16C6FC0000ED0707'
         # Randomize Sequence ID
         seq_id = random.getrandbits(8).to_bytes(1, 'big').hex().upper()
         gw_type = self.get_gateway_type(gateway_id)
         if gw_type == GatewayType.MOBILE:
             arg = ms_to_send
@@ -456,14 +456,22 @@
     def get_gw_ble_version(self, gw_id):
         """
         :type gw_id: string
         :param gw_id: gateway id
         """
         gw = self.get_gateway(gw_id)
         return gw["reportedConf"]["bleChipSwVersion"]
+    
+    def get_gw_interface_version(self, gw_id):
+        """
+        :type gw_id: string
+        :param gw_id: gateway id
+        """
+        gw = self.get_gateway(gw_id)
+        return gw["reportedConf"]["interfaceChipSwVersion"]
 
     def get_brg_ble_version(self, brg_id):
         """
         :type brg_id: string
         :param brg_id: bridge id
         """
         brg = self.get_bridge(brg_id)
@@ -574,15 +582,18 @@
             debug_print(f'GW {gw_id} and BRG {brg_id} are both updated to version {self.get_gw_version(gw_id)}')
             return True
         else:
             debug_print(f'GW {gw_id} ver. {gw_ver}, BRG {brg_id} ver. {brg_ver}')
             return False
 
     def check_thin_gw_support(self, gw_id):
-        return self.check_ble_thin_gw_support(self.get_gw_ble_version(gw_id))
+        if self.get_gateway_type(gw_id) == GatewayType.WIFI:
+            return self.check_ble_thin_gw_support(self.get_gw_ble_version(gw_id))
+        else:
+            return True
 
     @staticmethod
     def check_ble_thin_gw_support(ble_ver):
         """
         checks if thin GW is supported for BLE version
         :rtype: bool
         :return: True if supported, False otherwise
@@ -604,21 +615,23 @@
         major, minor, build = [int(v) for v in version]
         if major > 3 or major == 3 and minor > 6 or major == 3 and minor == 6 and build > 28:
             return True
         else:
             return False
 
     # Configuration Changes
-    def change_gw_config(self, gws_list, config_dict, minutes_timeout=5):
+    def change_gw_config(self, gws_list, config_dict, minutes_timeout=5, ignore_missing_params=False):
         """
             change configuration for multiple GWs
             :type gws_list: every iterable type
             :param gws_list: desired gateways to configure
             :type config_dict: dict
             :param config_dict: dictionary of parameters and values to configure
+            :type ignore_missing_params: bool
+            :param ignore_missing_params: if True, will return all GWs as updated as long as all available params have been changed
         """
         if not config_dict:  # check there are parameters to configure
             return gws_list
 
         def check_updated(gw_id, config_dict):
             """
             :param gw_id: Gateway ID
@@ -629,25 +642,35 @@
                 try:
                     gw_version = gw['version']
                     if gw_version != config_dict['version']:
                         return False
                 except KeyError:
                     debug_print(f'Version not yet updated for {gw_id}... sleeping for 30 seconds')
                     sleep(30)
-            gw_dict = gw['reportedConf']['additional']
+            if 'additional' in gw['reportedConf'].keys():
+                gw_dict = gw['reportedConf']['additional']
+            else:
+                gw_dict = {}
             relevant_dict = {}
             missing_keys = []
             for key in config_dict.keys():
                 if key not in gw_dict.keys():
                     missing_keys.append(key)
                 else:
                     relevant_dict.update({key: gw_dict[key]})
             if relevant_dict == config_dict:
                 return True
             if len(missing_keys) > 0:
+                if ignore_missing_params:
+                    relevant_config_dict = config_dict.copy()
+                    for key in missing_keys:
+                        relevant_config_dict.pop(key)
+                    if relevant_dict == relevant_config_dict:
+                        return True
+                    return False
                 raise ParamMissingError(
                     f"{missing_keys} not in GW {gw_id} Parameters! Check FW Version or change desired config")
             return False
 
         desired_version = None
         if 'version' in config_dict.keys():
             desired_version = config_dict.pop('version')
@@ -920,14 +943,55 @@
             browned_out_brgs = list(filter(brgs_brownout_status.get, brgs_brownout_status))
             non_browned_out_brgs = list(set(connected_bridges) - set(browned_out_brgs))
             raise WiliotCloudError(f'Cannot change connected BRGs {non_browned_out_brgs} to brownout! Check deployment!')
         
         debug_print(f'{len(gw_ids)} GWs {gw_ids} Connected')
         debug_print(f'{len(connected_bridges)} BRGs {connected_bridges} Connected')
         return connected_bridges, board_type_dict
+    
+    
+    def check_gw_compatible_for_action(self, gateway_id):
+        """
+        checks if gateway is compatible to send and receive power management configurations
+        :type gateway_id: str
+        :param gateway_id: gateway ID
+        :rtype: bool
+        """
+        gateway_type = self.get_gateway_type(gateway_id)
+        if gateway_type != GatewayType.WIFI:
+            if gateway_type == GatewayType.MOBILE: 
+                return True
+            else:
+                return False
+        gw_dict = self.get_gateway(gateway_id)        
+        ble_ver = gw_dict["reportedConf"]["bleChipSwVersion"]
+        if gw_dict['online']:
+            if gw_dict['reportedConf']['additional']['gwMgmtMode'] == 'transparent':
+                support = self.check_gw_ble_transparent_support(ble_ver)
+                if not support:
+                    debug_print(f'Please update GW {gateway_id} or change to active mode for power management support!')
+                return support
+            return True
+        return False
+    
+    @staticmethod
+    def check_gw_ble_transparent_support(ble_ver):
+        """
+        checks if power management is supported for transparent GW BLE version
+        :rtype: bool
+        :return: True if supported, False otherwise
+        """
+        ble_ver = ble_ver.split('.')
+        if not ((int(ble_ver[0]) > 3) or
+                (int(ble_ver[0]) > 2 and int(ble_ver[1]) > 14) or \
+                (int(ble_ver[0]) > 2 and int(ble_ver[1]) > 13 and int(ble_ver[2]) > 27)):
+            return False
+        else:
+            return True
+
 
 
 class ExtendedPlatformClient(PlatformClient):
     def __init__(self, api_key, owner_id, env='', log_file=None, logger_=None):
         super().__init__(api_key, owner_id, env, log_file, logger_)
 
     def get_locations(self, locations=None):
```

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/api/gw_ssid.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/api/gw_ssid.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/analysis_data_bricks.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/analysis_data_bricks.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/debug.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/debug.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/common/utils_defines.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/common/utils_defines.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,16 @@
     "sub1GhzOutputPower": 32,
     "sub1GhzFrequency": 919100,
     "rxTxPeriodMs": 15,
     "txPeriodMs": 5,
     "txProbability": 50,
     "otaUpgradeEnabled": 0,
     "pacerInterval": 15,
-    "globalPacingGroup": 0}
+    "globalPacingGroup": 0,
+    "txRepetition": 0}
 
 BRG_KEYS = ['txPeriodMs', 'rxTxPeriodMs', 'energyPattern', 'pacerInterval', 'txProbability', '2.4GhzOutputPower',
             'otaUpgradeEnabled', 'globalPacingEnabled', 'sub1GhzOutputPower', 'sub1GhzFrequency', 'globalPacingGroup',
             'txRepetition']
 GW_KEYS = ['gwDataSrc']
 GW_KEYS_THIN = ['dataCoupling', 'useStaticLocation', 'gwMgmtMode']
 GW_SHARED_KEYS = ['gw_2.4GhzOutputPower', 'gw_txPeriodMs', 'gw_pacerInterval', 'gw_energizingPattern',
```

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/firmware_update/firmware_update_cli.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/firmware_update/firmware_update_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/log_viewer/log_viewer_cli.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/log_viewer/log_viewer_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/configure_contextual_energizing.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,40 +153,14 @@
         on_duration_secs = on_duration * 30
         keep_alive_period_secs = keep_alive_period * 5
         keep_alive_scan_ms = keep_alive_scan * 10
         return sleep_duration_mins, on_duration_secs, keep_alive_period_secs, keep_alive_scan_ms, leds_on
 
 
 class BridgePowerManagementClient(ExtendedEdgeClient):
-        
-    def check_gw_compatible_for_pwr_mgmt(self, gateway_id):
-        """
-        checks if gateway is compatible to send and receive power management configurations
-        :type gateway_id: str
-        :param gateway_id: gateway ID
-        :rtype: bool
-        """
-        gateway_type = self.get_gateway_type(gateway_id)
-        if gateway_type != GatewayType.WIFI:
-            if gateway_type == GatewayType.MOBILE: 
-                return True
-            else:
-                return False
-        gw_dict = self.get_gateway(gateway_id)        
-        ble_ver = gw_dict["reportedConf"]["bleChipSwVersion"]
-        if gw_dict['online'] and \
-           self.check_ble_power_mgmt_support(ble_ver):
-            if gw_dict['reportedConf']['additional']['gwMgmtMode'] == 'transparent':
-                support = self.check_gw_ble_transparent_power_mgmt_support(ble_ver)
-                if not support:
-                    debug_print(f'Please update GW {gateway_id} or change to active mode for power management support!')
-                return support
-            return True
-        return False
-
 
     def get_bridge_relevant_gw(self, bridge_id):
         """
         Returns relevant GW for sending actions to bridge
         :param bridge_id: Bridge ID
         :rtype: str
         :return: relevant Gateway ID
@@ -198,15 +172,15 @@
         owner_gw_ids.extend(g['gatewayId'] for g in owner_gws)
         for gw in self.get_bridge(bridge_id)['connections']:
             if gw['gatewayId'] not in owner_gw_ids:
                 continue
             gw_id = gw['gatewayId']
             if gw['connected'] and \
                     bridge_id in self.get_seen_bridges(gw_id) and \
-                    self.check_gw_compatible_for_pwr_mgmt(gw_id):
+                    self.check_gw_compatible_for_action(gw_id):
                 if bridge_id in self.get_seen_bridges(gw['gatewayId']):
                             return gw['gatewayId']
         raise PowerManagementError(f'No relevant GW connected to bridge! Check deployment')
 
     def get_relevant_bridges(self, gateway_id):
         """
         Returns seen bridges by gateway that are associated to owner and have ble version with power management support
@@ -235,29 +209,14 @@
         ble_ver = ble_ver.split('.')
         if not ((int(ble_ver[0]) > 3) or
                 (int(ble_ver[0]) > 2 and int(ble_ver[1]) > 11) or \
                 (int(ble_ver[0]) > 2 and int(ble_ver[1]) > 10 and int(ble_ver[2]) > 39)):
             return False
         else:
             return True
-    
-    @staticmethod
-    def check_gw_ble_transparent_power_mgmt_support(ble_ver):
-        """
-        checks if power management is supported for transparent GW BLE version
-        :rtype: bool
-        :return: True if supported, False otherwise
-        """
-        ble_ver = ble_ver.split('.')
-        if not ((int(ble_ver[0]) > 3) or
-                (int(ble_ver[0]) > 2 and int(ble_ver[1]) > 14) or \
-                (int(ble_ver[0]) > 2 and int(ble_ver[1]) > 13 and int(ble_ver[2]) > 27)):
-            return False
-        else:
-            return True
 
 
     def send_pwr_mgmt_pkt(self, bridge_id, packet, gateway_id=None,
                           silent=False, seconds_to_send=1):
         """
         send power management packet to bridge
         :type bridge_id: str
@@ -318,15 +277,15 @@
         :type gateway_id: str
         :param gateway_id: Gateway ID
         :type silent: bool
         :param silent: print power management packet parameters
         :rtype: tuple
         :return: results (bool), bridges sent to (list)
         """
-        if not self.check_gw_compatible_for_pwr_mgmt(gateway_id):
+        if not self.check_gw_compatible_for_action(gateway_id):
             raise PowerManagementError(f'Gateway {gateway_id} not compatible with power management! '
                                        f'Try to update GW version')
         brgs_to_broadcast = self.get_relevant_bridges(gateway_id)
         if not silent:
             debug_print(f'Broadcasting Packet to bridges {brgs_to_broadcast}')
         res = self.send_pwr_mgmt_pkt(BROADCAST_DST_MAC, packet, gateway_id, silent, seconds_to_send)
         return res, brgs_to_broadcast
@@ -512,15 +471,15 @@
         if not ((bridge_id is not None and broadcast is False) or (bridge_id is None and broadcast is True)):
             raise PowerManagementError('Must specify bridgeId / set broadcast to True')
         if broadcast:
             if gateway_id is None:
                 raise PowerManagementError('Must specify GW ID to broadcast')
             return self.broadcast_packet_until_ack(gateway_id, packet, minutes_timeout)
         via_gw = self.get_bridge_relevant_gw(bridge_id) if gateway_id is None else gateway_id
-        if not self.check_gw_compatible_for_pwr_mgmt(via_gw):
+        if not self.check_gw_compatible_for_action(via_gw):
             raise PowerManagementError(f'GW {via_gw} Not compatible for power management!')
         return self.send_packet_until_ack(via_gw, bridge_id, packet, minutes_timeout)
 
     def exit_power_mgmt(self, gateway_id=None, update_gw=False, bridge_id=None, broadcast=False, minutes_timeout=3):
         """
         Exit power management mode (to normal bridge behavior).
         Function will search for the relevant gateway ID (if not specified) to send the configuration packet through.
@@ -540,15 +499,15 @@
         packet = PowerManagementPacket().exit_packet(silent=False)
         if not ((bridge_id is not None and broadcast is False) or (bridge_id is None and broadcast is True)):
             raise PowerManagementError('Must specify bridgeId / set broadcast to True')
         if broadcast:
             if gateway_id is None:
                 raise PowerManagementError('Must specify GW ID to broadcast')
         via_gw = self.get_bridge_relevant_gw(bridge_id) if gateway_id is None else gateway_id
-        if not self.check_gw_compatible_for_pwr_mgmt(via_gw):
+        if not self.check_gw_compatible_for_action(via_gw):
             raise PowerManagementError(f'GW {via_gw} Not compatible for power management!')
         gateway_type = self.get_gateway_type(via_gw)
         need_to_update = False
         if gateway_type == GatewayType.WIFI:
             gw_dict = self.get_gateway(via_gw)['reportedConf']['additional']
             for param in EXIT_POWER_MGMT_GW_DICT:
                 if gw_dict[param] != EXIT_POWER_MGMT_GW_DICT[param]:
@@ -580,7 +539,9 @@
         gw_type = self.get_gateway_type(gateway_id)
         assert gw_type == GatewayType.MOBILE, f'GW {gateway_id} not an android GW!'
         debug_print(f'Setting GW {gateway_id} uplink to {uplink_mode}')
         return self.send_action_to_gateway(gateway_id, payload[uplink_mode])
 
 class PowerManagementClient(BridgePowerManagementClient, AndroidPowerManagementClient):
     pass
+
+
```

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/power_mgmt/power_mgmt_cli.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools/utils/get_version.py` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/PKG-INFO` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-deployment-tools
-Version: 4.0.7
+Version: 4.0.8
 Summary: A library for interacting with Wiliot's Deployment Tools
 Home-page: 
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 
 # PyWiliot: wiliot-deployment-tools #
 
 wiliot-deployment-tools is a python library for accessing Wiliot's Deployment and Automation Tools.
 This python package includes the following CLI utilities:
  - Automatic Configuration Tool (`wlt-config`)
  - Power Management Tool (`wlt-power-mgmt`)
+ - Calibration Management Tool (`wlt-clibration-mgmt`)
  - Firmware Update Tool (`wlt-firmware`)
  - Log Viewer (`wlt-log`)
 
 
 ## Installing wiliot-deployment-tools
 ````commandline
 pip install wiliot-deployment-tools
@@ -62,14 +63,31 @@
 usage: wlt-firmware -owner OWNER [-beta] versions
 
 optional arguments:
   -beta              show available beta versions / update to beta firmware
 
 example usage: wlt-firmware -o wiliot versions
 ```
+### Calibration Management
+Configure Wiliot Bridge calibration mode
+```
+usage: wlt-calibration-mgmt -owner OwnerID -brg BridgeID -gw GW -mode CalibrationMode [-timeout TIMEOUT]
+
+required arguments:
+  -owner OWNER  Owner ID
+  -brg BRG      Bridge ID
+  -gw GW        GW ID to configure bridge
+  -mode Mode    CalibrationMode on of 3 options: 0-regular, 1-no ch37, 2-ch37 on data only
+
+optional arguments:
+
+  -timeout TIMEOUT      Minutes timeout (not required, defaults to 5 minutes)
+
+  example usage: wlt-calibration-mgmt -owner wiliot -brg 0123ABCD -gw AB1234CD -mode 1
+```
 
  #### Firmware Update
  Run OTA Process, first updating specified GWs to latest / specified FW version. Afterwards seuqentially update each specified Bridges / all Bridges to the same Firmware version.
  ```
 usage: wlt-firmware update -owner OWNER [-beta] [-version VERSION] [-gw GW [GW ...]] [-brg BRG [BRG ...]] [-all_brgs] [-ignore_bridges IGNORE_BRIDGES [IGNORE_BRIDGES ...]] [-action]
 
 optional arguments:
@@ -122,16 +140,17 @@
   -gw GW            GW ID to configure bridge (not required)
   -no_config        If used, GW will not change to optimal configuration
   -timeout TIMEOUT  Minutes timeout (not required, defaults to 5 minutes)
 
 example usage: wlt-power-mgmt -o wiliot exit -brg BridgeID
 ```
 
+
 ### Log Viewer
-View Wiliot Gatewa logs
+View Wiliot Gateway logs
 ```
 usage: wlt-log -owner OWNER -gw GW
 
 Log Viewer - CLI Tool to view Wiliot Gateway logs
 
 required arguments:
   -owner OWNER  Owner ID
@@ -141,14 +160,18 @@
 ------------------
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.8:
+* Support for python 3.11
+* Added new calibration mgmt tool
+
 Version 4.0.7:
 * Android power management support
 * Bugfix when no gateway logs found
   
 Version 4.0.4:
 * Bugfixes, add relevant printouts to CLI to help understand errors.
```

### Comparing `wiliot-deployment-tools-4.0.7/wiliot_deployment_tools.egg-info/SOURCES.txt` & `wiliot-deployment-tools-4.0.8/wiliot_deployment_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,21 @@
 wiliot_deployment_tools.egg-info/entry_points.txt
 wiliot_deployment_tools.egg-info/not-zip-safe
 wiliot_deployment_tools.egg-info/requires.txt
 wiliot_deployment_tools.egg-info/top_level.txt
 wiliot_deployment_tools/api/__init__.py
 wiliot_deployment_tools/api/extended_api.py
 wiliot_deployment_tools/api/gw_ssid.py
+wiliot_deployment_tools/api/s3_client.py
 wiliot_deployment_tools/automatic_configuration_tool/__init__.py
 wiliot_deployment_tools/automatic_configuration_tool/automatic_configuration_tool.py
 wiliot_deployment_tools/automatic_configuration_tool/configuration_tool_cli.py
+wiliot_deployment_tools/calibration_mgmt/__init__.py
+wiliot_deployment_tools/calibration_mgmt/calibration_mgmt.py
+wiliot_deployment_tools/calibration_mgmt/calibration_mgmt_cli.py
 wiliot_deployment_tools/common/__init__.py
 wiliot_deployment_tools/common/analysis_data_bricks.py
 wiliot_deployment_tools/common/debug.py
 wiliot_deployment_tools/common/utils.py
 wiliot_deployment_tools/common/utils_defines.py
 wiliot_deployment_tools/firmware_update/__init__.py
 wiliot_deployment_tools/firmware_update/firmware_update.py
```

