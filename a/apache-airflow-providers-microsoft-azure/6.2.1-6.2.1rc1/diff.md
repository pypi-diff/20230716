# Comparing `tmp/apache-airflow-providers-microsoft-azure-6.2.1.tar.gz` & `tmp/apache-airflow-providers-microsoft-azure-6.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-azure-6.2.1.tar", last modified: Wed Jul 12 19:10:19 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-azure-6.2.1rc1.tar", last modified: Wed Jul 12 19:13:31 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-azure-6.2.1.tar` & `apache-airflow-providers-microsoft-azure-6.2.1rc1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.361877 apache-airflow-providers-microsoft-azure-6.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:10:18.000000 apache-airflow-providers-microsoft-azure-6.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6589 2023-07-12 19:10:19.362458 apache-airflow-providers-microsoft-azure-6.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4851 2023-07-12 19:10:18.000000 apache-airflow-providers-microsoft-azure-6.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.151198 apache-airflow-providers-microsoft-azure-6.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.152334 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.153524 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.206462 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-12 19:08:31.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.215093 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py
--rw-r--r--   0 root         (0) root         (0)    17536 2023-07-12 19:10:17.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.255721 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8759 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0 root         (0) root         (0)    15302 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0 root         (0) root         (0)     6183 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0 root         (0) root         (0)     4062 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    44145 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0 root         (0) root         (0)    22133 2023-06-28 06:26:40.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0 root         (0) root         (0)    13004 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0 root         (0) root         (0)    29495 2023-07-12 17:52:12.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.261622 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10038 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.289994 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0 root         (0) root         (0)    29255 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0 root         (0) root         (0)    16254 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)    15968 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0 root         (0) root         (0)    12525 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0 root         (0) root         (0)     2687 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.295508 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7891 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/secrets/key_vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.309892 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0 root         (0) root         (0)     5896 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     8065 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.327148 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-07-09 14:40:47.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     4817 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0 root         (0) root         (0)     8202 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.335555 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11197 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0 root         (0) root         (0)     7382 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0 root         (0) root         (0)     2821 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:19.359198 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6589 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3152 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      604 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:10:19.000000 apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-microsoft-azure-6.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2457 2023-07-12 19:10:19.364332 apache-airflow-providers-microsoft-azure-6.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-12 19:10:17.000000 apache-airflow-providers-microsoft-azure-6.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.581397 apache-airflow-providers-microsoft-azure-6.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-12 19:13:31.581936 apache-airflow-providers-microsoft-azure-6.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4854 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.377077 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.378193 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.379220 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.423358 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-12 19:08:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.432138 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-04 06:09:02.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py
+-rw-r--r--   0 root         (0) root         (0)    17536 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.473019 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8759 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0 root         (0) root         (0)    15302 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0 root         (0) root         (0)     6183 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0 root         (0) root         (0)     4062 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    44145 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)    22133 2023-06-28 06:26:40.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0 root         (0) root         (0)    13004 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0 root         (0) root         (0)    29495 2023-07-12 17:52:12.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.478925 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.507784 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0 root         (0) root         (0)    29255 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0 root         (0) root         (0)    16254 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)    15968 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-06-20 06:40:52.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.513580 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7891 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.524663 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8065 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.541506 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-07-09 14:40:47.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0 root         (0) root         (0)     8202 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.550009 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11197 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7382 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-07-05 07:19:39.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:31.578400 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      609 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:31.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-07-12 19:13:31.583989 apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-12 19:13:30.000000 apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/LICENSE` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/MANIFEST.in` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.2.1
+Version: 6.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.2.1``
+Release: ``6.2.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/README.rst` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.2.1``
+Release: ``6.2.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_cosmos_document_sensor.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/example_dag/example_wasb_sensors.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/get_provider_info.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/adx.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/asb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/batch.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/log/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/adls.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/adx.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/asb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/batch.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/synapse.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/airflow/providers/microsoft/azure/utils.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 6.2.1
+Version: 6.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-azure package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-azure/6.2.1/
@@ -69,15 +69,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``6.2.1``
+Release: ``6.2.1rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/apache_airflow_providers_microsoft_azure.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 adal>=1.2.7
-apache-airflow>=2.4.0
+apache-airflow>=2.4.0.dev0
 azure-batch>=8.0.0
 azure-cosmos>=4.0.0
 azure-datalake-store>=0.0.45
 azure-identity>=1.3.1
 azure-keyvault-secrets>=4.1.0
 azure-kusto-data<0.1,>=0.0.43
 azure-mgmt-containerinstance<2.0,>=1.5.0
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/pyproject.toml` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/setup.cfg` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	adal>=1.2.7
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	azure-batch>=8.0.0
 	azure-cosmos>=4.0.0
 	azure-datalake-store>=0.0.45
 	azure-identity>=1.3.1
 	azure-keyvault-secrets>=4.1.0
 	azure-kusto-data>=0.0.43,<0.1
 	azure-mgmt-containerinstance>=1.5.0,<2.0
@@ -70,10 +70,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.azure.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.azure
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-azure-6.2.1/setup.py` & `apache-airflow-providers-microsoft-azure-6.2.1rc1/setup.py`

 * *Files identical despite different names*

