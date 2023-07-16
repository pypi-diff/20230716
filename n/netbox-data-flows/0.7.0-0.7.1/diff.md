# Comparing `tmp/netbox-data-flows-0.7.0.tar.gz` & `tmp/netbox-data-flows-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-data-flows-0.7.0.tar", last modified: Tue Jul  4 16:23:31 2023, max compression
+gzip compressed data, was "netbox-data-flows-0.7.1.tar", last modified: Sun Jul 16 17:59:53 2023, max compression
```

## Comparing `netbox-data-flows-0.7.0.tar` & `netbox-data-flows-0.7.1.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/addins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/filtersets/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/forms/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/graphql/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.555177 netbox-data-flows-0.7.0/netbox_data_flows/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.559177 netbox-data-flows-0.7.0/netbox_data_flows/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0002_alter_objectalias_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0007_remove_objectalias_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.559177 netbox-data-flows-0.7.0/netbox_data_flows/models/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/models/objectaliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.559177 netbox-data-flows-0.7.0/netbox_data_flows/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/tables/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/application.html
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/netbox_data_flows/views/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/applicationroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/dataflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/model_tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/netbox_data_flows/views/objectaliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 16:23:31.551177 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 16:23:31.000000 netbox-data-flows-0.7.0/netbox_data_flows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-04 16:23:14.000000 netbox-data-flows-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 16:23:31.563177 netbox-data-flows-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.632483 netbox-data-flows-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-16 17:59:53.632483 netbox-data-flows-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/addins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/filtersets/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/forms/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/graphql/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.624482 netbox-data-flows-0.7.1/netbox_data_flows/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/management/commands/delete_orphaned_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0002_alter_objectalias_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0005_dataflowgroup_slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0007_remove_objectalias_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/models/objectaliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/tables/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/application.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/applicationrole.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/inc/objectaliastarget_actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.628482 netbox-data-flows-0.7.1/netbox_data_flows/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/applicationroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/dataflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/model_tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/netbox_data_flows/views/objectaliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 17:59:53.620483 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 17:59:53.000000 netbox-data-flows-0.7.1/netbox_data_flows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-16 17:59:33.000000 netbox-data-flows-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 17:59:53.632483 netbox-data-flows-0.7.1/setup.cfg
```

### Comparing `netbox-data-flows-0.7.0/LICENSE` & `netbox-data-flows-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/PKG-INFO` & `netbox-data-flows-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.7.0
+Version: 0.7.1
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.7.0/README.md` & `netbox-data-flows-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/__init__.py` & `netbox-data-flows-0.7.1/netbox_data_flows/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginConfig
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 
 class DataFlowsConfig(PluginConfig):
     name = "netbox_data_flows"
     verbose_name = "Data Flows"
     description = (
         "NetBox plugin to document data flows between "
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/dataflows.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/groups.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/nested.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/nested.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/serializers/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/serializers/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/urls.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/api/views.py` & `netbox-data-flows-0.7.1/netbox_data_flows/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/choices.py` & `netbox-data-flows-0.7.1/netbox_data_flows/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/addins.py` & `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/addins.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/dataflows.py` & `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/filters.py` & `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/groups.py` & `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/filtersets/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/filtersets/objectaliases.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,17 @@
         return queryset
 
     def filter_devices(self, queryset, name, value):
         if not value:
             return queryset
 
         ip_addresses = get_device_ipaddresses(*value)
+        if not ip_addresses.exists():
+            return queryset.none()
+
         return self.filter_targets(queryset, name, ip_addresses)
 
     # OR all the targets
     # First, build a list
     def filter_targets(self, queryset, name, value):
         if not value:
             return queryset
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/forms/applicationroles.py` & `netbox-data-flows-0.7.1/netbox_data_flows/forms/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/forms/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/forms/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/forms/dataflows.py` & `netbox-data-flows-0.7.1/netbox_data_flows/forms/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/forms/groups.py` & `netbox-data-flows-0.7.1/netbox_data_flows/forms/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
     class Meta:
         model = models.DataFlowGroup
         fields = (
             "application",
             "parent",
             "name",
+            "slug",
             "description",
             "status",
             "comments",
             "tags",
         )
         help_texts = {
             "status": (
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/forms/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/forms/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/graphql/__init__.py` & `netbox-data-flows-0.7.1/netbox_data_flows/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/graphql/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/graphql/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/graphql/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/graphql/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/management/commands/delete_orphaned_aliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/management/commands/delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0001_initial.py` & `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py` & `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0005_dataflowgroup_slug.py` & `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0005_dataflowgroup_slug.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/migrations/0008_delete_orphaned_aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/models/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/models/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/models/dataflows.py` & `netbox-data-flows-0.7.1/netbox_data_flows/models/dataflows.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.contrib.postgres.fields import ArrayField
-from django.core.exceptions import ValidationError
 from django.core.validators import MaxValueValidator, MinValueValidator
 from django.db import models
 from django.urls import reverse
 from django.utils.functional import cached_property
 
 from netbox.models import NetBoxModel
 from utilities.querysets import RestrictedQuerySet
@@ -214,27 +213,7 @@
     )
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse("plugins:netbox_data_flows:dataflow", args=[self.pk])
-
-    def clean(self):
-        super().clean()
-
-        if self.group and self.group.application != self.application:
-            if not self.application:
-                self.application = self.group.application
-            else:
-                raise ValidationError(
-                    {
-                        "application": (
-                            "The application of the data flow must match "
-                            "the application of its group."
-                        ),
-                        "group": (
-                            "The application of the group must match the "
-                            "application of the data flow."
-                        ),
-                    }
-                )
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/models/groups.py` & `netbox-data-flows-0.7.1/netbox_data_flows/models/groups.py`

 * *Files 19% similar despite different names*

```diff
@@ -108,38 +108,14 @@
     objects = DataFlowGroupManager()
 
     def get_absolute_url(self):
         return reverse(
             "plugins:netbox_data_flows:dataflowgroup", args=[self.pk]
         )
 
-    def clean(self):
-        super().clean()
-
-        if self.parent and self.parent.application != self.application:
-            if not self.application:
-                self.application = self.parent.application
-            else:
-                raise ValidationError(
-                    {
-                        "application": (
-                            "The application of the data flow must match "
-                            "the application of its parent."
-                        ),
-                        "parent": (
-                            "The application of the parent must match the "
-                            "application of the data flow."
-                        ),
-                    }
-                )
-
-        # update all our descendants' application
-        if self.pk:
-            self.get_descendants().update(application_id=self.application)
-
     def validate_unique(self, exclude=None):
         if self.parent is None:
             groups = self.__class__.objects.exclude(pk=self.pk)
             if groups.filter(
                 name=self.name,
                 application=self.application,
                 parent__isnull=True,
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/models/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/models/objectaliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 
 class ObjectAliasTargetQuerySet(RestrictedQuerySet):
     def contains(self, *objects):
         """
         Return ObjectAliasTarget containing any one of the objects in parameter
         """
+        ip_ct = ContentType.objects.get_for_model(IPAddress)
 
         if not objects:
             return self.none()
 
         query = models.Q()
         for t in objects:
             ct = ContentType.objects.get_for_model(t.__class__)
@@ -54,21 +55,17 @@
                 try:
                     ip_addresses = get_device_ipaddresses(t)
                 except Exception as e:
                     raise Exception(
                         f"Cannot test if {self.__class__} contains {t}"
                     ) from e
 
-                if ip_addresses:
-                    ip_ct = ContentType.objects.get_for_model(
-                        ip_addresses[0].__class__
-                    )
-
-                    for ip in ip_addresses:
-                        query |= models.Q(target_type=ip_ct, target_id=ip.pk)
+                query |= models.Q(
+                    target_type=ip_ct, target_id__in=ip_addresses
+                )
 
         return self.filter(query)
 
 
 class ObjectAliasTarget(models.Model):
     """
     A single prefix, range or IP address to be used in ObjectAlias.
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/navigation.py` & `netbox-data-flows-0.7.1/netbox_data_flows/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/search.py` & `netbox-data-flows-0.7.1/netbox_data_flows/search.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/tables/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/tables/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/tables/dataflows.py` & `netbox-data-flows-0.7.1/netbox_data_flows/tables/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/tables/groups.py` & `netbox-data-flows-0.7.1/netbox_data_flows/tables/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/tables/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/tables/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/application.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/application.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/applicationrole.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/applicationrole.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_list.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_tab.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflow_targets.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/dataflowgroup.html`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,26 @@
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Data Flow Group</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
             <tr>
+              <th scope="row">Name</th>
+              <td>
+                {{ object.name }}
+              </td>
+            </tr>
+            <tr>
+              <th scope="row">Slug</th>
+              <td>
+                {{ object.slug }}
+              </td>
+            </tr>
+            <tr>
               <th scope="row">Application</th>
               <td>{{ object.application|linkify }}</td>
             </tr>
             <tr>
               <th scope="row">Description</th>
               <td>{{ object.description|placeholder }}</td>
             </tr>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load helpers %} {%
 load perms %} {% load plugins %} {% load render_table from django_tables2 %} {%
 block breadcrumbs %} {{ block.super }}
 {{_object.application_}}
 {% endblock %} {% block content %}
 ** Data Flow Group **
+Name        {{ object.name }}
+Slug        {{ object.slug }}
 Application {{ object.application|linkify }}
 Description {{ object.description|placeholder }}
 Status      {% badge object.inherited_status_display
             bg_color=object.get_status_color %}
 Parent      {{ object.parent|placeholder|linkify }}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html` & `netbox-data-flows-0.7.1/netbox_data_flows/templates/netbox_data_flows/objectalias_removetarget.html`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/urls.py` & `netbox-data-flows-0.7.1/netbox_data_flows/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/utils/aliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/utils/helpers.py` & `netbox-data-flows-0.7.1/netbox_data_flows/utils/helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import itertools
+from django.contrib.contenttypes.models import ContentType
+
+from ipam.models import IPAddress
 
 from django.db.models import Q
 from django.utils.safestring import mark_safe
 
 
 def object_list_to_string(
     objects, *, linkify=False, default="", separator=", "
@@ -27,27 +29,40 @@
     qs = Q()
     for app_label, model in models:
         qs |= Q(app_label=app_label, model=model)
 
     return Q(qs)
 
 
+def _get_ip_qs(device):
+    """
+    Return a querystring matching any IP assigned to the device
+    """
+
+    interfaces = device.interfaces.all()
+    ct = ContentType.objects.get_for_model(interfaces.model)
+
+    return Q(
+        assigned_object_type=ct.pk,
+        assigned_object_id__in=interfaces,
+    )
+
+
+def get_one_device_ipaddresses(device):
+    """
+    Return the list of IP addresses of a device or virtual machine
+    """
+
+    ip_qs = _get_ip_qs(device)
+    return IPAddress.objects.filter(ip_qs)
+
+
 def get_device_ipaddresses(*devices):
     """
     Return the list of IP addresses of a list of devices or virtual machines
     """
 
-    interfaces = []
+    qs = Q()
     for dev in devices:
-        if hasattr(dev, "vc_interfaces"):
-            # Device
-            interfaces += [dev.vc_interfaces(if_master=False)]
-        else:
-            # Virtual Machine
-            interfaces += [dev.interfaces.all()]
-
-    interfaces = itertools.chain.from_iterable(interfaces)
-    ip_addresses = itertools.chain.from_iterable(
-        ifce.ip_addresses.all() for ifce in interfaces
-    )
-    ip_addresses = list(ip_addresses)
-    return ip_addresses
+        qs |= _get_ip_qs(dev)
+
+    return IPAddress.objects.filter(qs)
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/views/applicationroles.py` & `netbox-data-flows-0.7.1/netbox_data_flows/views/applicationroles.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/views/applications.py` & `netbox-data-flows-0.7.1/netbox_data_flows/views/applications.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/views/dataflows.py` & `netbox-data-flows-0.7.1/netbox_data_flows/views/dataflows.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/views/groups.py` & `netbox-data-flows-0.7.1/netbox_data_flows/views/groups.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/views/model_tabs.py` & `netbox-data-flows-0.7.1/netbox_data_flows/views/model_tabs.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows/views/objectaliases.py` & `netbox-data-flows-0.7.1/netbox_data_flows/views/objectaliases.py`

 * *Files identical despite different names*

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows.egg-info/PKG-INFO` & `netbox-data-flows-0.7.1/netbox_data_flows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-data-flows
-Version: 0.7.0
+Version: 0.7.1
 Summary: NetBox plugin to document data flows between systems and applications.
 Author: Thomas Fargeix
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Alef-Burzmali/netbox-data-flows
 Project-URL: Bug Tracker, https://github.com/Alef-Burzmali/netbox-data-flows/issues
 Keywords: netbox,netbox-plugins
 Classifier: Development Status :: 4 - Beta
```

### Comparing `netbox-data-flows-0.7.0/netbox_data_flows.egg-info/SOURCES.txt` & `netbox-data-flows-0.7.1/netbox_data_flows.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 netbox_data_flows/migrations/0002_alter_objectalias_options.py
 netbox_data_flows/migrations/0003_alter_application_custom_field_data_and_more.py
 netbox_data_flows/migrations/0004_reindex_netbox_data_flows.py
 netbox_data_flows/migrations/0005_dataflowgroup_slug.py
 netbox_data_flows/migrations/0006_reindex_netbox_data_flows.py
 netbox_data_flows/migrations/0007_remove_objectalias_size.py
 netbox_data_flows/migrations/0008_delete_orphaned_aliases.py
+netbox_data_flows/migrations/0009_fix_empty_dfg_slugs.py
 netbox_data_flows/migrations/__init__.py
 netbox_data_flows/models/__init__.py
 netbox_data_flows/models/applications.py
 netbox_data_flows/models/dataflows.py
 netbox_data_flows/models/groups.py
 netbox_data_flows/models/objectaliases.py
 netbox_data_flows/tables/__init__.py
```

### Comparing `netbox-data-flows-0.7.0/pyproject.toml` & `netbox-data-flows-0.7.1/pyproject.toml`

 * *Files identical despite different names*

