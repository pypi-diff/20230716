# Comparing `tmp/skypilot-nightly-1.0.0.dev20230714.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230715.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230714.tar", last modified: Fri Jul 14 10:42:07 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230715.tar", last modified: Sat Jul 15 10:40:53 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230714.tar` & `skypilot-nightly-1.0.0.dev20230715.tar`

### file list

```diff
@@ -1,223 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-14 10:41:58.000000 skypilot-nightly-1.0.0.dev20230714/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.718555 skypilot-nightly-1.0.0.dev20230714/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-14 10:41:58.000000 skypilot-nightly-1.0.0.dev20230714/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112593 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   201662 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.726555 skypilot-nightly-1.0.0.dev20230714/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41085 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25564 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    24158 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24297 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.726555 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    22995 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.726555 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41325 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    45043 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-14 10:41:58.000000 skypilot-nightly-1.0.0.dev20230714/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.714555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   123678 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-15 10:40:45.000000 skypilot-nightly-1.0.0.dev20230715/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-15 10:40:45.000000 skypilot-nightly-1.0.0.dev20230715/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112833 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200283 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.047319 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41057 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25706 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42681 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.051319 skypilot-nightly-1.0.0.dev20230715/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-15 10:40:45.000000 skypilot-nightly-1.0.0.dev20230715/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.043318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.055318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.059318 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.063319 skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 10:40:53.000000 skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:40:53.067319 skypilot-nightly-1.0.0.dev20230715/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123678 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 10:40:42.000000 skypilot-nightly-1.0.0.dev20230715/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/LICENSE` & `skypilot-nightly-1.0.0.dev20230715/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230715/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230715/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,12 @@
-Metadata-Version: 2.1
-Name: skypilot-nightly
-Version: 1.0.0.dev20230714
-Summary: SkyPilot: An intercloud broker for the clouds
-Author: SkyPilot Team
-License: Apache 2.0
-Project-URL: Homepage, https://github.com/skypilot-org/skypilot
-Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
-Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
-Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Distributed Computing
-Description-Content-Type: text/markdown
-Provides-Extra: aws
-Provides-Extra: azure
-Provides-Extra: gcp
-Provides-Extra: ibm
-Provides-Extra: docker
-Provides-Extra: lambda
-Provides-Extra: cloudflare
-Provides-Extra: scp
-Provides-Extra: oci
-Provides-Extra: all
-License-File: LICENSE
-
 <p align="center">
-  <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-light-1k.png" width=55%>
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-dark-1k.png">
+    <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-light-1k.png" width=55%>
+  </picture>
 </p>
 
 <p align="center">
   <a href="https://skypilot.readthedocs.io/en/latest/"> 
     <img alt="Documentation" src="https://readthedocs.org/projects/skypilot/badge/?version=latest">
   </a>
   
@@ -82,25 +54,28 @@
 Install with pip or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
 ```
 pip install "skypilot[aws,gcp,azure,ibm,oci,scp,lambda]"  # choose your clouds
 ```
 
 Current supported providers (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung, OCI, Cloudflare):
 <p align="center">
-  <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-light.png" width=80%>
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-dark.png">
+    <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-light.png" width=80%>
+  </picture>
 </p>
 
 
 ## Getting Started
 You can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
 - [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html)
 - [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html)
 - [CLI reference](https://skypilot.readthedocs.io/en/latest/reference/cli.html)
 
-## SkyPilot in 1 minute
+## SkyPilot in 1 Minute
 
 A SkyPilot task specifies: resource requirements, data to be synced, setup commands, and the task commands. 
 
 Once written in this [**unified interface**](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched on any available cloud.  This avoids vendor lock-in, and allows easily moving jobs to a different provider.
 
 Paste the following into a file `my_task.yaml`:
 
@@ -146,28 +121,39 @@
 <p align="center">
   <img src="https://i.imgur.com/TgamzZ2.gif" alt="SkyPilot Demo"/>
 </p>
 
 
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html) to get started with SkyPilot.
 
-## Learn more
+## More Information
+To learn more, see our [Documentation](https://skypilot.readthedocs.io/en/latest/) and [Tutorials](https://github.com/skypilot-org/skypilot-tutorial).
 
-- [Documentation](https://skypilot.readthedocs.io/en/latest/)
-- [Example: HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/tutorial.html) 
-- [Tutorials](https://github.com/skypilot-org/skypilot-tutorial) 
-- [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html)
-- Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml),  [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more](./examples).
-
-More information:
-- [SkyPilot Blog](https://blog.skypilot.co/)
-  - [Introductory blog post](https://blog.skypilot.co/introducing-skypilot/)
-- [NSDI 2023 paper & talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng)
+Runnable examples:
+- LLMs on SkyPilot
+  - [Vicuna chatbots: Training & Serving](./llm/vicuna/) (from official Vicuna team)
+  - [vLLM: Serving LLM 24x Faster On the Cloud](./llm/vllm/) (from official vLLM team)
+  - [QLoRA](https://github.com/artidoro/qlora/pull/132)
+  - [LLaMA-LoRA-Tuner](https://github.com/zetavg/LLaMA-LoRA-Tuner#run-on-a-cloud-service-via-skypilot)
+  - [Tabby: Self-hosted AI coding assistant](https://github.com/TabbyML/tabby/blob/bed723fcedb44a6b867ce22a7b1f03d2f3531c1e/experimental/eval/skypilot.yaml)
+  - [LocalGPT](./llm/localgpt)
+  - Add yours here & see more in [`llm/`](./llm)!
+- Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml), [DeepSpeed](./examples/deepspeed-multinode/sky.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more (`examples/`)](./examples).
+
+Follow updates:
+- [Twitter](https://twitter.com/skypilot_org)
+- [Slack](http://slack.skypilot.co)
+- [SkyPilot Blog](https://blog.skypilot.co/) ([Introductory blog post](https://blog.skypilot.co/introducing-skypilot/))
+
+Read the research:
+- [SkyPilot paper](https://www.usenix.org/system/files/nsdi23-yang-zongheng.pdf) and [talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng) (NSDI 2023)
+- [Sky Computing whitepaper](https://arxiv.org/abs/2205.07147)
+- [Sky Computing vision paper](https://sigops.org/s/conferences/hotos/2021/papers/hotos21-s02-stoica.pdf) (HotOS 2021)
 
-## Issues, feature requests, and questions
+## Support and Questions
 We are excited to hear your feedback! 
 * For issues and feature requests, please [open a GitHub issue](https://github.com/skypilot-org/skypilot/issues/new).
 * For questions, please use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
 
 For general discussions, join us on the [SkyPilot Slack](http://slack.skypilot.co).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230714
-Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
-License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
-skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
-Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
-Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: Topic :: System :: Distributed Computing Description-
-Content-Type: text/markdown Provides-Extra: aws Provides-Extra: azure Provides-
-Extra: gcp Provides-Extra: ibm Provides-Extra: docker Provides-Extra: lambda
-Provides-Extra: cloudflare Provides-Extra: scp Provides-Extra: oci Provides-
-Extra: all License-File: LICENSE
-                                  [SkyPilot]
+                                   [SkyPilot]
                  [Documentation] [GitHub_Release] [Join_Slack]
                     **** Run LLMs and AI on Any Cloud ****
 ---- :fire: *News* :fire: - [June, 2023] Serving LLM **24x Faster On the
 Cloud** with vLLM and SkyPilot: [**example**](./llm/vllm/), [**blog post**]
 (https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-
 skypilot/) - [June, 2023] [**Two new clouds supported**](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html): Samsung
@@ -42,21 +26,21 @@
 skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup
 of idle clusters SkyPilot supports your existing GPU, TPU, and CPU workloads,
 with no code changes. Install with pip or [from source](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html): ``` pip
 install "skypilot[aws,gcp,azure,ibm,oci,scp,lambda]" # choose your clouds ```
 Current supported providers (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung, OCI,
 Cloudflare):
-                                  [SkyPilot]
+                                   [SkyPilot]
 ## Getting Started You can find our documentation [here](https://
 skypilot.readthedocs.io/en/latest/). - [Installation](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
 [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
 quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
-reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
+reference/cli.html) ## SkyPilot in 1 Minute A SkyPilot task specifies: resource
 requirements, data to be synced, setup commands, and the task commands. Once
 written in this [**unified interface**](https://skypilot.readthedocs.io/en/
 latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
 on any available cloud. This avoids vendor lock-in, and allows easily moving
 jobs to a different provider. Paste the following into a file `my_task.yaml`:
 ```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
 Number of VMs to launch # Working directory (optional) containing the project
@@ -72,35 +56,47 @@
 lifting for you, including: 1. Find the lowest priced VM instance type across
 different clouds 2. Provision the VM, with auto-failover if the cloud returned
 capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
 commands to prepare the VM for running the task 5. Run the task's `run`
 commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
-started/quickstart.html) to get started with SkyPilot. ## Learn more -
-[Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
-HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
-tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
-- [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
-spec.html) - Framework examples: [PyTorch DDP](https://github.com/skypilot-org/
-skypilot/blob/master/examples/resnet_distributed_torch.yaml), [Distributed]
-(https://github.com/skypilot-org/skypilot/blob/master/examples/
-resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/
-skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU]
-(https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/
-tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/
-tree/master/examples/stable_diffusion), [Detectron2](https://github.com/
-skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml),
-[programmatic grid search](https://github.com/skypilot-org/skypilot/blob/
-master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://
-github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml),
-and [many more](./examples). More information: - [SkyPilot Blog](https://
-blog.skypilot.co/) - [Introductory blog post](https://blog.skypilot.co/
-introducing-skypilot/) - [NSDI 2023 paper & talk](https://www.usenix.org/
-conference/nsdi23/presentation/yang-zongheng) ## Issues, feature requests, and
-questions We are excited to hear your feedback! * For issues and feature
-requests, please [open a GitHub issue](https://github.com/skypilot-org/
-skypilot/issues/new). * For questions, please use [GitHub Discussions](https://
-github.com/skypilot-org/skypilot/discussions). For general discussions, join us
-on the [SkyPilot Slack](http://slack.skypilot.co). ## Contributing We welcome
-and value all contributions to the project! Please refer to [CONTRIBUTING]
-(CONTRIBUTING.md) for how to get involved.
+started/quickstart.html) to get started with SkyPilot. ## More Information To
+learn more, see our [Documentation](https://skypilot.readthedocs.io/en/latest/
+) and [Tutorials](https://github.com/skypilot-org/skypilot-tutorial). Runnable
+examples: - LLMs on SkyPilot - [Vicuna chatbots: Training & Serving](./llm/
+vicuna/) (from official Vicuna team) - [vLLM: Serving LLM 24x Faster On the
+Cloud](./llm/vllm/) (from official vLLM team) - [QLoRA](https://github.com/
+artidoro/qlora/pull/132) - [LLaMA-LoRA-Tuner](https://github.com/zetavg/LLaMA-
+LoRA-Tuner#run-on-a-cloud-service-via-skypilot) - [Tabby: Self-hosted AI coding
+assistant](https://github.com/TabbyML/tabby/blob/
+bed723fcedb44a6b867ce22a7b1f03d2f3531c1e/experimental/eval/skypilot.yaml) -
+[LocalGPT](./llm/localgpt) - Add yours here & see more in [`llm/`](./llm)! -
+Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/
+blob/master/examples/resnet_distributed_torch.yaml), [DeepSpeed](./examples/
+deepspeed-multinode/sky.yaml), [JAX/Flax on TPU](https://github.com/skypilot-
+org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion]
+(https://github.com/skypilot-org/skypilot/tree/master/examples/
+stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/
+master/examples/detectron2_docker.yaml), [Distributed](https://github.com/
+skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py)
+[TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/
+resnet_app_storage.yaml), [programmatic grid search](https://github.com/
+skypilot-org/skypilot/blob/master/examples/
+huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/
+skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many
+more (`examples/`)](./examples). Follow updates: - [Twitter](https://
+twitter.com/skypilot_org) - [Slack](http://slack.skypilot.co) - [SkyPilot Blog]
+(https://blog.skypilot.co/) ([Introductory blog post](https://blog.skypilot.co/
+introducing-skypilot/)) Read the research: - [SkyPilot paper](https://
+www.usenix.org/system/files/nsdi23-yang-zongheng.pdf) and [talk](https://
+www.usenix.org/conference/nsdi23/presentation/yang-zongheng) (NSDI 2023) - [Sky
+Computing whitepaper](https://arxiv.org/abs/2205.07147) - [Sky Computing vision
+paper](https://sigops.org/s/conferences/hotos/2021/papers/hotos21-s02-
+stoica.pdf) (HotOS 2021) ## Support and Questions We are excited to hear your
+feedback! * For issues and feature requests, please [open a GitHub issue]
+(https://github.com/skypilot-org/skypilot/issues/new). * For questions, please
+use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
+For general discussions, join us on the [SkyPilot Slack](http://
+slack.skypilot.co). ## Contributing We welcome and value all contributions to
+the project! Please refer to [CONTRIBUTING](CONTRIBUTING.md) for how to get
+involved.
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/README.md` & `skypilot-nightly-1.0.0.dev20230715/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,40 @@
+Metadata-Version: 2.1
+Name: skypilot-nightly
+Version: 1.0.0.dev20230715
+Summary: SkyPilot: An intercloud broker for the clouds
+Author: SkyPilot Team
+License: Apache 2.0
+Project-URL: Homepage, https://github.com/skypilot-org/skypilot
+Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
+Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
+Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Distributed Computing
+Description-Content-Type: text/markdown
+Provides-Extra: aws
+Provides-Extra: azure
+Provides-Extra: gcp
+Provides-Extra: ibm
+Provides-Extra: docker
+Provides-Extra: lambda
+Provides-Extra: cloudflare
+Provides-Extra: scp
+Provides-Extra: oci
+Provides-Extra: all
+License-File: LICENSE
+
 <p align="center">
-  <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-dark-1k.png">
-    <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-light-1k.png" width=55%>
-  </picture>
+  <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/skypilot-wide-light-1k.png" width=55%>
 </p>
 
 <p align="center">
   <a href="https://skypilot.readthedocs.io/en/latest/"> 
     <img alt="Documentation" src="https://readthedocs.org/projects/skypilot/badge/?version=latest">
   </a>
   
@@ -54,28 +82,25 @@
 Install with pip or [from source](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html):
 ```
 pip install "skypilot[aws,gcp,azure,ibm,oci,scp,lambda]"  # choose your clouds
 ```
 
 Current supported providers (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung, OCI, Cloudflare):
 <p align="center">
-  <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-dark.png">
-    <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-light.png" width=80%>
-  </picture>
+  <img alt="SkyPilot" src="https://raw.githubusercontent.com/skypilot-org/skypilot/master/docs/source/images/cloud-logos-light.png" width=80%>
 </p>
 
 
 ## Getting Started
 You can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
 - [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html)
 - [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html)
 - [CLI reference](https://skypilot.readthedocs.io/en/latest/reference/cli.html)
 
-## SkyPilot in 1 minute
+## SkyPilot in 1 Minute
 
 A SkyPilot task specifies: resource requirements, data to be synced, setup commands, and the task commands. 
 
 Once written in this [**unified interface**](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched on any available cloud.  This avoids vendor lock-in, and allows easily moving jobs to a different provider.
 
 Paste the following into a file `my_task.yaml`:
 
@@ -121,28 +146,39 @@
 <p align="center">
   <img src="https://i.imgur.com/TgamzZ2.gif" alt="SkyPilot Demo"/>
 </p>
 
 
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html) to get started with SkyPilot.
 
-## Learn more
+## More Information
+To learn more, see our [Documentation](https://skypilot.readthedocs.io/en/latest/) and [Tutorials](https://github.com/skypilot-org/skypilot-tutorial).
 
-- [Documentation](https://skypilot.readthedocs.io/en/latest/)
-- [Example: HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/tutorial.html) 
-- [Tutorials](https://github.com/skypilot-org/skypilot-tutorial) 
-- [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html)
-- Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml),  [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more](./examples).
-
-More information:
-- [SkyPilot Blog](https://blog.skypilot.co/)
-  - [Introductory blog post](https://blog.skypilot.co/introducing-skypilot/)
-- [NSDI 2023 paper & talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng)
+Runnable examples:
+- LLMs on SkyPilot
+  - [Vicuna chatbots: Training & Serving](./llm/vicuna/) (from official Vicuna team)
+  - [vLLM: Serving LLM 24x Faster On the Cloud](./llm/vllm/) (from official vLLM team)
+  - [QLoRA](https://github.com/artidoro/qlora/pull/132)
+  - [LLaMA-LoRA-Tuner](https://github.com/zetavg/LLaMA-LoRA-Tuner#run-on-a-cloud-service-via-skypilot)
+  - [Tabby: Self-hosted AI coding assistant](https://github.com/TabbyML/tabby/blob/bed723fcedb44a6b867ce22a7b1f03d2f3531c1e/experimental/eval/skypilot.yaml)
+  - [LocalGPT](./llm/localgpt)
+  - Add yours here & see more in [`llm/`](./llm)!
+- Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml), [DeepSpeed](./examples/deepspeed-multinode/sky.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more (`examples/`)](./examples).
+
+Follow updates:
+- [Twitter](https://twitter.com/skypilot_org)
+- [Slack](http://slack.skypilot.co)
+- [SkyPilot Blog](https://blog.skypilot.co/) ([Introductory blog post](https://blog.skypilot.co/introducing-skypilot/))
+
+Read the research:
+- [SkyPilot paper](https://www.usenix.org/system/files/nsdi23-yang-zongheng.pdf) and [talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng) (NSDI 2023)
+- [Sky Computing whitepaper](https://arxiv.org/abs/2205.07147)
+- [Sky Computing vision paper](https://sigops.org/s/conferences/hotos/2021/papers/hotos21-s02-stoica.pdf) (HotOS 2021)
 
-## Issues, feature requests, and questions
+## Support and Questions
 We are excited to hear your feedback! 
 * For issues and feature requests, please [open a GitHub issue](https://github.com/skypilot-org/skypilot/issues/new).
 * For questions, please use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
 
 For general discussions, join us on the [SkyPilot Slack](http://slack.skypilot.co).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,24 @@
-                                   [SkyPilot]
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230715
+Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
+License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
+skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
+Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
+Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Operating System :: OS
+Independent Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Classifier: Topic :: System :: Distributed Computing Description-
+Content-Type: text/markdown Provides-Extra: aws Provides-Extra: azure Provides-
+Extra: gcp Provides-Extra: ibm Provides-Extra: docker Provides-Extra: lambda
+Provides-Extra: cloudflare Provides-Extra: scp Provides-Extra: oci Provides-
+Extra: all License-File: LICENSE
+                                  [SkyPilot]
                  [Documentation] [GitHub_Release] [Join_Slack]
                     **** Run LLMs and AI on Any Cloud ****
 ---- :fire: *News* :fire: - [June, 2023] Serving LLM **24x Faster On the
 Cloud** with vLLM and SkyPilot: [**example**](./llm/vllm/), [**blog post**]
 (https://blog.skypilot.co/serving-llm-24x-faster-on-the-cloud-with-vllm-and-
 skypilot/) - [June, 2023] [**Two new clouds supported**](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html): Samsung
@@ -26,21 +42,21 @@
 skypilot.readthedocs.io/en/latest/reference/auto-stop.html): hands-free cleanup
 of idle clusters SkyPilot supports your existing GPU, TPU, and CPU workloads,
 with no code changes. Install with pip or [from source](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html): ``` pip
 install "skypilot[aws,gcp,azure,ibm,oci,scp,lambda]" # choose your clouds ```
 Current supported providers (AWS, Azure, GCP, Lambda Cloud, IBM, Samsung, OCI,
 Cloudflare):
-                                   [SkyPilot]
+                                  [SkyPilot]
 ## Getting Started You can find our documentation [here](https://
 skypilot.readthedocs.io/en/latest/). - [Installation](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
 [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
 quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
-reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
+reference/cli.html) ## SkyPilot in 1 Minute A SkyPilot task specifies: resource
 requirements, data to be synced, setup commands, and the task commands. Once
 written in this [**unified interface**](https://skypilot.readthedocs.io/en/
 latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
 on any available cloud. This avoids vendor lock-in, and allows easily moving
 jobs to a different provider. Paste the following into a file `my_task.yaml`:
 ```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
 Number of VMs to launch # Working directory (optional) containing the project
@@ -56,35 +72,47 @@
 lifting for you, including: 1. Find the lowest priced VM instance type across
 different clouds 2. Provision the VM, with auto-failover if the cloud returned
 capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
 commands to prepare the VM for running the task 5. Run the task's `run`
 commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
-started/quickstart.html) to get started with SkyPilot. ## Learn more -
-[Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
-HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
-tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
-- [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
-spec.html) - Framework examples: [PyTorch DDP](https://github.com/skypilot-org/
-skypilot/blob/master/examples/resnet_distributed_torch.yaml), [Distributed]
-(https://github.com/skypilot-org/skypilot/blob/master/examples/
-resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/
-skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU]
-(https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/
-tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/
-tree/master/examples/stable_diffusion), [Detectron2](https://github.com/
-skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml),
-[programmatic grid search](https://github.com/skypilot-org/skypilot/blob/
-master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://
-github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml),
-and [many more](./examples). More information: - [SkyPilot Blog](https://
-blog.skypilot.co/) - [Introductory blog post](https://blog.skypilot.co/
-introducing-skypilot/) - [NSDI 2023 paper & talk](https://www.usenix.org/
-conference/nsdi23/presentation/yang-zongheng) ## Issues, feature requests, and
-questions We are excited to hear your feedback! * For issues and feature
-requests, please [open a GitHub issue](https://github.com/skypilot-org/
-skypilot/issues/new). * For questions, please use [GitHub Discussions](https://
-github.com/skypilot-org/skypilot/discussions). For general discussions, join us
-on the [SkyPilot Slack](http://slack.skypilot.co). ## Contributing We welcome
-and value all contributions to the project! Please refer to [CONTRIBUTING]
-(CONTRIBUTING.md) for how to get involved.
+started/quickstart.html) to get started with SkyPilot. ## More Information To
+learn more, see our [Documentation](https://skypilot.readthedocs.io/en/latest/
+) and [Tutorials](https://github.com/skypilot-org/skypilot-tutorial). Runnable
+examples: - LLMs on SkyPilot - [Vicuna chatbots: Training & Serving](./llm/
+vicuna/) (from official Vicuna team) - [vLLM: Serving LLM 24x Faster On the
+Cloud](./llm/vllm/) (from official vLLM team) - [QLoRA](https://github.com/
+artidoro/qlora/pull/132) - [LLaMA-LoRA-Tuner](https://github.com/zetavg/LLaMA-
+LoRA-Tuner#run-on-a-cloud-service-via-skypilot) - [Tabby: Self-hosted AI coding
+assistant](https://github.com/TabbyML/tabby/blob/
+bed723fcedb44a6b867ce22a7b1f03d2f3531c1e/experimental/eval/skypilot.yaml) -
+[LocalGPT](./llm/localgpt) - Add yours here & see more in [`llm/`](./llm)! -
+Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/
+blob/master/examples/resnet_distributed_torch.yaml), [DeepSpeed](./examples/
+deepspeed-multinode/sky.yaml), [JAX/Flax on TPU](https://github.com/skypilot-
+org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion]
+(https://github.com/skypilot-org/skypilot/tree/master/examples/
+stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/
+master/examples/detectron2_docker.yaml), [Distributed](https://github.com/
+skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py)
+[TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/
+resnet_app_storage.yaml), [programmatic grid search](https://github.com/
+skypilot-org/skypilot/blob/master/examples/
+huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/
+skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many
+more (`examples/`)](./examples). Follow updates: - [Twitter](https://
+twitter.com/skypilot_org) - [Slack](http://slack.skypilot.co) - [SkyPilot Blog]
+(https://blog.skypilot.co/) ([Introductory blog post](https://blog.skypilot.co/
+introducing-skypilot/)) Read the research: - [SkyPilot paper](https://
+www.usenix.org/system/files/nsdi23-yang-zongheng.pdf) and [talk](https://
+www.usenix.org/conference/nsdi23/presentation/yang-zongheng) (NSDI 2023) - [Sky
+Computing whitepaper](https://arxiv.org/abs/2205.07147) - [Sky Computing vision
+paper](https://sigops.org/s/conferences/hotos/2021/papers/hotos21-s02-
+stoica.pdf) (HotOS 2021) ## Support and Questions We are excited to hear your
+feedback! * For issues and feature requests, please [open a GitHub issue]
+(https://github.com/skypilot-org/skypilot/issues/new). * For questions, please
+use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
+For general discussions, join us on the [SkyPilot Slack](http://
+slack.skypilot.co). ## Contributing We welcome and value all contributions to
+the project! Please refer to [CONTRIBUTING](CONTRIBUTING.md) for how to get
+involved.
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230715/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/setup.py` & `skypilot-nightly-1.0.0.dev20230715/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230715/sky/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = 'f35f65d802f575c7e12b7573196b66ac1ced3a38'
-__version__ = '1.0.0-dev20230714'
+__commit__ = 'e924e44a4a2a0bf8dae2953f3cf3c05e4bdb5f76'
+__version__ = '1.0.0-dev20230715'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """GCP cloud adaptors"""
 
 # pylint: disable=import-outside-toplevel
-from functools import wraps
+import functools
 
 googleapiclient = None
 google = None
 
 
 def import_package(func):
 
-    @wraps(func)
+    @functools.wraps(func)
     def wrapper(*args, **kwargs):
         global googleapiclient, google
         if googleapiclient is None or google is None:
             try:
                 import googleapiclient as _googleapiclient
                 import google as _google
                 googleapiclient = _googleapiclient
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230715/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230715/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,23 @@
         return self._setup(handle, task, detach_setup)
 
     def add_storage_objects(self, task: 'task_lib.Task') -> None:
         raise NotImplementedError
 
     @timeline.event
     @usage_lib.messages.usage.update_runtime('execute')
-    def execute(self, handle: _ResourceHandleType, task: 'task_lib.Task',
-                detach_run: bool) -> None:
+    def execute(self,
+                handle: _ResourceHandleType,
+                task: 'task_lib.Task',
+                detach_run: bool,
+                dryrun: bool = False) -> None:
         usage_lib.record_cluster_name_for_current_operation(
             handle.get_cluster_name())
         usage_lib.messages.usage.update_actual_task(task)
-        return self._execute(handle, task, detach_run)
+        return self._execute(handle, task, detach_run, dryrun)
 
     @timeline.event
     def post_execute(self, handle: _ResourceHandleType, down: bool) -> None:
         """Post execute(): e.g., print helpful inspection messages."""
         return self._post_execute(handle, down)
 
     @timeline.event
@@ -132,16 +135,19 @@
     ) -> None:
         raise NotImplementedError
 
     def _setup(self, handle: _ResourceHandleType, task: 'task_lib.Task',
                detach_setup: bool) -> None:
         raise NotImplementedError
 
-    def _execute(self, handle: _ResourceHandleType, task: 'task_lib.Task',
-                 detach_run: bool) -> None:
+    def _execute(self,
+                 handle: _ResourceHandleType,
+                 task: 'task_lib.Task',
+                 detach_run: bool,
+                 dryrun: bool = False) -> None:
         raise NotImplementedError
 
     def _post_execute(self, handle: _ResourceHandleType, down: bool) -> None:
         raise NotImplementedError
 
     def _teardown_ephemeral_storage(self, task: 'task_lib.Task') -> None:
         raise NotImplementedError
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/backend_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2132,46 +2132,53 @@
 
 @typing.overload
 def check_cluster_available(
     cluster_name: str,
     *,
     operation: str,
     check_cloud_vm_ray_backend: Literal[True] = True,
+    dryrun: bool = ...,
 ) -> 'cloud_vm_ray_backend.CloudVmRayResourceHandle':
     ...
 
 
 @typing.overload
 def check_cluster_available(
     cluster_name: str,
     *,
     operation: str,
     check_cloud_vm_ray_backend: Literal[False],
+    dryrun: bool = ...,
 ) -> backends.ResourceHandle:
     ...
 
 
 def check_cluster_available(
     cluster_name: str,
     *,
     operation: str,
     check_cloud_vm_ray_backend: bool = True,
+    dryrun: bool = False,
 ) -> backends.ResourceHandle:
     """Check if the cluster is available.
 
     Raises:
         ValueError: if the cluster does not exist.
         exceptions.ClusterNotUpError: if the cluster is not UP.
         exceptions.NotSupportedError: if the cluster is not based on
           CloudVmRayBackend.
         exceptions.ClusterOwnerIdentityMismatchError: if the current user is
           not the same as the user who created the cluster.
         exceptions.CloudUserIdentityError: if we fail to get the current user
           identity.
     """
+    if dryrun:
+        record = global_user_state.get_cluster_from_name(cluster_name)
+        assert record is not None, cluster_name
+        return record['handle']
     try:
         cluster_status, handle = refresh_cluster_status_handle(cluster_name)
     except exceptions.ClusterStatusFetchingError as e:
         # Failed to refresh the cluster status is not fatal error as the callers
         # can still be done by only using ssh, but the ssh can hang if the
         # cluster is not up (e.g., autostopped).
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/cloud_vm_ray_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 _PATH_SIZE_MEGABYTES_WARN_THRESHOLD = 256
 
 # Timeout (seconds) for provision progress: if in this duration no new nodes
 # are launched, abort and failover.
 _NODES_LAUNCHING_PROGRESS_TIMEOUT = {
     clouds.AWS: 90,
     clouds.Azure: 90,
-    clouds.GCP: 120,
+    clouds.GCP: 240,
     clouds.Lambda: 150,
     clouds.IBM: 160,
     clouds.Local: 90,
     clouds.OCI: 300,
 }
 
 # Time gap between retries after failing to provision in all possible places.
@@ -1436,15 +1436,15 @@
                     keep_launch_fields_in_existing_config=cluster_exists)
             except exceptions.ResourcesUnavailableError as e:
                 # Failed due to catalog issue, e.g. image not found.
                 logger.info(
                     f'Failed to find catalog in region {region.name}: {e}')
                 continue
             if dryrun:
-                return
+                return config_dict
             cluster_config_file = config_dict['ray']
 
             # Record early, so if anything goes wrong, 'sky status' will show
             # the cluster name and users can appropriately 'sky down'.  It also
             # means a second 'sky launch -c <name>' will attempt to reuse.
             handle = CloudVmRayResourceHandle(
                 cluster_name=cluster_name,
@@ -2410,18 +2410,17 @@
             backend_utils.CLUSTER_STATUS_LOCK_PATH.format(cluster_name))
         with timeline.FileLockEvent(lock_path):
             to_provision_config = RetryingVmProvisioner.ToProvisionConfig(
                 cluster_name,
                 to_provision,
                 task.num_nodes,
                 prev_cluster_status=None)
-            if not dryrun:  # dry run doesn't need to check existing cluster.
-                # Try to launch the exiting cluster first
-                to_provision_config = self._check_existing_cluster(
-                    task, to_provision, cluster_name)
+            # Try to launch the exiting cluster first
+            to_provision_config = self._check_existing_cluster(
+                task, to_provision, cluster_name, dryrun)
             assert to_provision_config.resources is not None, (
                 'to_provision should not be None', to_provision_config)
 
             prev_cluster_status = to_provision_config.prev_cluster_status
             usage_lib.messages.usage.update_cluster_resources(
                 to_provision_config.num_nodes, to_provision_config.resources)
             usage_lib.messages.usage.update_cluster_status(prev_cluster_status)
@@ -2491,15 +2490,16 @@
                         '\nTo keep retrying until the cluster is up, use the '
                         '`--retry-until-up` flag.')
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.ResourcesUnavailableError(
                             error_message,
                             failover_history=e.failover_history) from None
             if dryrun:
-                return None
+                record = global_user_state.get_cluster_from_name(cluster_name)
+                return record['handle'] if record is not None else None
             cluster_config_file = config_dict['ray']
 
             handle = CloudVmRayResourceHandle(
                 cluster_name=cluster_name,
                 cluster_yaml=cluster_config_file,
                 launched_nodes=config_dict['launched_nodes'],
                 launched_resources=config_dict['launched_resources'],
@@ -3004,23 +3004,29 @@
         return job_id
 
     def _execute(
         self,
         handle: CloudVmRayResourceHandle,
         task: task_lib.Task,
         detach_run: bool,
+        dryrun: bool = False,
     ) -> None:
         if task.run is None:
             logger.info('Run commands not specified or empty.')
             return
         # Check the task resources vs the cluster resources. Since `sky exec`
         # will not run the provision and _check_existing_cluster
         self.check_resources_fit_cluster(handle, task)
 
         resources_str = backend_utils.get_task_resources_str(task)
+
+        if dryrun:
+            logger.info(f'Dryrun complete. Would have run:\n{task}')
+            return
+
         job_id = self._add_job(handle, task.name, resources_str)
 
         is_tpu_vm_pod = tpu_utils.is_tpu_vm_pod(handle.launched_resources)
         # Case: task_lib.Task(run, num_nodes=N) or TPU VM Pods
         if task.num_nodes > 1 or is_tpu_vm_pod:
             self._execute_task_n_nodes(handle, task, job_id, detach_run)
         else:
@@ -3340,24 +3346,22 @@
             return
         log_path = os.path.join(os.path.expanduser(self.log_dir),
                                 'teardown.log')
         log_abs_path = os.path.abspath(log_path)
         cloud = handle.launched_resources.cloud
         config = common_utils.read_yaml(handle.cluster_yaml)
         cluster_name = handle.cluster_name
-        use_tpu_vm = config['provider'].get('_has_tpus', False)
 
         # Avoid possibly unbound warnings. Code below must overwrite these vars:
         returncode = 0
         stdout = ''
         stderr = ''
 
         # Use the new provisioner for AWS.
-        if isinstance(cloud, clouds.AWS):
-            region = config['provider']['region']
+        if isinstance(cloud, (clouds.AWS, clouds.GCP)):
             # Stop the ray autoscaler first to avoid the head node trying to
             # re-launch the worker nodes, during the termination of the
             # cluster.
             try:
                 # We do not check the return code, since Ray returns
                 # non-zero return code when calling Ray stop,
                 # even when the command was executed successfully.
@@ -3369,19 +3373,23 @@
                 if prev_cluster_status == status_lib.ClusterStatus.UP:
                     logger.warning(
                         'Failed to take down Ray autoscaler on the head node. '
                         'It might be because the cluster\'s head node has '
                         'already been terminated. It is fine to skip this.')
             try:
                 if terminate:
-                    provision_api.terminate_instances(repr(cloud), region,
-                                                      cluster_name)
+                    provision_api.terminate_instances(
+                        repr(cloud),
+                        cluster_name,
+                        provider_config=config['provider'])
                 else:
-                    provision_api.stop_instances(repr(cloud), region,
-                                                 cluster_name)
+                    provision_api.stop_instances(
+                        repr(cloud),
+                        cluster_name,
+                        provider_config=config['provider'])
             except Exception as e:  # pylint: disable=broad-except
                 if purge:
                     logger.warning(
                         _TEARDOWN_PURGE_WARNING.format(
                             reason='stopping/terminating cluster nodes',
                             details=common_utils.format_exception(
                                 e, use_bracket=True)))
@@ -3475,47 +3483,14 @@
 
             # 0: All terminated successfully, failed count otherwise
             returncode = oci_query_helper.terminate_instances_by_tags(
                 {TAG_RAY_CLUSTER_NAME: cluster_name}, region)
 
             # To avoid undefined local variables error.
             stdout = stderr = ''
-        elif (terminate and
-              (prev_cluster_status == status_lib.ClusterStatus.STOPPED or
-               use_tpu_vm)):
-            # For TPU VMs, gcloud CLI is used for VM termination.
-            if isinstance(cloud, clouds.GCP):
-                zone = config['provider']['availability_zone']
-                # TODO(wei-lin): refactor by calling functions of node provider
-                # that uses Python API rather than CLI
-                if use_tpu_vm:
-                    terminate_cmd = tpu_utils.terminate_tpu_vm_cluster_cmd(
-                        cluster_name, zone, log_abs_path)
-                else:
-                    query_cmd = (f'gcloud compute instances list --filter='
-                                 f'"(labels.ray-cluster-name={cluster_name})" '
-                                 f'--zones={zone} --format=value\\(name\\)')
-                    # If there are no instances, exit with 0 rather than causing
-                    # the delete command to fail.
-                    terminate_cmd = (
-                        f'VMS=$({query_cmd}) && [ -n "$VMS" ] && '
-                        f'gcloud compute instances delete --zone={zone} --quiet'
-                        ' $VMS || echo "No instances to delete."')
-            else:
-                with ux_utils.print_exception_no_traceback():
-                    raise ValueError(f'Unsupported cloud {cloud} for stopped '
-                                     f'cluster {cluster_name!r}.')
-            with log_utils.safe_rich_status(f'[bold cyan]Terminating '
-                                            f'[green]{cluster_name}'):
-                returncode, stdout, stderr = log_lib.run_with_log(
-                    terminate_cmd,
-                    log_abs_path,
-                    shell=True,
-                    stream_logs=False,
-                    require_outputs=True)
         else:
             config['provider']['cache_stopped_nodes'] = not terminate
             with tempfile.NamedTemporaryFile('w',
                                              prefix='sky_',
                                              delete=False,
                                              suffix='.yml') as f:
                 common_utils.dump_yaml(f.name, config)
@@ -3763,48 +3738,55 @@
             **kwargs,
         )
 
     # --- Utilities ---
 
     @timeline.event
     def _check_existing_cluster(
-            self, task: task_lib.Task,
+            self,
+            task: task_lib.Task,
             to_provision: Optional[resources_lib.Resources],
-            cluster_name: str) -> RetryingVmProvisioner.ToProvisionConfig:
+            cluster_name: str,
+            dryrun: bool = False) -> RetryingVmProvisioner.ToProvisionConfig:
         """Checks if the cluster exists and returns the provision config.
 
         Raises:
             exceptions.ResourcesMismatchError: If the resources in the task
                 does not match the existing cluster.
             exceptions.InvalidClusterNameError: If the cluster name is invalid.
             # TODO(zhwu): complete the list of exceptions.
         """
         record = global_user_state.get_cluster_from_name(cluster_name)
         handle_before_refresh = None if record is None else record['handle']
         status_before_refresh = None if record is None else record['status']
 
-        prev_cluster_status, handle = (
-            backend_utils.refresh_cluster_status_handle(
-                cluster_name,
-                # We force refresh for the init status to determine the actual
-                # state of a previous cluster in INIT state.
-                #
-                # This is important for the case, where an existing cluster is
-                # transitioned into INIT state due to key interruption during
-                # launching, with the following steps:
-                # (1) launch, after answering prompt immediately ctrl-c;
-                # (2) launch again.
-                # If we don't refresh the state of the cluster and reset it back
-                # to STOPPED, our failover logic will consider it as an abnormal
-                # cluster after hitting resources capacity limit on the cloud,
-                # and will start failover. This is not desired, because the user
-                # may want to keep the data on the disk of that cluster.
-                force_refresh_statuses={status_lib.ClusterStatus.INIT},
-                acquire_per_cluster_status_lock=False,
-            ))
+        prev_cluster_status, handle = (status_before_refresh,
+                                       handle_before_refresh)
+
+        if not dryrun:
+            prev_cluster_status, handle = (
+                backend_utils.refresh_cluster_status_handle(
+                    cluster_name,
+                    # We force refresh for the init status to determine the
+                    # actual state of a previous cluster in INIT state.
+                    #
+                    # This is important for the case, where an existing cluster
+                    # is transitioned into INIT state due to key interruption
+                    # during launching, with the following steps:
+                    # (1) launch, after answering prompt immediately ctrl-c;
+                    # (2) launch again.
+                    # If we don't refresh the state of the cluster and reset it
+                    # back to STOPPED, our failover logic will consider it as an
+                    # abnormal cluster after hitting resources capacity limit on
+                    # the cloud, and will start failover. This is not desired,
+                    # because the user may want to keep the data on the disk of
+                    # that cluster.
+                    force_refresh_statuses={status_lib.ClusterStatus.INIT},
+                    acquire_per_cluster_status_lock=False,
+                ))
         if prev_cluster_status is not None:
             assert handle is not None
             # Cluster already exists.
             self.check_resources_fit_cluster(handle, task)
             # Use the existing cluster.
             assert handle.launched_resources is not None, (cluster_name, handle)
             return RetryingVmProvisioner.ToProvisionConfig(
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/local_docker_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,16 +261,19 @@
             f'{image_tag} /bin/bash{style.RESET_ALL}.\n')
         global_user_state.add_or_update_cluster(
             cluster_name,
             cluster_handle=handle,
             requested_resources=task.resources,
             ready=True)
 
-    def _execute(self, handle: LocalDockerResourceHandle, task: 'task_lib.Task',
-                 detach_run: bool) -> None:
+    def _execute(self,
+                 handle: LocalDockerResourceHandle,
+                 task: 'task_lib.Task',
+                 detach_run: bool,
+                 dryrun: bool = False) -> None:
         """ Launches the container."""
 
         if detach_run:
             raise NotImplementedError('detach_run=True is not supported in '
                                       'LocalDockerBackend.')
 
         if task.num_nodes > 1:
@@ -279,14 +282,18 @@
                 'LocalDockerBackend.')
 
         # Handle a basic task
         if task.run is None:
             logger.info(f'Nothing to run; run command not specified:\n{task}')
             return
 
+        if dryrun:
+            logger.info(f'Dryrun complete. Would have run:\n{task}')
+            return
+
         self._execute_task_one_node(handle, task)
 
     def _post_execute(self, handle: LocalDockerResourceHandle,
                       down: bool) -> None:
         del down  # unused
         style = colorama.Style
         container = self.containers[handle]
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/check.py` & `skypilot-nightly-1.0.0.dev20230715/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230715/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230715/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,16 +356,16 @@
             'use_spot': r.use_spot,
             'region': region_name,
             'zones': ','.join(zone_names),
             'image_id': image_id,
             **AWS._get_disk_specs(r.disk_tier)
         }
 
-    def get_feasible_launchable_resources(self,
-                                          resources: 'resources_lib.Resources'):
+    def _get_feasible_launchable_resources(
+            self, resources: 'resources_lib.Resources'):
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Treat Resources(AWS, p3.2x, V100) as Resources(AWS, p3.2x).
             resources = resources.copy(accelerators=None)
             return ([resources], [])
 
         def _make(instance_list):
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             'region': region_name,
             # Azure does not support specific zones.
             'zones': None,
             **image_config,
             'disk_tier': Azure._get_disk_type(r.disk_tier)
         }
 
-    def get_feasible_launchable_resources(self, resources):
+    def _get_feasible_launchable_resources(self, resources):
 
         def failover_disk_tier(
                 instance_type: str,
                 disk_tier: Optional[str]) -> Tuple[bool, Optional[str]]:
             """Figure out the actual disk tier to be used
 
             Check the disk_tier specified by the user with the instance type to
@@ -284,19 +284,23 @@
 
         if resources.use_spot:
             # TODO(zhwu): our azure subscription offer ID does not support spot.
             # Need to support it.
             return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
-            # Treat Resources(AWS, p3.2x, V100) as Resources(AWS, p3.2x).
+            ok, disk_tier = failover_disk_tier(resources.instance_type,
+                                               resources.disk_tier)
+            if not ok:
+                return ([], [])
+            # Treat Resources(Azure, Standard_NC4as_T4_v3, T4) as
+            # Resources(Azure, Standard_NC4as_T4_v3).
             resources = resources.copy(
                 accelerators=None,
-                disk_tier=failover_disk_tier(resources.instance_type,
-                                             resources.disk_tier),
+                disk_tier=disk_tier,
             )
             return ([resources], [])
 
         def _make(instance_list):
             resource_list = []
             for instance_type in instance_list:
                 ok, disk_tier = failover_disk_tier(instance_type,
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sky import exceptions
 from sky.clouds import service_catalog
 from sky.utils import log_utils
 from sky.utils import ux_utils
 
 if typing.TYPE_CHECKING:
     from sky import status_lib
-    from sky import resources
+    from sky import resources as resources_lib
 
 
 class CloudImplementationFeatures(enum.Enum):
     """Features that might not be implemented for all clouds.
 
     Used by Cloud.check_features_are_supported().
 
@@ -215,15 +215,15 @@
         raise NotImplementedError
 
     def is_same_cloud(self, other):
         raise NotImplementedError
 
     def make_deploy_resources_variables(
         self,
-        resources: 'resources.Resources',
+        resources: 'resources_lib.Resources',
         region: 'Region',
         zones: Optional[List['Zone']],
     ) -> Dict[str, Optional[str]]:
         """Converts planned sky.Resources to cloud-specific resource variables.
 
         These variables are used to fill the node type section (instance type,
         any accelerators, etc.) in the cloud's deployment YAML template.
@@ -290,14 +290,19 @@
 
         Feasible resources refer to an offering respecting the resource
         requirements.  Currently, this function implements "filtering" the
         cloud's offerings only w.r.t. accelerators constraints.
 
         Launchable resources require a cloud and an instance type be assigned.
         """
+        if resources.is_launchable():
+            self._check_instance_type_accelerators_combination(resources)
+        return self._get_feasible_launchable_resources(resources)
+
+    def _get_feasible_launchable_resources(self, resources):
         raise NotImplementedError
 
     @classmethod
     def check_credentials(cls) -> Tuple[bool, Optional[str]]:
         """Checks if the user has access credentials to this cloud.
 
         Returns a boolean of whether the user can access this cloud, and a
@@ -391,16 +396,16 @@
                                       accelerator: str,
                                       acc_count: int,
                                       region: Optional[str] = None,
                                       zone: Optional[str] = None) -> bool:
         """Returns whether the accelerator is valid in the region or zone."""
         raise NotImplementedError
 
-    def need_cleanup_after_preemption(self,
-                                      resource: 'resources.Resources') -> bool:
+    def need_cleanup_after_preemption(
+            self, resource: 'resources_lib.Resources') -> bool:
         """Returns whether a spot resource needs cleanup after preeemption.
 
         In most cases, spot resources do not need cleanup after preemption,
         as long as the cluster can be relaunched with the same name and tag,
         no matter the preemption behavior is to terminate or stop the cluster.
         The only exception by far is GCP's Spot TPU VM. We override this method
         in gcp.py.
@@ -474,15 +479,62 @@
 
         Raises:
             exceptions.NotSupportedError: If the disk tier is not supported.
         """
         raise NotImplementedError
 
     @classmethod
-    # pylint: disable=unused-argument
+    def _check_instance_type_accelerators_combination(
+            cls, resources: 'resources_lib.Resources') -> None:
+        """Errors out if the accelerator is not supported by the instance type.
+
+        This function is overridden by GCP for host-accelerator logic.
+
+        Raises:
+            ResourcesMismatchError: If the accelerator is not supported.
+        """
+        assert resources.is_launchable(), resources
+
+        def _equal_accelerators(
+                acc_requested: Optional[Dict[str, int]],
+                acc_from_instance_type: Optional[Dict[str, int]]) -> bool:
+            """Check the requested accelerators equals to the instance type
+
+            Check the requested accelerators equals to the accelerators
+            from the instance type (both the accelerator type and the
+            count).
+            """
+            if acc_requested is None:
+                return acc_from_instance_type is None
+            if acc_from_instance_type is None:
+                return False
+
+            for acc in acc_requested:
+                if acc not in acc_from_instance_type:
+                    return False
+                if acc_requested[acc] != acc_from_instance_type[acc]:
+                    return False
+            return True
+
+        acc_from_instance_type = (cls.get_accelerators_from_instance_type(
+            resources.instance_type))
+        if not _equal_accelerators(resources.accelerators,
+                                   acc_from_instance_type):
+            with ux_utils.print_exception_no_traceback():
+                raise exceptions.ResourcesMismatchError(
+                    'Infeasible resource demands found:'
+                    '\n  Instance type requested: '
+                    f'{resources.instance_type}\n'
+                    f'  Accelerators for {resources.instance_type}: '
+                    f'{acc_from_instance_type}\n'
+                    f'  Accelerators requested: {resources.accelerators}\n'
+                    f'To fix: either only specify instance_type, or '
+                    'change the accelerators field to be consistent.')
+
+    @classmethod
     def check_quota_available(cls,
                               region: str,
                               instance_type: str,
                               use_spot: bool = False) -> bool:
         """Check if quota is available for `instance_type` in `region`.
 
         (Currently, check_quota_available is only implemented for AWS.)
@@ -522,14 +574,15 @@
         because, for example, _retry_zones may only need to go through one or
         a few regions before a successful region, and running a query to check
         *every* region's quota beforehand would cause an unnecessary delay.
 
         Returns:
             False if the quota is found to be zero, and true otherwise.
         """
+        del region, instance_type, use_spot  # unused
 
         return True
 
     @classmethod
     def query_status(cls, name: str, tag_filters: Dict[str, str],
                      region: Optional[str], zone: Optional[str],
                      **kwargs) -> List['status_lib.ClusterStatus']:
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,15 +390,15 @@
         assert image_id is not None, (image_id, r)
         resources_vars['image_id'] = image_id
 
         resources_vars['disk_tier'] = GCP._get_disk_type(r.disk_tier)
 
         return resources_vars
 
-    def get_feasible_launchable_resources(self, resources):
+    def _get_feasible_launchable_resources(self, resources):
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             return ([resources], [])
 
         if resources.accelerators is None:
             # Return a default instance type with the given number of vCPUs.
             host_vm_type = GCP.get_default_instance_type(
@@ -762,26 +762,20 @@
             raise exceptions.CloudUserIdentityError(
                 'Failed to get GCP project id. Please make sure you have '
                 'run the following: gcloud init; '
                 'gcloud auth application-default login')
         return project_id
 
     @staticmethod
-    def check_host_accelerator_compatibility(
-            instance_type: str, accelerators: Optional[Dict[str, int]]) -> None:
-        service_catalog.check_host_accelerator_compatibility(
-            instance_type, accelerators, 'gcp')
-
-    @staticmethod
-    def check_accelerator_attachable_to_host(
-            instance_type: str,
-            accelerators: Optional[Dict[str, int]],
-            zone: Optional[str] = None) -> None:
+    def _check_instance_type_accelerators_combination(
+            resources: 'resources.Resources') -> None:
+        assert resources.is_launchable(), resources
         service_catalog.check_accelerator_attachable_to_host(
-            instance_type, accelerators, zone, 'gcp')
+            resources.instance_type, resources.accelerators, resources.zone,
+            'gcp')
 
     @classmethod
     def check_disk_tier_enabled(cls, instance_type: str,
                                 disk_tier: str) -> None:
         del instance_type, disk_tier  # unused
 
     @classmethod
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/ibm.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,16 +242,16 @@
             memory: Optional[str] = None,
             disk_tier: Optional[str] = None) -> Optional[str]:
         return service_catalog.get_default_instance_type(cpus=cpus,
                                                          memory=memory,
                                                          disk_tier=disk_tier,
                                                          clouds='ibm')
 
-    def get_feasible_launchable_resources(self,
-                                          resources: 'resources_lib.Resources'):
+    def _get_feasible_launchable_resources(
+            self, resources: 'resources_lib.Resources'):
         """Returns a list of feasible and launchable resources.
 
         Feasible resources refer to an offering respecting the resource
         requirements.  Currently, this function implements "filtering" the
         cloud's offerings only w.r.t. accelerators constraints.
 
         Launchable resources require a cloud and an instance type be assigned.
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/lambda_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,16 +159,16 @@
 
         return {
             'instance_type': resources.instance_type,
             'custom_resources': custom_resources,
             'region': region.name,
         }
 
-    def get_feasible_launchable_resources(self,
-                                          resources: 'resources_lib.Resources'):
+    def _get_feasible_launchable_resources(
+            self, resources: 'resources_lib.Resources'):
         if resources.use_spot or resources.disk_tier is not None:
             return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Accelerators are part of the instance type in Lambda Cloud
             resources = resources.copy(accelerators=None)
             return ([resources], [])
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,16 +130,16 @@
 
     def make_deploy_resources_variables(
             self, resources: 'resources_lib.Resources',
             region: Optional['clouds.Region'],
             zones: Optional[List['clouds.Zone']]) -> Dict[str, Optional[str]]:
         return {}
 
-    def get_feasible_launchable_resources(self,
-                                          resources: 'resources_lib.Resources'):
+    def _get_feasible_launchable_resources(
+            self, resources: 'resources_lib.Resources'):
         if resources.disk_tier is not None:
             return ([], [])
         # The entire local cluster's resources is considered launchable, as the
         # check for task resources is deferred later.
         # The check for task resources meeting cluster resources is run in
         # cloud_vm_ray_backend._check_task_resources_smaller_than_cluster.
         resources = resources.copy(
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/oci.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,16 +271,16 @@
             'zone': f'{_tenancy_prefix}:{zone}',
             'image': image_id,
             'app_catalog_listing_id': listing_id,
             'resource_version': res_ver,
             'use_spot': resources.use_spot
         }
 
-    def get_feasible_launchable_resources(self,
-                                          resources: 'resources_lib.Resources'):
+    def _get_feasible_launchable_resources(
+            self, resources: 'resources_lib.Resources'):
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             resources = resources.copy(accelerators=None)
             return ([resources], [])
 
         def _make(instance_list):
             resource_list = []
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/scp.py`

 * *Files 4% similar despite different names*

```diff
@@ -224,18 +224,22 @@
         # CloudVMRayBackend will be correctly triggered.
         # TODO(zhwu): This is a information leakage to the cloud implementor,
         # we need to find a better way to handle this.
         raise exceptions.ResourcesUnavailableError(
             'No image found in catalog for region '
             f'{region_name}. Try setting a valid image_id.')
 
-    def get_feasible_launchable_resources(self,
-                                          resources: 'resources_lib.Resources'):
+    def _get_feasible_launchable_resources(
+            self, resources: 'resources_lib.Resources'):
         if resources.use_spot or resources.disk_tier is not None:
             return ([], [])
+        # Check if the host VM satisfies the min/max disk size limits.
+        is_allowed = self._is_disk_size_allowed(resources)
+        if not is_allowed:
+            return ([], [])
         if resources.instance_type is not None:
             assert resources.is_launchable(), resources
             # Accelerators are part of the instance type in SCP Cloud
             resources = resources.copy(accelerators=None)
             return ([resources], [])
 
         def _make(instance_list):
@@ -322,24 +326,24 @@
                                       acc_count: int,
                                       region: Optional[str] = None,
                                       zone: Optional[str] = None) -> bool:
         return service_catalog.accelerator_in_region_or_zone(
             accelerator, acc_count, region, zone, 'scp')
 
     @staticmethod
-    def is_disk_size_allowed(resources):
+    def _is_disk_size_allowed(resources):
         if (resources.disk_size and
             (resources.disk_size < _SCP_MIN_DISK_SIZE_GB or
              resources.disk_size > _SCP_MAX_DISK_SIZE_GB)):
             logger.info(f'In SCP, the disk size must range between'
                         f' {_SCP_MIN_DISK_SIZE_GB} GB '
                         f'and {_SCP_MAX_DISK_SIZE_GB} GB. '
                         f'Input: {resources.disk_size}')
-            return False, []
-        return True, [resources]
+            return False
+        return True
 
     @classmethod
     def query_status(cls, name: str, tag_filters: Dict[str, str],
                      region: Optional[str], zone: Optional[str],
                      **kwargs) -> List[status_lib.ClusterStatus]:
         del tag_filters, region, zone, kwargs  # Unused.
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -256,30 +256,14 @@
         use_spot: bool,
         clouds: CloudFilter = None) -> 'List[cloud.Region]':
     """Returns a list of regions for a given accelerators."""
     return _map_clouds_catalog(clouds, 'get_region_zones_for_accelerators',
                                acc_name, acc_count, use_spot)
 
 
-def check_host_accelerator_compatibility(instance_type: str,
-                                         accelerators: Optional[Dict[str, int]],
-                                         clouds: CloudFilter = None) -> None:
-    """GCP only: Check if host VM type is compatible with the accelerators.
-
-    This function is invoked whenever a Resources object is created.
-    This function ensures that TPUs and GPUs (except A100) are attached to N1,
-    and A100 GPUs are attached to A2 machines. However, it does NOT check
-    the maximum vCPU count and maximum memory limits for the accelerators
-    because any Resources like GCP(n1-highmem-64, {'V100': 0.01}) can be valid
-    for sky exec/launch on an existing cluster.
-    """
-    _map_clouds_catalog(clouds, 'check_host_accelerator_compatibility',
-                        instance_type, accelerators)
-
-
 def check_accelerator_attachable_to_host(instance_type: str,
                                          accelerators: Optional[Dict[str, int]],
                                          zone: Optional[str] = None,
                                          clouds: CloudFilter = None) -> None:
     """GCP only: Check if the accelerators can be attached to the host VM.
 
     Specifically, this function checks the max CPU count and memory of the host
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/aws_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,32 @@
 _image_df = common.read_catalog('aws/images.csv',
                                 pull_frequency_hours=_PULL_FREQUENCY_HOURS)
 
 _quotas_df = common.read_catalog('aws/instance_quota_mapping.csv',
                                  pull_frequency_hours=_PULL_FREQUENCY_HOURS)
 
 
+def _get_az_mappings(aws_user_hash: str) -> Optional[pd.DataFrame]:
+    az_mapping_path = common.get_catalog_path(
+        f'aws/az_mappings-{aws_user_hash}.csv')
+    if not os.path.exists(az_mapping_path):
+        az_mappings = None
+        if aws_user_hash != 'default':
+            # Fetch az mapping from AWS.
+            logger.info(f'{colorama.Style.DIM}Fetching availability zones '
+                        f'mapping for AWS...{colorama.Style.RESET_ALL}')
+            az_mappings = fetch_aws.fetch_availability_zone_mappings()
+        else:
+            return None
+        az_mappings.to_csv(az_mapping_path, index=False)
+    else:
+        az_mappings = pd.read_csv(az_mapping_path)
+    return az_mappings
+
+
 def _fetch_and_apply_az_mapping(df: pd.DataFrame) -> pd.DataFrame:
     """Maps zone IDs (use1-az1) to zone names (us-east-1x).
 
     The upper-level functions that use the availability zone information
     should be able to handle the case where the zone name is not correct,
     due to the credentials not being configured.
 
@@ -110,31 +128,20 @@
             aws_user_hash = aws_user_hash.split('.')[0]
         else:
             aws_user_hash = 'default'
         logger.debug(
             'Failed to get AWS user identity. Using the latest mapping '
             f'file for user {aws_user_hash!r}.')
 
-    az_mapping_path = common.get_catalog_path(
-        f'aws/az_mappings-{aws_user_hash}.csv')
-    if not os.path.exists(az_mapping_path):
-        az_mappings = None
-        if aws_user_hash != 'default':
-            # Fetch az mapping from AWS.
-            logger.info(f'{colorama.Style.DIM}Fetching availability zones '
-                        f'mapping for AWS...{colorama.Style.RESET_ALL}')
-            az_mappings = fetch_aws.fetch_availability_zone_mappings()
-        else:
-            # Returning the original dataframe directly, as no cloud
-            # identity can be fetched which suggests there are no
-            # credentials.
-            return df
-        az_mappings.to_csv(az_mapping_path, index=False)
-    else:
-        az_mappings = pd.read_csv(az_mapping_path)
+    az_mappings = _get_az_mappings(aws_user_hash)
+    if az_mappings is None:
+        # Returning the original dataframe directly, as no cloud
+        # identity can be fetched which suggests there are no
+        # credentials.
+        return df
     # Use inner join to drop rows with unknown AZ IDs, which are likely
     # because the user does not have access to that Region. Otherwise,
     # there will be rows with NaN in the AvailabilityZone column.
     df = df.merge(az_mappings, on=['AvailabilityZone'], how='inner')
     df = df.drop(columns=['AvailabilityZone']).rename(
         columns={'AvailabilityZoneName': 'AvailabilityZone'})
     return df
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         return (f'\nList of supported {cloud_name} regions: '
                 f'{", ".join(all_regions)!r}')
 
     validated_region, validated_zone = region, zone
 
     filter_df = df
     if region is not None:
-        filter_df = filter_df[filter_df['Region'].str.lower() == region.lower()]
+        filter_df = _filter_region_zone(filter_df, region, zone=None)
         if len(filter_df) == 0:
             with ux_utils.print_exception_no_traceback():
                 error_msg = (f'Invalid region {region!r}')
                 candidate_strs = _get_candidate_str(
                     region.lower(), df['Region'].str.lower().unique())
                 if not candidate_strs:
                     error_msg += _get_all_supported_regions_str()
@@ -331,14 +331,23 @@
         return df[df['MemoryGiB'] >= memory]
     elif memory_gb_or_ratio.endswith('x'):
         return df[df['MemoryGiB'] >= df['vCPUs'] * memory]
     else:
         return df[df['MemoryGiB'] == memory]
 
 
+def _filter_region_zone(df: pd.DataFrame, region: Optional[str],
+                        zone: Optional[str]) -> pd.DataFrame:
+    if region is not None:
+        df = df[df['Region'].str.lower() == region.lower()]
+    if zone is not None:
+        df = df[df['AvailabilityZone'].str.lower() == zone.lower()]
+    return df
+
+
 def get_instance_type_for_cpus_mem_impl(
         df: pd.DataFrame, cpus: Optional[str],
         memory_gb_or_ratio: Optional[str]) -> Optional[str]:
     """Returns the cheapest instance type that satisfies the requirements.
 
     Args:
         df: The catalog cloud catalog data frame.
@@ -387,35 +396,33 @@
 ) -> Tuple[Optional[List[str]], List[str]]:
     """
     Returns a list of instance types satisfying the required count of
     accelerators with sorted prices and a list of candidates with fuzzy search.
     """
     result = df[(df['AcceleratorName'].str.fullmatch(acc_name, case=False)) &
                 (df['AcceleratorCount'] == acc_count)]
+    result = _filter_region_zone(result, region, zone)
     if len(result) == 0:
         fuzzy_result = df[
             (df['AcceleratorName'].str.contains(acc_name, case=False)) &
             (df['AcceleratorCount'] >= acc_count)]
+        fuzzy_result = _filter_region_zone(fuzzy_result, region, zone)
         fuzzy_result = fuzzy_result.sort_values('Price', ascending=True)
         fuzzy_result = fuzzy_result[['AcceleratorName',
                                      'AcceleratorCount']].drop_duplicates()
         fuzzy_candidate_list = []
         if len(fuzzy_result) > 0:
             for _, row in fuzzy_result.iterrows():
                 fuzzy_candidate_list.append(f'{row["AcceleratorName"]}:'
                                             f'{int(row["AcceleratorCount"])}')
         return (None, fuzzy_candidate_list)
 
     result = _filter_with_cpus(result, cpus)
     result = _filter_with_mem(result, memory)
-    if region is not None:
-        result = result[result['Region'].str.lower() == region]
-    if zone is not None:
-        # NOTE: For Azure regions, zone must be None.
-        result = result[result['AvailabilityZone'] == zone]
+    result = _filter_region_zone(result, region, zone)
     if len(result) == 0:
         return ([], [])
 
     # Current strategy: choose the cheapest instance
     price_str = 'SpotPrice' if use_spot else 'Price'
     result = result.sort_values(price_str, ascending=True)
     instance_types = list(result['InstanceType'].drop_duplicates())
@@ -565,27 +572,25 @@
 
     If region is None, there must be only one image with the given tag.
 
     Returns None if a region (or globally if region is None) does not have
     an image that matches the tag.
     """
     df = df[df['Tag'] == tag]
-    if region is not None:
-        df = df[df['Region'].str.lower() == region.lower()]
+    df = _filter_region_zone(df, region, zone=None)
     assert len(df) <= 1, ('Multiple images found for tag '
                           f'{tag} in region {region}')
     if len(df) == 0:
         return None
     image_id = df['ImageId'].iloc[0]
     if pd.isna(image_id):
         return None
     return image_id
 
 
 def is_image_tag_valid_impl(df: pd.DataFrame, tag: str,
                             region: Optional[str]) -> bool:
     """Returns True if the image tag is valid."""
     df = df[df['Tag'] == tag]
-    if region is not None:
-        df = df[df['Region'].str.lower() == region.lower()]
+    df = _filter_region_zone(df, region, zone=None)
     df = df.dropna(subset=['ImageId'])
     return len(df) > 0
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,123 +394,100 @@
     use_spot: bool = False,
 ) -> List['cloud.Region']:
     """Returns a list of regions for a given accelerators."""
     df = _get_accelerator(_df, accelerator, count, region=None)
     return common.get_region_zones(df, use_spot)
 
 
-def check_host_accelerator_compatibility(
-        instance_type: str, accelerators: Optional[Dict[str, int]]) -> None:
-    """Check if the instance type is compatible with the accelerators.
+def check_accelerator_attachable_to_host(instance_type: str,
+                                         accelerators: Optional[Dict[str, int]],
+                                         zone: Optional[str] = None) -> None:
+    """Check if the accelerators can be attached to the host.
+
+    This function checks the max CPU count and memory of the host that
+    the accelerators can be attached to.
 
-    This function ensures that TPUs and GPUs except A100 are attached to N1,
-    and A100 GPUs are attached to A2 machines.
+    Raises:
+        exceptions.ResourcesMismatchError: If the accelerators cannot be
+            attached to the host.
     """
     if accelerators is None:
         if instance_type.startswith('a2-'):
             # NOTE: While it is allowed to use A2 machines as CPU-only nodes,
             # we exclude this case as it is uncommon and undesirable.
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesMismatchError(
                     'A2 instance types should be used with A100 GPUs. '
                     'Either use other instance types or specify the '
                     'accelerators as A100.')
         return
 
     acc = list(accelerators.items())
     assert len(acc) == 1, acc
-    acc_name, _ = acc[0]
+    acc_name, acc_count = acc[0]
 
     # Check if the accelerator is supported by GCP.
     if not list_accelerators(gpus_only=False, name_filter=acc_name):
         with ux_utils.print_exception_no_traceback():
-            raise exceptions.ResourcesUnavailableError(
+            raise exceptions.ResourcesMismatchError(
                 f'{acc_name} is not available in GCP. '
                 'See \'sky show-gpus --cloud gcp\'')
 
     if acc_name.startswith('tpu-'):
         if instance_type != 'TPU-VM' and not instance_type.startswith('n1-'):
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesMismatchError(
                     'TPU Nodes can be only used with N1 machines. '
                     'Please refer to: '
                     'https://cloud.google.com/compute/docs/general-purpose-machines#n1_machines')  # pylint: disable=line-too-long
         return
 
     # Treat A100 as a special case.
     if acc_name in _A100_INSTANCE_TYPE_DICTS:
-        # A100 must be attached to A2 instance type.
-        if not instance_type.startswith('a2-'):
+        a100_instance_type = _A100_INSTANCE_TYPE_DICTS[acc_name][acc_count]
+        if instance_type != a100_instance_type:
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesMismatchError(
-                    f'A100 GPUs cannot be attached to {instance_type}. '
-                    f'Use A2 machines instead. Please refer to '
+                    f'A100:{acc_count} cannot be attached to {instance_type}. '
+                    f'Use {a100_instance_type} instead. Please refer to '
                     'https://cloud.google.com/compute/docs/gpus#a100-gpus')
-        return
-
-    # Other GPUs must be attached to N1 machines.
-    # Refer to: https://cloud.google.com/compute/docs/machine-types#gpus
-    if not instance_type.startswith('n1-'):
+    elif not instance_type.startswith('n1-'):
+        # Other GPUs must be attached to N1 machines.
+        # Refer to: https://cloud.google.com/compute/docs/machine-types#gpus
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ResourcesMismatchError(
                 f'{acc_name} GPUs cannot be attached to {instance_type}. '
                 'Use N1 instance types instead. Please refer to: '
                 'https://cloud.google.com/compute/docs/machine-types#gpus')
 
-
-def check_accelerator_attachable_to_host(instance_type: str,
-                                         accelerators: Optional[Dict[str, int]],
-                                         zone: Optional[str] = None) -> None:
-    """Check if the accelerators can be attached to the host.
-
-    This function checks the max CPU count and memory of the host that
-    the accelerators can be attached to.
-    """
-    if accelerators is None:
-        return
-
-    acc = list(accelerators.items())
-    assert len(acc) == 1, acc
-    acc_name, acc_count = acc[0]
-
-    if acc_name.startswith('tpu-'):
-        # TODO(woosuk): Check max vCPUs and memory for each TPU type.
-        assert instance_type == 'TPU-VM' or instance_type.startswith('n1-')
-        return
-
     if acc_name in _A100_INSTANCE_TYPE_DICTS:
         valid_counts = list(_A100_INSTANCE_TYPE_DICTS[acc_name].keys())
     else:
         assert acc_name in _NUM_ACC_TO_MAX_CPU_AND_MEMORY, acc_name
         valid_counts = list(_NUM_ACC_TO_MAX_CPU_AND_MEMORY[acc_name].keys())
     if acc_count not in valid_counts:
         with ux_utils.print_exception_no_traceback():
             raise exceptions.ResourcesMismatchError(
                 f'{acc_name}:{acc_count} is not launchable on GCP. '
                 f'The valid {acc_name} counts are {valid_counts}.')
 
-    if acc_name in _A100_INSTANCE_TYPE_DICTS:
-        a100_instance_type = _A100_INSTANCE_TYPE_DICTS[acc_name][acc_count]
-        if instance_type != a100_instance_type:
-            with ux_utils.print_exception_no_traceback():
-                raise exceptions.ResourcesMismatchError(
-                    f'A100:{acc_count} cannot be attached to {instance_type}. '
-                    f'Use {a100_instance_type} instead. Please refer to '
-                    'https://cloud.google.com/compute/docs/gpus#a100-gpus')
-        return
-
     # Check maximum vCPUs and memory.
-    max_cpus, max_memory = _NUM_ACC_TO_MAX_CPU_AND_MEMORY[acc_name][acc_count]
-    if acc_name == 'K80' and acc_count == 8:
-        if zone in ['asia-east1-a', 'us-east1-d']:
-            max_memory = 416
-    elif acc_name == 'P100' and acc_count == 4:
-        if zone in ['us-east1-c', 'europe-west1-d', 'europe-west1-b']:
-            max_cpus = 64
-            max_memory = 208
+    if acc_name in _A100_INSTANCE_TYPE_DICTS:
+        max_cpus, max_memory = get_vcpus_mem_from_instance_type(
+            a100_instance_type)
+    else:
+        max_cpus, max_memory = _NUM_ACC_TO_MAX_CPU_AND_MEMORY[acc_name][
+            acc_count]
+        if acc_name == 'K80' and acc_count == 8:
+            if zone in ['asia-east1-a', 'us-east1-d']:
+                max_memory = 416
+        elif acc_name == 'P100' and acc_count == 4:
+            if zone in ['us-east1-c', 'europe-west1-d', 'europe-west1-b']:
+                max_cpus = 64
+                max_memory = 208
 
     # vCPU counts and memory sizes of N1 machines.
     df = _df[_df['InstanceType'] == instance_type]
     num_cpus = df['vCPUs'].iloc[0]
     memory = df['MemoryGiB'].iloc[0]
 
     if num_cpus > max_cpus:
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230715/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/core.py` & `skypilot-nightly-1.0.0.dev20230715/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230715/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230715/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230715/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230715/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230715/sky/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,47 +324,47 @@
                 handle = backend.provision(task,
                                            task.best_resources,
                                            dryrun=dryrun,
                                            stream_logs=stream_logs,
                                            cluster_name=cluster_name,
                                            retry_until_up=retry_until_up)
 
-        if dryrun:
-            logger.info('Dry run finished.')
+        if dryrun and handle is None:
+            logger.info('Dryrun finished.')
             return
 
-        if Stage.SYNC_WORKDIR in stages:
+        if Stage.SYNC_WORKDIR in stages and not dryrun:
             if task.workdir is not None:
                 backend.sync_workdir(handle, task.workdir)
 
-        if Stage.SYNC_FILE_MOUNTS in stages:
+        if Stage.SYNC_FILE_MOUNTS in stages and not dryrun:
             backend.sync_file_mounts(handle, task.file_mounts,
                                      task.storage_mounts)
 
         if no_setup:
             logger.info('Setup commands skipped.')
-        elif Stage.SETUP in stages:
+        elif Stage.SETUP in stages and not dryrun:
             backend.setup(handle, task, detach_setup=detach_setup)
 
-        if Stage.PRE_EXEC in stages:
+        if Stage.PRE_EXEC in stages and not dryrun:
             if idle_minutes_to_autostop is not None:
                 assert isinstance(backend, backends.CloudVmRayBackend)
                 backend.set_autostop(handle,
                                      idle_minutes_to_autostop,
                                      down=down)
 
         if Stage.EXEC in stages:
             try:
                 global_user_state.update_last_use(handle.get_cluster_name())
-                backend.execute(handle, task, detach_run)
+                backend.execute(handle, task, detach_run, dryrun=dryrun)
             finally:
                 # Enables post_execute() to be run after KeyboardInterrupt.
                 backend.post_execute(handle, down)
 
-        if Stage.DOWN in stages:
+        if Stage.DOWN in stages and not dryrun:
             if down and idle_minutes_to_autostop is None:
                 backend.teardown_ephemeral_storage(task)
                 backend.teardown(handle, terminate=True)
     finally:
         if cluster_name != spot.SPOT_CONTROLLER_NAME:
             # UX: print live clusters to make users aware (to save costs).
             #
@@ -566,15 +566,16 @@
             f'{colorama.Style.RESET_ALL}')
     backend_utils.check_cluster_name_not_reserved(cluster_name,
                                                   operation_str='sky.exec')
 
     handle = backend_utils.check_cluster_available(
         cluster_name,
         operation='executing tasks',
-        check_cloud_vm_ray_backend=False)
+        check_cloud_vm_ray_backend=False,
+        dryrun=dryrun)
     _execute(entrypoint=entrypoint,
              dryrun=dryrun,
              down=down,
              stream_logs=stream_logs,
              handle=handle,
              backend=backend,
              stages=[
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230715/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230715/sky/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
                         elif specified_resources.region:
                             location_hint = (
                                 f' Region: {specified_resources.region}.')
 
                     error_msg = (
                         'No launchable resource found for task '
                         f'{node}.{location_hint}\nThis means the '
-                        'catalog does not contain any instance types that '
+                        'catalog does not contain any resources that '
                         'satisfy this request.\n'
                         'To fix: relax or change the resource requirements.\n'
                         'Hint: \'sky show-gpus --all\' '
                         'to list available accelerators.\n'
                         '      \'sky check\' to check the enabled clouds.')
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.ResourcesUnavailableError(error_msg)
@@ -950,38 +950,14 @@
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesUnavailableError(
                     f'task_lib.Task {task} requires {resources.cloud} which is '
                     'not enabled. To enable access, run '
                     f'{colorama.Style.BRIGHT}'
                     f'sky check {colorama.Style.RESET_ALL}, or change the '
                     'cloud requirement')
-        elif resources.is_launchable():
-            if isinstance(resources.cloud, clouds.GCP):
-                # Check if the host VM satisfies the max vCPU and memory limits.
-                clouds.GCP.check_accelerator_attachable_to_host(
-                    resources.instance_type, resources.accelerators,
-                    resources.zone)
-            # If the user has specified a GCP zone and the zone does not support
-            # the host-accelerator combination, then an error will be raised by
-            # the above check_accelerator_attachable_to_host() call.
-            # If the user has not specified any zone, a launchable will be made
-            # for every zone even if some of the zones do not support the
-            # host-accelerator combination. Then the provisioner may try to
-            # launch the instance, and fail over to other zones. We find this
-            # behavior acceptable because this will happen only when the user
-            # requested GCP 4:P100 or 8:K80 with a very large host VM.
-            elif isinstance(resources.cloud, clouds.SCP):
-                # Check if the host VM satisfies the min/max disk size limits.
-                is_allowed, launchable[resources] = \
-                    clouds.SCP.is_disk_size_allowed(resources)
-                if not is_allowed:
-                    continue
-
-            launchable[resources] = _make_launchables_for_valid_region_zones(
-                resources)
         else:
             clouds_list = ([resources.cloud]
                            if resources.cloud is not None else enabled_clouds)
             # Hack: When >=2 cloud candidates, always remove local cloud from
             # possible candidates. This is so the optimizer will consider
             # public clouds, except local. Local will be included as part of
             # optimizer in a future PR.
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230715/sky/provision/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Cloud provision interface.
 
 This module provides a standard low-level interface that all
 providers supported by SkyPilot need to follow.
 """
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 import functools
 import importlib
 import inspect
 
 
 def _route_to_cloud_impl(func):
@@ -33,24 +33,28 @@
 
 # pylint: disable=unused-argument
 
 # TODO(suquark): Bring all other functions here from the
 
 
 @_route_to_cloud_impl
-def stop_instances(provider_name: str,
-                   region: str,
-                   cluster_name: str,
-                   included_instances: Optional[List[str]] = None,
-                   excluded_instances: Optional[List[str]] = None) -> None:
+def stop_instances(
+    provider_name: str,
+    cluster_name: str,
+    provider_config: Optional[Dict[str, Any]] = None,
+    included_instances: Optional[List[str]] = None,
+    excluded_instances: Optional[List[str]] = None,
+) -> None:
     """Stop running instances."""
     raise NotImplementedError
 
 
 @_route_to_cloud_impl
-def terminate_instances(provider_name: str,
-                        region: str,
-                        cluster_name: str,
-                        included_instances: Optional[List[str]] = None,
-                        excluded_instances: Optional[List[str]] = None) -> None:
+def terminate_instances(
+    provider_name: str,
+    cluster_name: str,
+    provider_config: Optional[Dict[str, Any]] = None,
+    included_instances: Optional[List[str]] = None,
+    excluded_instances: Optional[List[str]] = None,
+) -> None:
     """Terminate running or stopped instances."""
     raise NotImplementedError
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230715/sky/provision/aws/instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,19 +23,23 @@
         for inst in list(instances):
             if inst.id not in excluded_instances:
                 included_instances.append(inst.id)
         instances = instances.filter(InstanceIds=included_instances)
     return instances
 
 
-def stop_instances(region: str,
-                   cluster_name: str,
-                   included_instances: Optional[List[str]] = None,
-                   excluded_instances: Optional[List[str]] = None) -> None:
+def stop_instances(
+    cluster_name: str,
+    provider_config: Optional[Dict[str, Any]] = None,
+    included_instances: Optional[List[str]] = None,
+    excluded_instances: Optional[List[str]] = None,
+) -> None:
     """See sky/provision/__init__.py"""
+    assert provider_config is not None, (cluster_name, provider_config)
+    region = provider_config['region']
     ec2 = aws.resource(
         'ec2',
         region_name=region,
         config=config.Config(retries={'max_attempts': BOTO_MAX_RETRIES}))
     filters = [
         {
             'Name': 'instance-state-name',
@@ -53,19 +57,23 @@
     #  wait util the cluster is fully terminated, while other clouds just
     #  trigger the termination process (via http call) and then return.
     #  It's not clear that which behavior should be expected. We will not
     #  wait for the termination for now, since this is the default behavior
     #  of most cloud implementations (including AWS).
 
 
-def terminate_instances(region: str,
-                        cluster_name: str,
-                        included_instances: Optional[List[str]] = None,
-                        excluded_instances: Optional[List[str]] = None) -> None:
+def terminate_instances(
+    cluster_name: str,
+    provider_config: Optional[Dict[str, Any]] = None,
+    included_instances: Optional[List[str]] = None,
+    excluded_instances: Optional[List[str]] = None,
+) -> None:
     """See sky/provision/__init__.py"""
+    assert provider_config is not None, (cluster_name, provider_config)
+    region = provider_config['region']
     ec2 = aws.resource(
         'ec2',
         region_name=region,
         config=config.Config(retries={'max_attempts': BOTO_MAX_RETRIES}))
     filters = [
         {
             'Name': 'instance-state-name',
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230715/sky/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -158,15 +158,14 @@
         self._set_cpus(cpus)
         self._set_memory(memory)
         self._set_accelerators(accelerators, accelerator_args)
 
         self._try_validate_local()
         self._try_validate_instance_type()
         self._try_validate_cpus_mem()
-        self._try_validate_accelerators()
         self._try_validate_spot()
         self._try_validate_image_id()
         self._try_validate_disk_tier()
 
     def __repr__(self) -> str:
         """Returns a string representation for display.
 
@@ -501,15 +500,16 @@
 
         Each `Region` has a list of `Zone`s that can provision this Resources.
 
         (Internal) This function respects any config in skypilot_config that
         may have restricted the regions to be considered (e.g., a
         ssh_proxy_command dict with region names as keys).
         """
-        assert self.is_launchable()
+        assert self.is_launchable(), self
+
         regions = self._cloud.regions_with_offering(self._instance_type,
                                                     self.accelerators,
                                                     self._use_spot,
                                                     self._region, self._zone)
         if self._image_id is not None and None not in self._image_id:
             regions = [r for r in regions if r.name in self._image_id]
 
@@ -620,64 +620,14 @@
                 elif mem != float(self.memory):
                     with ux_utils.print_exception_no_traceback():
                         raise ValueError(
                             f'{self.instance_type} does not have the requested '
                             f'memory. {self.instance_type} has {mem} GB '
                             f'memory, but {self.memory} is requested.')
 
-    def _try_validate_accelerators(self) -> None:
-        """Validate accelerators against the instance type and region/zone."""
-        acc_requested = self.accelerators
-        if (isinstance(self.cloud, clouds.GCP) and
-                self.instance_type is not None):
-            # Do this check even if acc_requested is None.
-            clouds.GCP.check_host_accelerator_compatibility(
-                self.instance_type, acc_requested)
-
-        if acc_requested is None:
-            return
-
-        if self.is_launchable() and not isinstance(self.cloud, clouds.GCP):
-            # GCP attaches accelerators to VMs, so no need for this check.
-            acc_requested = self.accelerators
-            acc_from_instance_type = (
-                self.cloud.get_accelerators_from_instance_type(
-                    self._instance_type))
-            if not Resources(accelerators=acc_requested).less_demanding_than(
-                    Resources(accelerators=acc_from_instance_type)):
-                with ux_utils.print_exception_no_traceback():
-                    raise ValueError(
-                        'Infeasible resource demands found:\n'
-                        f'  Instance type requested: {self._instance_type}\n'
-                        f'  Accelerators for {self._instance_type}: '
-                        f'{acc_from_instance_type}\n'
-                        f'  Accelerators requested: {acc_requested}\n'
-                        f'To fix: either only specify instance_type, or change '
-                        'the accelerators field to be consistent.')
-            # NOTE: should not clear 'self.accelerators' even for AWS/Azure,
-            # because e.g., the instance may have 4 GPUs, while the task
-            # specifies to use 1 GPU.
-
-        # Validate whether accelerator is available in specified region/zone.
-        acc, acc_count = list(acc_requested.items())[0]
-        # Fractional accelerators are temporarily bumped up to 1.
-        if 0 < acc_count < 1:
-            acc_count = 1
-        if self.region is not None or self.zone is not None:
-            if not self._cloud.accelerator_in_region_or_zone(
-                    acc, acc_count, self.region, self.zone):
-                error_str = (f'Accelerator "{acc}" is not available in '
-                             '"{}".')
-                if self.zone:
-                    error_str = error_str.format(self.zone)
-                else:
-                    error_str = error_str.format(self.region)
-                with ux_utils.print_exception_no_traceback():
-                    raise ValueError(error_str)
-
     def _try_validate_spot(self) -> None:
         if self._spot_recovery is None:
             return
         if not self._use_spot:
             with ux_utils.print_exception_no_traceback():
                 raise ValueError(
                     'Cannot specify spot_recovery without use_spot set to True.'
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230715/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230715/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230715/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230715/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/recovery_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,16 @@
                 sky.launch(self.dag,
                            cluster_name=self.cluster_name,
                            detach_setup=True,
                            detach_run=True,
                            _is_launched_by_spot_controller=True)
                 logger.info('Spot cluster launched.')
             except (exceptions.InvalidClusterNameError,
-                    exceptions.NoCloudAccessError) as e:
+                    exceptions.NoCloudAccessError,
+                    exceptions.ResourcesMismatchError) as e:
                 logger.error('Failure happened before provisioning. '
                              f'{common_utils.format_exception(e)}')
                 if raise_on_failure:
                     raise exceptions.ProvisionPrechecksError(reasons=[e])
                 return None
             except exceptions.ResourcesUnavailableError as e:
                 # This is raised when the launch fails due to prechecks or
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230715/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/task.py` & `skypilot-nightly-1.0.0.dev20230715/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230715/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230715/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230715/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230715/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230714
+Version: 1.0.0.dev20230715
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
@@ -92,15 +92,15 @@
 
 ## Getting Started
 You can find our documentation [here](https://skypilot.readthedocs.io/en/latest/).
 - [Installation](https://skypilot.readthedocs.io/en/latest/getting-started/installation.html)
 - [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html)
 - [CLI reference](https://skypilot.readthedocs.io/en/latest/reference/cli.html)
 
-## SkyPilot in 1 minute
+## SkyPilot in 1 Minute
 
 A SkyPilot task specifies: resource requirements, data to be synced, setup commands, and the task commands. 
 
 Once written in this [**unified interface**](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched on any available cloud.  This avoids vendor lock-in, and allows easily moving jobs to a different provider.
 
 Paste the following into a file `my_task.yaml`:
 
@@ -146,28 +146,39 @@
 <p align="center">
   <img src="https://i.imgur.com/TgamzZ2.gif" alt="SkyPilot Demo"/>
 </p>
 
 
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/quickstart.html) to get started with SkyPilot.
 
-## Learn more
+## More Information
+To learn more, see our [Documentation](https://skypilot.readthedocs.io/en/latest/) and [Tutorials](https://github.com/skypilot-org/skypilot-tutorial).
 
-- [Documentation](https://skypilot.readthedocs.io/en/latest/)
-- [Example: HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/tutorial.html) 
-- [Tutorials](https://github.com/skypilot-org/skypilot-tutorial) 
-- [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-spec.html)
-- Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml),  [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more](./examples).
-
-More information:
-- [SkyPilot Blog](https://blog.skypilot.co/)
-  - [Introductory blog post](https://blog.skypilot.co/introducing-skypilot/)
-- [NSDI 2023 paper & talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng)
+Runnable examples:
+- LLMs on SkyPilot
+  - [Vicuna chatbots: Training & Serving](./llm/vicuna/) (from official Vicuna team)
+  - [vLLM: Serving LLM 24x Faster On the Cloud](./llm/vllm/) (from official vLLM team)
+  - [QLoRA](https://github.com/artidoro/qlora/pull/132)
+  - [LLaMA-LoRA-Tuner](https://github.com/zetavg/LLaMA-LoRA-Tuner#run-on-a-cloud-service-via-skypilot)
+  - [Tabby: Self-hosted AI coding assistant](https://github.com/TabbyML/tabby/blob/bed723fcedb44a6b867ce22a7b1f03d2f3531c1e/experimental/eval/skypilot.yaml)
+  - [LocalGPT](./llm/localgpt)
+  - Add yours here & see more in [`llm/`](./llm)!
+- Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_torch.yaml), [DeepSpeed](./examples/deepspeed-multinode/sky.yaml), [JAX/Flax on TPU](https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/tree/master/examples/stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml), [Distributed](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/resnet_app_storage.yaml), [programmatic grid search](https://github.com/skypilot-org/skypilot/blob/master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many more (`examples/`)](./examples).
+
+Follow updates:
+- [Twitter](https://twitter.com/skypilot_org)
+- [Slack](http://slack.skypilot.co)
+- [SkyPilot Blog](https://blog.skypilot.co/) ([Introductory blog post](https://blog.skypilot.co/introducing-skypilot/))
+
+Read the research:
+- [SkyPilot paper](https://www.usenix.org/system/files/nsdi23-yang-zongheng.pdf) and [talk](https://www.usenix.org/conference/nsdi23/presentation/yang-zongheng) (NSDI 2023)
+- [Sky Computing whitepaper](https://arxiv.org/abs/2205.07147)
+- [Sky Computing vision paper](https://sigops.org/s/conferences/hotos/2021/papers/hotos21-s02-stoica.pdf) (HotOS 2021)
 
-## Issues, feature requests, and questions
+## Support and Questions
 We are excited to hear your feedback! 
 * For issues and feature requests, please [open a GitHub issue](https://github.com/skypilot-org/skypilot/issues/new).
 * For questions, please use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
 
 For general discussions, join us on the [SkyPilot Slack](http://slack.skypilot.co).
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230714
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230715
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -48,15 +48,15 @@
 Cloudflare):
                                   [SkyPilot]
 ## Getting Started You can find our documentation [here](https://
 skypilot.readthedocs.io/en/latest/). - [Installation](https://
 skypilot.readthedocs.io/en/latest/getting-started/installation.html) -
 [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-started/
 quickstart.html) - [CLI reference](https://skypilot.readthedocs.io/en/latest/
-reference/cli.html) ## SkyPilot in 1 minute A SkyPilot task specifies: resource
+reference/cli.html) ## SkyPilot in 1 Minute A SkyPilot task specifies: resource
 requirements, data to be synced, setup commands, and the task commands. Once
 written in this [**unified interface**](https://skypilot.readthedocs.io/en/
 latest/reference/yaml-spec.html) (YAML or Python API), the task can be launched
 on any available cloud. This avoids vendor lock-in, and allows easily moving
 jobs to a different provider. Paste the following into a file `my_task.yaml`:
 ```yaml resources: accelerators: V100:1 # 1x NVIDIA V100 GPU num_nodes: 1 #
 Number of VMs to launch # Working directory (optional) containing the project
@@ -72,35 +72,47 @@
 lifting for you, including: 1. Find the lowest priced VM instance type across
 different clouds 2. Provision the VM, with auto-failover if the cloud returned
 capacity errors 3. Sync the local `workdir` to the VM 4. Run the task's `setup`
 commands to prepare the VM for running the task 5. Run the task's `run`
 commands
                                 [SkyPilot Demo]
 Refer to [Quickstart](https://skypilot.readthedocs.io/en/latest/getting-
-started/quickstart.html) to get started with SkyPilot. ## Learn more -
-[Documentation](https://skypilot.readthedocs.io/en/latest/) - [Example:
-HuggingFace](https://skypilot.readthedocs.io/en/latest/getting-started/
-tutorial.html) - [Tutorials](https://github.com/skypilot-org/skypilot-tutorial)
-- [YAML reference](https://skypilot.readthedocs.io/en/latest/reference/yaml-
-spec.html) - Framework examples: [PyTorch DDP](https://github.com/skypilot-org/
-skypilot/blob/master/examples/resnet_distributed_torch.yaml), [Distributed]
-(https://github.com/skypilot-org/skypilot/blob/master/examples/
-resnet_distributed_tf_app.py) [TensorFlow](https://github.com/skypilot-org/
-skypilot/blob/master/examples/resnet_app_storage.yaml), [JAX/Flax on TPU]
-(https://github.com/skypilot-org/skypilot/blob/master/examples/tpu/
-tpuvm_mnist.yaml), [Stable Diffusion](https://github.com/skypilot-org/skypilot/
-tree/master/examples/stable_diffusion), [Detectron2](https://github.com/
-skypilot-org/skypilot/blob/master/examples/detectron2_docker.yaml),
-[programmatic grid search](https://github.com/skypilot-org/skypilot/blob/
-master/examples/huggingface_glue_imdb_grid_search_app.py), [Docker](https://
-github.com/skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml),
-and [many more](./examples). More information: - [SkyPilot Blog](https://
-blog.skypilot.co/) - [Introductory blog post](https://blog.skypilot.co/
-introducing-skypilot/) - [NSDI 2023 paper & talk](https://www.usenix.org/
-conference/nsdi23/presentation/yang-zongheng) ## Issues, feature requests, and
-questions We are excited to hear your feedback! * For issues and feature
-requests, please [open a GitHub issue](https://github.com/skypilot-org/
-skypilot/issues/new). * For questions, please use [GitHub Discussions](https://
-github.com/skypilot-org/skypilot/discussions). For general discussions, join us
-on the [SkyPilot Slack](http://slack.skypilot.co). ## Contributing We welcome
-and value all contributions to the project! Please refer to [CONTRIBUTING]
-(CONTRIBUTING.md) for how to get involved.
+started/quickstart.html) to get started with SkyPilot. ## More Information To
+learn more, see our [Documentation](https://skypilot.readthedocs.io/en/latest/
+) and [Tutorials](https://github.com/skypilot-org/skypilot-tutorial). Runnable
+examples: - LLMs on SkyPilot - [Vicuna chatbots: Training & Serving](./llm/
+vicuna/) (from official Vicuna team) - [vLLM: Serving LLM 24x Faster On the
+Cloud](./llm/vllm/) (from official vLLM team) - [QLoRA](https://github.com/
+artidoro/qlora/pull/132) - [LLaMA-LoRA-Tuner](https://github.com/zetavg/LLaMA-
+LoRA-Tuner#run-on-a-cloud-service-via-skypilot) - [Tabby: Self-hosted AI coding
+assistant](https://github.com/TabbyML/tabby/blob/
+bed723fcedb44a6b867ce22a7b1f03d2f3531c1e/experimental/eval/skypilot.yaml) -
+[LocalGPT](./llm/localgpt) - Add yours here & see more in [`llm/`](./llm)! -
+Framework examples: [PyTorch DDP](https://github.com/skypilot-org/skypilot/
+blob/master/examples/resnet_distributed_torch.yaml), [DeepSpeed](./examples/
+deepspeed-multinode/sky.yaml), [JAX/Flax on TPU](https://github.com/skypilot-
+org/skypilot/blob/master/examples/tpu/tpuvm_mnist.yaml), [Stable Diffusion]
+(https://github.com/skypilot-org/skypilot/tree/master/examples/
+stable_diffusion), [Detectron2](https://github.com/skypilot-org/skypilot/blob/
+master/examples/detectron2_docker.yaml), [Distributed](https://github.com/
+skypilot-org/skypilot/blob/master/examples/resnet_distributed_tf_app.py)
+[TensorFlow](https://github.com/skypilot-org/skypilot/blob/master/examples/
+resnet_app_storage.yaml), [programmatic grid search](https://github.com/
+skypilot-org/skypilot/blob/master/examples/
+huggingface_glue_imdb_grid_search_app.py), [Docker](https://github.com/
+skypilot-org/skypilot/blob/master/examples/docker/echo_app.yaml), and [many
+more (`examples/`)](./examples). Follow updates: - [Twitter](https://
+twitter.com/skypilot_org) - [Slack](http://slack.skypilot.co) - [SkyPilot Blog]
+(https://blog.skypilot.co/) ([Introductory blog post](https://blog.skypilot.co/
+introducing-skypilot/)) Read the research: - [SkyPilot paper](https://
+www.usenix.org/system/files/nsdi23-yang-zongheng.pdf) and [talk](https://
+www.usenix.org/conference/nsdi23/presentation/yang-zongheng) (NSDI 2023) - [Sky
+Computing whitepaper](https://arxiv.org/abs/2205.07147) - [Sky Computing vision
+paper](https://sigops.org/s/conferences/hotos/2021/papers/hotos21-s02-
+stoica.pdf) (HotOS 2021) ## Support and Questions We are excited to hear your
+feedback! * For issues and feature requests, please [open a GitHub issue]
+(https://github.com/skypilot-org/skypilot/issues/new). * For questions, please
+use [GitHub Discussions](https://github.com/skypilot-org/skypilot/discussions).
+For general discussions, join us on the [SkyPilot Slack](http://
+slack.skypilot.co). ## Contributing We welcome and value all contributions to
+the project! Please refer to [CONTRIBUTING](CONTRIBUTING.md) for how to get
+involved.
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 sky/data/data_utils.py
 sky/data/mounting_utils.py
 sky/data/storage.py
 sky/data/storage_utils.py
 sky/provision/__init__.py
 sky/provision/aws/__init__.py
 sky/provision/aws/instance.py
+sky/provision/gcp/__init__.py
+sky/provision/gcp/instance.py
+sky/provision/gcp/instance_utils.py
 sky/setup_files/MANIFEST.in
 sky/setup_files/setup.py
 sky/skylet/LICENSE
 sky/skylet/__init__.py
 sky/skylet/attempt_skylet.py
 sky/skylet/autostop_lib.py
 sky/skylet/configs.py
@@ -172,14 +175,15 @@
 skypilot_nightly.egg-info/dependency_links.txt
 skypilot_nightly.egg-info/entry_points.txt
 skypilot_nightly.egg-info/requires.txt
 skypilot_nightly.egg-info/top_level.txt
 tests/test_cli.py
 tests/test_config.py
 tests/test_global_user_state.py
+tests/test_jobs.py
 tests/test_list_accelerators.py
 tests/test_onprem.py
 tests/test_optimizer_dryruns.py
 tests/test_optimizer_random_dag.py
 tests/test_pycryptodome_version.py
 tests/test_smoke.py
 tests/test_spot.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230715/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tempfile
 import textwrap
 
 from click import testing as cli_testing
 
 import sky
+from sky import exceptions
 import sky.cli as cli
 
 CLOUDS_TO_TEST = ['aws', 'gcp', 'ibm', 'azure', 'lambda', 'scp', 'oci']
 
 
 def test_infer_gpunode_type():
     resources = [
@@ -50,15 +51,15 @@
           cloud: aws
           instance_type: p3.2xlarge""")
     cli_runner = cli_testing.CliRunner()
 
     def _capture_mismatch_gpus_spec(file_path, gpus: str):
         result = cli_runner.invoke(cli.launch,
                                    [file_path, '--gpus', gpus, '--dryrun'])
-        assert isinstance(result.exception, ValueError)
+        assert isinstance(result.exception, exceptions.ResourcesMismatchError)
         assert 'Infeasible resource demands found:' in str(result.exception)
 
     def _capture_match_gpus_spec(file_path, gpus: str):
         result = cli_runner.invoke(cli.launch,
                                    [file_path, '--gpus', gpus, '--dryrun'])
         assert not result.exit_code
 
@@ -66,18 +67,18 @@
         f.write(spec)
         f.flush()
 
         _capture_mismatch_gpus_spec(f.name, 'T4:1')
         _capture_mismatch_gpus_spec(f.name, 'T4:0.5')
         _capture_mismatch_gpus_spec(f.name, 'V100:2')
         _capture_mismatch_gpus_spec(f.name, 'v100:2')
+        _capture_mismatch_gpus_spec(f.name, 'V100:0.5')
 
         _capture_match_gpus_spec(f.name, 'V100:1')
         _capture_match_gpus_spec(f.name, 'v100:1')
-        _capture_match_gpus_spec(f.name, 'V100:0.5')
         _capture_match_gpus_spec(f.name, 'V100')
 
 
 def test_show_gpus():
     """
     This is a test suite for `sky show-gpus` to check functionality (but not correctness).
     The tests below correspond to the following terminal commands,
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_dryruns.py`

 * *Files 6% similar despite different names*

```diff
@@ -325,36 +325,66 @@
     bad_instance_and_accs = [
         # Actual: V100
         ('p3.2xlarge', 'K80'),
         # Actual: None
         ('m4.2xlarge', 'V100'),
     ]
     for instance, acc in bad_instance_and_accs:
-        with pytest.raises(ValueError) as e:
+        with pytest.raises(exceptions.ResourcesMismatchError) as e:
             _test_resources_launch(monkeypatch,
                                    sky.AWS(),
                                    instance_type=instance,
                                    accelerators=acc)
         assert 'Infeasible resource demands found' in str(e.value)
 
+    with pytest.raises(exceptions.ResourcesMismatchError) as e:
+        _test_resources_launch(monkeypatch,
+                               sky.GCP(),
+                               instance_type='n2-standard-8',
+                               accelerators={'V100': 1})
+        assert 'can only be attached to N1 VMs,' in str(e.value), str(e.value)
+
+    with pytest.raises(exceptions.ResourcesMismatchError) as e:
+        _test_resources_launch(monkeypatch,
+                               sky.GCP(),
+                               instance_type='a2-highgpu-1g',
+                               accelerators={'A100': 2})
+        assert 'cannot be attached to' in str(e.value), str(e.value)
+
+    with pytest.raises(exceptions.ResourcesMismatchError) as e:
+        _test_resources_launch(monkeypatch,
+                               sky.AWS(),
+                               instance_type='p3.16xlarge',
+                               accelerators={'V100': 1})
+        assert 'Infeasible resource demands found' in str(e.value)
+
 
 def test_instance_type_matches_accelerators(monkeypatch):
     _test_resources_launch(monkeypatch,
                            sky.AWS(),
                            instance_type='p3.2xlarge',
                            accelerators='V100')
     _test_resources_launch(monkeypatch,
                            sky.GCP(),
                            instance_type='n1-standard-2',
                            accelerators='V100')
-    # Partial use: Instance has 8 V100s, while the task needs 1 of them.
+
+    _test_resources_launch(monkeypatch,
+                           sky.GCP(),
+                           instance_type='n1-standard-8',
+                           accelerators='tpu-v3-8')
+    _test_resources_launch(monkeypatch,
+                           sky.GCP(),
+                           instance_type='a2-highgpu-1g',
+                           accelerators='a100')
+
     _test_resources_launch(monkeypatch,
                            sky.AWS(),
                            instance_type='p3.16xlarge',
-                           accelerators={'V100': 1})
+                           accelerators={'V100': 8})
 
 
 def test_invalid_instance_type(monkeypatch):
     for cloud in [sky.AWS(), sky.Azure(), sky.GCP(), None]:
         with pytest.raises(ValueError) as e:
             _test_resources(monkeypatch, cloud, instance_type='invalid')
         assert 'Invalid instance type' in str(e.value)
@@ -398,14 +428,21 @@
 
 def test_invalid_region(monkeypatch):
     for cloud in [sky.AWS(), sky.Azure(), sky.GCP()]:
         with pytest.raises(ValueError) as e:
             _test_resources(monkeypatch, cloud, region='invalid')
         assert 'Invalid region' in str(e.value)
 
+    with pytest.raises(exceptions.ResourcesUnavailableError) as e:
+        _test_resources_launch(monkeypatch,
+                               sky.GCP(),
+                               region='us-west1',
+                               accelerators='tpu-v3-8')
+        assert 'No launchable resource found' in str(e.value)
+
 
 def test_invalid_zone(monkeypatch):
     for cloud in [sky.AWS(), sky.GCP()]:
         with pytest.raises(ValueError) as e:
             _test_resources(monkeypatch, cloud, zone='invalid')
         assert 'Invalid zone' in str(e.value)
 
@@ -595,7 +632,20 @@
     spec = textwrap.dedent("""\
         envs:
           hello_world: 1
           HELLO: val
           GOOD123: 123
         """)
     _test_parse_task_yaml(spec)
+
+
+def test_invalid_accelerators_regions(enable_all_clouds, monkeypatch):
+    task = sky.Task(run='echo hi')
+    task.set_resources(
+        sky.Resources(
+            sky.AWS(),
+            accelerators='A100:8',
+            region='us-west-1',
+        ))
+    with pytest.raises(exceptions.ResourcesUnavailableError) as e:
+        sky.launch(task, cluster_name='should-fail', dryrun=True)
+        assert 'No launchable resource found for' in str(e.value), str(e.value)
```

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230714/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230715/tests/test_wheels.py`

 * *Files identical despite different names*

