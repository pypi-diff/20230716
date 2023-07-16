# Comparing `tmp/domain-admin-1.5.0.tar.gz` & `tmp/domain-admin-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.5.0.tar", last modified: Sun Jul 16 03:30:36 2023, max compression
+gzip compressed data, was "domain-admin-1.5.1.tar", last modified: Sun Jul 16 13:46:09 2023, max compression
```

## Comparing `domain-admin-1.5.0.tar` & `domain-admin-1.5.1.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.847051 domain-admin-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-16 03:30:22.000000 domain-admin-1.5.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-16 03:30:22.000000 domain-admin-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-16 03:30:36.843051 domain-admin-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16712 2023-07-16 03:30:22.000000 domain-admin-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.819051 domain-admin-1.5.0/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/domain_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/group_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/log_operation_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/api/whois_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.819051 domain-admin-1.5.0/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/config/default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/config/env_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/config/runtime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.819051 domain-admin-1.5.0/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/config_key_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/event_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/operation_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/role_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.819051 domain-admin-1.5.0/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_1213_to_131.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_136_to_140_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_140_alpha_to_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_1413_to_1414.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_1422_to_1423.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_143_to_144.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_145_to_146.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/migrate/migrate_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.819051 domain-admin-1.5.0/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/group_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/log_operation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.819051 domain-admin-1.5.0/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.811051 domain-admin-1.5.0/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.811051 domain-admin-1.5.0/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.811051 domain-admin-1.5.0/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/11/
--r--r--r--   0 runner    (1001) docker     (123)     3180 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/11/e53e58b56342d3ed07f7ad82094209a85110d0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/19/
--r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/24/
--r--r--r--   0 runner    (1001) docker     (123)     6153 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/24/933b4eedb8202eacc8a8dc76466bb8ff28efcd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/2a/
--r--r--r--   0 runner    (1001) docker     (123)      223 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/2a/495a2b7d8f5ff034faec7f33caab9440ed4304
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/33/
--r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/33/ea7b19add95fae6c823919ab86c3bcdcf87307
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/35/
--r--r--r--   0 runner    (1001) docker     (123)      247 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/35/eeddd87c8cb15685d288c8eda40c337c7d5667
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/3c/
--r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/3f/
--r--r--r--   0 runner    (1001) docker     (123)    81098 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/3f/9f711ce627c122b8c70ac9300d1d5a046c4690
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/52/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/55/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/5f/
--r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/67/
--r--r--r--   0 runner    (1001) docker     (123)    33934 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/67/e95e36239b9f21e0c968cde274e1c8074caa0f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/6c/
--r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/71/
--r--r--r--   0 runner    (1001) docker     (123)     9377 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/71/01c7e7cd243bb0c4a7caf901ce1005911a8432
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/7a/1141eeeacfc2052b0496001fffad61c6672ffd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/7f/
--r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/85/
--r--r--r--   0 runner    (1001) docker     (123)     1735 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/85/d5b39f098d01c9dbc10214df393ab55c5c5685
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/89/
--r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/8c/
--r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/94/
--r--r--r--   0 runner    (1001) docker     (123)     1699 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/94/8be774e1f2613f4fa1b82ae88043ef92d70761
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.823051 domain-admin-1.5.0/domain_admin/public/.git/objects/9a/
--r--r--r--   0 runner    (1001) docker     (123)      757 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/9a/4957917630d72546f62ab236f9e916c0e8670b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/a0/
--r--r--r--   0 runner    (1001) docker     (123)      465 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/a0/b8ee977ea74de0720a00aad1b41570c2488aea
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/ab/
--r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/ab/b5db9b4b7005df3a44582c0e992b3a1da365cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/b3/
--r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/b6/
--r--r--r--   0 runner    (1001) docker     (123)   365904 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/b6/81b7d87ead80778d68ff251ed7f9a2dde0950a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/be/
--r--r--r--   0 runner    (1001) docker     (123)     1896 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/be/4d5a11a24cb52c5bc6ad7cb0f0cba03770565d
--r--r--r--   0 runner    (1001) docker     (123)      475 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/be/a294c5fea5d8882221f1810c2f6d85827a062b
--r--r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/be/c3dc9a28420fa1fbb7115f5acb47dc690dd4db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/bf/
--r--r--r--   0 runner    (1001) docker     (123)    10076 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/bf/6e10bcc54e0b8256bb0a7bbe2cdb0c2384db91
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/c0/
--r--r--r--   0 runner    (1001) docker     (123)     8843 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/c0/5315f3d882bac87d0845ebd85af8097c722b5f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/c4/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/cb/
--r--r--r--   0 runner    (1001) docker     (123)      229 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/cb/f418bdf2a49f64c14ebe734fb6d6dce4c00366
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/da/
--r--r--r--   0 runner    (1001) docker     (123)     1025 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/da/6a99e6a186e30a655b7b7082699da9e6dc557f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/e1/
--r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/fb/
--r--r--r--   0 runner    (1001) docker     (123)   156723 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/fb/d49bf5e92b08848a3c75b285c90c0100d7b440
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/objects/ff/
--r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.811051 domain-admin-1.5.0/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.811051 domain-admin-1.5.0/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/css/index.563210a3.css
--rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/css/index.69a97337.css
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/css/index.a676cc2e.css
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/css/index.b285e10a.css
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/css/index.d028ae37.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/gif/
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/gif/user-avatar.ea67286d.gif
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.827051 domain-admin-1.5.0/domain_admin/public/jpg/
--rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/jpg/chatpet.fce5580e.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.831051 domain-admin-1.5.0/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/ConditionFilterGroup.98203553.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/ConnectStatus.afc51e5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/SelectGroup.c4ef5dae.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/element-icon.1ce1c350.js
--rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/element-plus.c20bc0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/event-enums.6c6f25e7.js
--rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.18819e48.js
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.1a48d33b.js
--rw-r--r--   0 runner    (1001) docker     (123)    30256 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.4846c617.js
--rw-r--r--   0 runner    (1001) docker     (123)   419180 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.5aa6512c.js
--rw-r--r--   0 runner    (1001) docker     (123)    21906 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.730c57dc.js
--rw-r--r--   0 runner    (1001) docker     (123)  1068448 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.a12c098a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.b5155817.js
--rw-r--r--   0 runner    (1001) docker     (123)   255125 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.c5fb6f8c.js
--rw-r--r--   0 runner    (1001) docker     (123)    94070 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.deda20cc.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.e036cf3b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.f2a38d9e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/index.fd336ece.js
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/vendor-lib.cb4f08bf.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/js/vendor-vue.9e61e0af.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.831051 domain-admin-1.5.0/domain_admin/public/m/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/m/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin/public/m/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin/public/m/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/2d/
--r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/43/
--r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/4b/
--r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/5c/
--r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/61/
--r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/62/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/67/
--r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/6f/
--r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/71/
--r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
--r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/8e/
--r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
--r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/98/
--r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/a9/
--r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/b0/
--r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/c2/
--r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/c7/
--r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/c8/
--r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/d9/
--r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/ed/
--r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/f0/
--r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/f8/
--r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/objects/fd/
--r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin/public/m/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.835051 domain-admin-1.5.0/domain_admin/public/m/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin/public/m/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.839051 domain-admin-1.5.0/domain_admin/public/m/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.839051 domain-admin-1.5.0/domain_admin/public/m/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/common-c7dd5d89.css
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/common.6194c42f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index-5eda257b.css
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index-958ae3a0.css
--rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index-9c365a03.js
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index-ad047368.css
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index-e8224928.css
--rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index-f79acb3d.css
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index.1a0d1182.js
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index.1d067866.js
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index.daaf9893.js
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/index.feef7c0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/login-cb9f43ad.css
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/pages-login-login.09426b90.js
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/uni.06dd3c8e.css
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/assets/user-index-be7005ab.css
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.839051 domain-admin-1.5.0/domain_admin/public/m/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-16 03:30:35.000000 domain-admin-1.5.0/domain_admin/public/m/static/user-avatar.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.839051 domain-admin-1.5.0/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-16 03:30:34.000000 domain-admin-1.5.0/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.839051 domain-admin-1.5.0/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.839051 domain-admin-1.5.0/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/common_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/group_user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/operation_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/service/version_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/templates/cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/templates/cert-export.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/templates/domain-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/cert_openssl_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/icp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/md5_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/open_api/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/open_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/open_api/crtsh_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/open_api/ding_talk_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/open_api/feishu_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/open_api/work_weixin_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/utils/whois_util/whois_util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-16 03:30:22.000000 domain-admin-1.5.0/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.815051 domain-admin-1.5.0/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-16 03:30:36.000000 domain-admin-1.5.0/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-16 03:30:36.000000 domain-admin-1.5.0/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:30:36.000000 domain-admin-1.5.0/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-16 03:30:36.000000 domain-admin-1.5.0/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 03:30:36.000000 domain-admin-1.5.0/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 03:30:36.000000 domain-admin-1.5.0/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 03:30:36.843051 domain-admin-1.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-16 03:30:22.000000 domain-admin-1.5.0/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 03:30:36.847051 domain-admin-1.5.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-16 03:30:22.000000 domain-admin-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-16 13:45:57.000000 domain-admin-1.5.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-07-16 13:45:57.000000 domain-admin-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-07-16 13:46:09.497462 domain-admin-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16721 2023-07-16 13:45:57.000000 domain-admin-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.465461 domain-admin-1.5.1/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.465461 domain-admin-1.5.1/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14762 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/domain_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/group_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/log_operation_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/api/whois_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.465461 domain-admin-1.5.1/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/config/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/config/runtime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.469461 domain-admin-1.5.1/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/config_key_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/event_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/operation_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/role_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.469461 domain-admin-1.5.1/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_1213_to_131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_136_to_140_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_140_alpha_to_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_1413_to_1414.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_1422_to_1423.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_143_to_144.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_145_to_146.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/migrate/migrate_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.469461 domain-admin-1.5.1/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/group_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/log_operation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.469461 domain-admin-1.5.1/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.469461 domain-admin-1.5.1/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-16 13:46:06.000000 domain-admin-1.5.1/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.457460 domain-admin-1.5.1/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.457460 domain-admin-1.5.1/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/05/
+-r--r--r--   0 runner    (1001) docker     (123)     1699 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/05/4a020e56d7af80d0110b8500a034ea21c16a9c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/0e/
+-r--r--r--   0 runner    (1001) docker     (123)    81110 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/0e/0f1ee6c217e5da4bd965f2d9ce0ab2cac11e03
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/19/
+-r--r--r--   0 runner    (1001) docker     (123)    64350 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/1b/
+-r--r--r--   0 runner    (1001) docker     (123)      694 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/1b/3eab78b7dfba767ded92178c81c404f5c21052
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/1d/
+-r--r--r--   0 runner    (1001) docker     (123)     1739 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/1d/3e7887c6d2b61648a0ec4ae187a97314a3d9a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/2b/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/2b/5704558111e371903e48b7fedf70d24dad55bf
+-r--r--r--   0 runner    (1001) docker     (123)     1025 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/2b/879e31c999b53e51dbbb528db102aac5a0ddb5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/33/
+-r--r--r--   0 runner    (1001) docker     (123)   279936 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/33/ea7b19add95fae6c823919ab86c3bcdcf87307
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/35/
+-r--r--r--   0 runner    (1001) docker     (123)      247 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/35/eeddd87c8cb15685d288c8eda40c337c7d5667
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/3c/
+-r--r--r--   0 runner    (1001) docker     (123)     3081 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/41/
+-r--r--r--   0 runner    (1001) docker     (123)     3179 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/41/b5605e3f03a272f1f17c91a1c9203df59a19d6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/51/
+-r--r--r--   0 runner    (1001) docker     (123)     9378 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/51/b89a9c3bf4fb6075399ba7bacc0f1594493956
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/52/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/55/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/5f/
+-r--r--r--   0 runner    (1001) docker     (123)      530 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/6c/
+-r--r--r--   0 runner    (1001) docker     (123)      155 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/7f/
+-r--r--r--   0 runner    (1001) docker     (123)      368 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/84/
+-r--r--r--   0 runner    (1001) docker     (123)     6154 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/84/155baa6831b822324d3b71d53c2da8e799e6ad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/89/
+-r--r--r--   0 runner    (1001) docker     (123)      106 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/8c/
+-r--r--r--   0 runner    (1001) docker     (123)       69 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.473461 domain-admin-1.5.1/domain_admin/public/.git/objects/a0/
+-r--r--r--   0 runner    (1001) docker     (123)   365903 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/a0/0aeea345a67ff29a66605c34e468c397bcecf6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/ad/
+-r--r--r--   0 runner    (1001) docker     (123)      465 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/ad/f592e42021579d5e29d616ab778f5549b949a7
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/b3/
+-r--r--r--   0 runner    (1001) docker     (123)    41902 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/b8/
+-r--r--r--   0 runner    (1001) docker     (123)     5817 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/b8/bbbb563dcaa4e5e8a878d603dcc0821eadb842
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/be/
+-r--r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/be/c3dc9a28420fa1fbb7115f5acb47dc690dd4db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/bf/
+-r--r--r--   0 runner    (1001) docker     (123)    10076 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/bf/6e10bcc54e0b8256bb0a7bbe2cdb0c2384db91
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/c4/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/d9/
+-r--r--r--   0 runner    (1001) docker     (123)     1894 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/d9/04d142c9bf7ef514a7a46daf1a1a63daffb3ec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/df/
+-r--r--r--   0 runner    (1001) docker     (123)      228 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/df/90cac9bc9a446000e264e59d549b7b0144fbdc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/e1/
+-r--r--r--   0 runner    (1001) docker     (123)    23927 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/e2/
+-r--r--r--   0 runner    (1001) docker     (123)     8845 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/e2/ae3e466505ab377291c9bc893b36ea4e4cc346
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/ea/
+-r--r--r--   0 runner    (1001) docker     (123)   156724 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/ea/014768708683bab0f086bbe7bbbee4bd721482
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/f1/
+-r--r--r--   0 runner    (1001) docker     (123)    33933 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/f1/d1775a53fb6d01f3cf868d7675175acb4972e5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/fa/
+-r--r--r--   0 runner    (1001) docker     (123)      760 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/fa/b7c448af6beaf517ef73175a858b241978b57d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/objects/ff/
+-r--r--r--   0 runner    (1001) docker     (123)      474 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/ff/3abe67801fd71004bf50541b8e22677539048b
+-r--r--r--   0 runner    (1001) docker     (123)    13943 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/css/index.563210a3.css
+-rw-r--r--   0 runner    (1001) docker     (123)   331526 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/css/index.69a97337.css
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/css/index.a676cc2e.css
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/css/index.b285e10a.css
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/css/index.d028ae37.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/gif/
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/gif/user-avatar.ea67286d.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.477461 domain-admin-1.5.1/domain_admin/public/jpg/
+-rw-r--r--   0 runner    (1001) docker     (123)    14271 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    24940 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/jpg/chatpet.fce5580e.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    18591 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/ConditionFilterGroup.345e94e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/ConnectStatus.b684931b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/SelectGroup.f3c9557e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/element-icon.1ce1c350.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749914 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/element-plus.c20bc0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/event-enums.6c6f25e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)   419180 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.0454165e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.1ca9564a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.2f7d52d5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28958 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.6e09f947.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1068448 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.b0fe3ecf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.b12ea372.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21906 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.b862d533.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.d48aa76e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.d5eedcdd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   255125 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.de952ab7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.fd8734f6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94070 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/index.fe4c8ff8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/vendor-lib.cb4f08bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/js/vendor-vue.9e61e0af.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2308 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/m/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/m/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/m/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/2d/
+-r--r--r--   0 runner    (1001) docker     (123)      814 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/43/
+-r--r--r--   0 runner    (1001) docker     (123)     1262 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/4b/
+-r--r--r--   0 runner    (1001) docker     (123)     5351 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/5c/
+-r--r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/5c/98d16331bcc99b0cbbe89a3ffb23e3f5918ff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/61/
+-r--r--r--   0 runner    (1001) docker     (123)      421 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/61/05f9fd4f4b11812fcca0d2e0704e4c8dd6e7a3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.485462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/62/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/62/59838c4de171bc95a934ee2384d626eeb3040a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/67/
+-r--r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/67/d2a69f1213016d777c02e0c99a38871d07da5b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/6f/
+-r--r--r--   0 runner    (1001) docker     (123)      725 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/71/
+-r--r--r--   0 runner    (1001) docker     (123)     2231 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)     2494 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329
+-r--r--r--   0 runner    (1001) docker     (123)      968 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/8e/
+-r--r--r--   0 runner    (1001) docker     (123)     2655 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/93/
+-r--r--r--   0 runner    (1001) docker     (123)     1108 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6
+-r--r--r--   0 runner    (1001) docker     (123)     4673 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/98/
+-r--r--r--   0 runner    (1001) docker     (123)     5141 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/a9/
+-r--r--r--   0 runner    (1001) docker     (123)     1110 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/b0/
+-r--r--r--   0 runner    (1001) docker     (123)     1821 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/c2/
+-r--r--r--   0 runner    (1001) docker     (123)      505 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/c2/c748e84bc4d5118b0e33d6e0073e315a36d034
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/c7/
+-r--r--r--   0 runner    (1001) docker     (123)    31300 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/c8/
+-r--r--r--   0 runner    (1001) docker     (123)   143922 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/d9/
+-r--r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/d9/d9ca2809d6994fef91c1ee2d22bc7a54b8b4a5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/ed/
+-r--r--r--   0 runner    (1001) docker     (123)      979 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/f0/
+-r--r--r--   0 runner    (1001) docker     (123)      755 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/f8/
+-r--r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/objects/fd/
+-r--r--r--   0 runner    (1001) docker     (123)     5204 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/m/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.461461 domain-admin-1.5.1/domain_admin/public/m/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.489462 domain-admin-1.5.1/domain_admin/public/m/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/m/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.493462 domain-admin-1.5.1/domain_admin/public/m/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/common-c7dd5d89.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/common.6194c42f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index-5eda257b.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index-958ae3a0.css
+-rw-r--r--   0 runner    (1001) docker     (123)   379599 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index-9c365a03.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index-ad047368.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index-e8224928.css
+-rw-r--r--   0 runner    (1001) docker     (123)    53115 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index-f79acb3d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index.1a0d1182.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index.1d067866.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index.daaf9893.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/index.feef7c0f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/login-cb9f43ad.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/pages-login-login.09426b90.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/uni.06dd3c8e.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/assets/user-index-be7005ab.css
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.493462 domain-admin-1.5.1/domain_admin/public/m/static/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-07-16 13:46:08.000000 domain-admin-1.5.1/domain_admin/public/m/static/user-avatar.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.493462 domain-admin-1.5.1/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-16 13:46:07.000000 domain-admin-1.5.1/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.493462 domain-admin-1.5.1/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.493462 domain-admin-1.5.1/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/common_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/group_user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/operation_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/service/version_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.493462 domain-admin-1.5.1/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/templates/cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/templates/cert-export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/templates/domain-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/cert_openssl_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/icp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/md5_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/open_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/open_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/open_api/crtsh_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/open_api/ding_talk_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/open_api/feishu_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/open_api/work_weixin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25912 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/utils/whois_util/whois_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      236 2023-07-16 13:45:57.000000 domain-admin-1.5.1/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.465461 domain-admin-1.5.1/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18163 2023-07-16 13:46:09.000000 domain-admin-1.5.1/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-16 13:46:09.000000 domain-admin-1.5.1/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:46:09.000000 domain-admin-1.5.1/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-16 13:46:09.000000 domain-admin-1.5.1/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 13:46:09.000000 domain-admin-1.5.1/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:46:09.000000 domain-admin-1.5.1/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:46:09.497462 domain-admin-1.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-16 13:45:57.000000 domain-admin-1.5.1/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:46:09.497462 domain-admin-1.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3190 2023-07-16 13:45:57.000000 domain-admin-1.5.1/setup.py
```

### Comparing `domain-admin-1.5.0/LICENSE` & `domain-admin-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/PKG-INFO` & `domain-admin-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.5.0
+Version: 1.5.1
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain,ssl,cert,web,monitor
 Platform: any
@@ -647,20 +647,19 @@
 - 暗黑模式
 - `已完成` 支持内网用户自己设置过期时间
 - `已完成` 增加筛选功能: 筛选域名状态、证书状态、网站状态
 - `已完成` 增加批量删除域名的功能
 
 - v1.5.0（开发中）
     - 新增网站监控 [issues#17](https://github.com/mouday/domain-admin/issues/17)
-
-- v1.4.x(开发中)
     - SSL证书申请
     - SSL证书部署
     - admin拥有所有权限
-
+    - 用户密码重置 
+    
 证书测试：[https://badssl.com/](https://badssl.com/)
 
 获取证书列表
 
 ```js
 JSON.stringify([...document.querySelectorAll('a')].map(a=>a.href))
 ```
```

### Comparing `domain-admin-1.5.0/README.md` & `domain-admin-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -613,20 +613,19 @@
 - 暗黑模式
 - `已完成` 支持内网用户自己设置过期时间
 - `已完成` 增加筛选功能: 筛选域名状态、证书状态、网站状态
 - `已完成` 增加批量删除域名的功能
 
 - v1.5.0（开发中）
     - 新增网站监控 [issues#17](https://github.com/mouday/domain-admin/issues/17)
-
-- v1.4.x(开发中)
     - SSL证书申请
     - SSL证书部署
     - admin拥有所有权限
-
+    - 用户密码重置 
+    
 证书测试：[https://badssl.com/](https://badssl.com/)
 
 获取证书列表
 
 ```js
 JSON.stringify([...document.querySelectorAll('a')].map(a=>a.href))
 ```
```

### Comparing `domain-admin-1.5.0/domain_admin/api/address_api.py` & `domain-admin-1.5.1/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/auth_api.py` & `domain-admin-1.5.1/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/cert_api.py` & `domain-admin-1.5.1/domain_admin/api/cert_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/domain_api.py` & `domain-admin-1.5.1/domain_admin/api/domain_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/domain_info_api.py` & `domain-admin-1.5.1/domain_admin/api/domain_info_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/group_api.py` & `domain-admin-1.5.1/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/group_user_api.py` & `domain-admin-1.5.1/domain_admin/api/group_user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/log_operation_api.py` & `domain-admin-1.5.1/domain_admin/api/log_operation_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.5.1/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/notify_api.py` & `domain-admin-1.5.1/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/prometheus_api.py` & `domain-admin-1.5.1/domain_admin/api/prometheus_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/system_api.py` & `domain-admin-1.5.1/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/user_api.py` & `domain-admin-1.5.1/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/api/whois_api.py` & `domain-admin-1.5.1/domain_admin/api/whois_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/compat.py` & `domain-admin-1.5.1/domain_admin/compat.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/config/default_config.py` & `domain-admin-1.5.1/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/config/env_config.py` & `domain-admin-1.5.1/domain_admin/config/env_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/config/runtime_config.py` & `domain-admin-1.5.1/domain_admin/config/runtime_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/enums/config_key_enum.py` & `domain-admin-1.5.1/domain_admin/enums/config_key_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/enums/operation_enum.py` & `domain-admin-1.5.1/domain_admin/enums/operation_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/enums/version_enum.py` & `domain-admin-1.5.1/domain_admin/enums/version_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 @File    : version_enum.py
 @Date    : 2023-02-06
 """
 from __future__ import print_function, unicode_literals, absolute_import, division
 
+
 class VersionEnum(object):
     """
     版本号常量
     """
     Version_100 = '1.0.0'
 
     Version_101 = '1.0.1'
```

### Comparing `domain-admin-1.5.0/domain_admin/log.py` & `domain-admin-1.5.1/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/main.py` & `domain-admin-1.5.1/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_136_to_140_alpha.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_136_to_140_alpha.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_140_alpha_to_140.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_140_alpha_to_140.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_1413_to_1414.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_1413_to_1414.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_1422_to_1423.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_1422_to_1423.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_143_to_144.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_143_to_144.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_145_to_146.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_145_to_146.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/migrate/migrate_common.py` & `domain-admin-1.5.1/domain_admin/migrate/migrate_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/address_model.py` & `domain-admin-1.5.1/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/base_model.py` & `domain-admin-1.5.1/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/database.py` & `domain-admin-1.5.1/domain_admin/model/database.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/domain_info_model.py` & `domain-admin-1.5.1/domain_admin/model/domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/domain_model.py` & `domain-admin-1.5.1/domain_admin/model/domain_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/group_model.py` & `domain-admin-1.5.1/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/group_user_model.py` & `domain-admin-1.5.1/domain_admin/model/group_user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/log_operation_model.py` & `domain-admin-1.5.1/domain_admin/model/log_operation_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.5.1/domain_admin/model/log_scheduler_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/notify_model.py` & `domain-admin-1.5.1/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/system_model.py` & `domain-admin-1.5.1/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/user_model.py` & `domain-admin-1.5.1/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/model/version_model.py` & `domain-admin-1.5.1/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.5.1/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/index` & `domain-admin-1.5.1/domain_admin/public/.git/index`

 * *Files 25% similar despite different names*

#### Comparing `/tmp/diffoscope_v24dqbs3_/tmpx262nlrb_TarContainer/0/91` & `/tmp/diffoscope_v24dqbs3_/tmp9tfygf6z_TarContainer/0/91`

```diff
@@ -5,353 +5,353 @@
 
 Path:      b'css/ConditionFilterGroup.a91875e6.css'
 SHA:       5fa7faf700c98850aa96022ab07af6a07b854f34
 Size:      1601
 Flags:     0b100101
 User ID:   1001
 Group ID:  123
-Created:   1689478234.659030463
-Modified:  1689478234.659030463
-Inode:     291054
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291053
+Device ID: (8, 1)
 
 Path:      b'css/index.563210a3.css'
 SHA:       bec3dc9a28420fa1fbb7115f5acb47dc690dd4db
 Size:      167
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1689478234.659030463
-Modified:  1689478234.659030463
-Inode:     291055
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291054
+Device ID: (8, 1)
 
 Path:      b'css/index.69a97337.css'
 SHA:       197f5cf73cf11d43d915904e0d8aad4736a77d63
 Size:      331526
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291056
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291055
+Device ID: (8, 1)
 
 Path:      b'css/index.a676cc2e.css'
 SHA:       551103b11c4b699a3b4107d3a2ab173dfe238556
 Size:      117
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291057
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291056
+Device ID: (8, 1)
 
 Path:      b'css/index.b285e10a.css'
 SHA:       6c3e3059f9ec00c015681abca34b751c3439513d
 Size:      250
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291058
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291057
+Device ID: (8, 1)
 
 Path:      b'css/index.d028ae37.css'
 SHA:       c4c46ae2c464a49661d7793709077759039f0b5e
 Size:      45
 Flags:     0b10110
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291059
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291058
+Device ID: (8, 1)
 
 Path:      b'favicon.ico'
 SHA:       3c0f2e923566dc74d04e67d46d8b722923ed1949
 Size:      15406
 Flags:     0b1011
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291060
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291059
+Device ID: (8, 1)
 
 Path:      b'gif/user-avatar.ea67286d.gif'
 SHA:       fdbd32c675f85af4ed57021ac0638a21a3c6cad3
 Size:      6334
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291062
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291061
+Device ID: (8, 1)
 
 Path:      b'index.html'
-SHA:       a0b8ee977ea74de0720a00aad1b41570c2488aea
+SHA:       adf592e42021579d5e29d616ab778f5549b949a7
 Size:      911
 Flags:     0b1010
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291063
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291062
+Device ID: (8, 1)
 
 Path:      b'jpg/chatpet-white.10f4f36c.jpg'
 SHA:       ff9c65dfdc7a16150c07745e0030a9d6373920cd
 Size:      14271
 Flags:     0b11110
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291065
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291064
+Device ID: (8, 1)
 
 Path:      b'jpg/chatpet.fce5580e.jpg'
 SHA:       e113bfd922675ce50e68cdf88cd94d16130ad58b
 Size:      24940
 Flags:     0b11000
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291066
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291065
+Device ID: (8, 1)
 
-Path:      b'js/ConditionFilterGroup.98203553.js'
-SHA:       abb5db9b4b7005df3a44582c0e992b3a1da365cc
+Path:      b'js/ConditionFilterGroup.345e94e7.js'
+SHA:       b8bbbb563dcaa4e5e8a878d603dcc0821eadb842
 Size:      18591
 Flags:     0b100011
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291068
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291067
+Device ID: (8, 1)
 
-Path:      b'js/ConnectStatus.afc51e5e.js'
-SHA:       bea294c5fea5d8882221f1810c2f6d85827a062b
+Path:      b'js/ConnectStatus.b684931b.js'
+SHA:       ff3abe67801fd71004bf50541b8e22677539048b
 Size:      953
 Flags:     0b11100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291069
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291068
+Device ID: (8, 1)
 
-Path:      b'js/SelectGroup.c4ef5dae.js'
-SHA:       7a1141eeeacfc2052b0496001fffad61c6672ffd
+Path:      b'js/SelectGroup.f3c9557e.js'
+SHA:       1b3eab78b7dfba767ded92178c81c404f5c21052
 Size:      1257
 Flags:     0b11010
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291070
-Device ID: (8, 17)
+Created:   1689515167.489398872
+Modified:  1689515167.489398872
+Inode:     291069
+Device ID: (8, 1)
 
 Path:      b'js/element-icon.1ce1c350.js'
 SHA:       52c1926de72b181c9b7faf597fb8f71f48565462
 Size:      195335
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1689478234.663030509
-Modified:  1689478234.663030509
-Inode:     291071
-Device ID: (8, 17)
+Created:   1689515167.493398998
+Modified:  1689515167.493398998
+Inode:     291070
+Device ID: (8, 1)
 
 Path:      b'js/element-plus.c20bc0dd.js'
 SHA:       33ea7b19add95fae6c823919ab86c3bcdcf87307
 Size:      749914
 Flags:     0b11011
 User ID:   1001
 Group ID:  123
-Created:   1689478234.671030602
-Modified:  1689478234.671030602
-Inode:     291072
-Device ID: (8, 17)
+Created:   1689515167.497399124
+Modified:  1689515167.497399124
+Inode:     291071
+Device ID: (8, 1)
 
 Path:      b'js/event-enums.6c6f25e7.js'
 SHA:       7f64d8af0501887e805dc9ccf8228f4fb5e73fdb
 Size:      579
 Flags:     0b11010
 User ID:   1001
 Group ID:  123
-Created:   1689478234.671030602
-Modified:  1689478234.671030602
+Created:   1689515167.497399124
+Modified:  1689515167.497399124
+Inode:     291072
+Device ID: (8, 1)
+
+Path:      b'js/index.0454165e.js'
+SHA:       ea014768708683bab0f086bbe7bbbee4bd721482
+Size:      419180
+Flags:     0b10100
+User ID:   1001
+Group ID:  123
+Created:   1689515167.501399250
+Modified:  1689515167.501399250
 Inode:     291073
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.18819e48.js'
-SHA:       c05315f3d882bac87d0845ebd85af8097c722b5f
-Size:      28958
+Path:      b'js/index.1ca9564a.js'
+SHA:       51b89a9c3bf4fb6075399ba7bacc0f1594493956
+Size:      30254
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.671030602
-Modified:  1689478234.671030602
+Created:   1689515167.501399250
+Modified:  1689515167.501399250
 Inode:     291074
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.1a48d33b.js'
-SHA:       948be774e1f2613f4fa1b82ae88043ef92d70761
-Size:      4147
+Path:      b'js/index.2f7d52d5.js'
+SHA:       1d3e7887c6d2b61648a0ec4ae187a97314a3d9a5
+Size:      4248
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.671030602
-Modified:  1689478234.671030602
+Created:   1689515167.501399250
+Modified:  1689515167.501399250
 Inode:     291075
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.4846c617.js'
-SHA:       7101c7e7cd243bb0c4a7caf901ce1005911a8432
-Size:      30256
+Path:      b'js/index.6e09f947.js'
+SHA:       e2ae3e466505ab377291c9bc893b36ea4e4cc346
+Size:      28958
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.671030602
-Modified:  1689478234.671030602
+Created:   1689515167.501399250
+Modified:  1689515167.501399250
 Inode:     291076
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.5aa6512c.js'
-SHA:       fbd49bf5e92b08848a3c75b285c90c0100d7b440
-Size:      419180
+Path:      b'js/index.b0fe3ecf.js'
+SHA:       a00aeea345a67ff29a66605c34e468c397bcecf6
+Size:      1068448
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.675030649
-Modified:  1689478234.675030649
+Created:   1689515167.505399377
+Modified:  1689515167.505399377
 Inode:     291077
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.730c57dc.js'
-SHA:       24933b4eedb8202eacc8a8dc76466bb8ff28efcd
-Size:      21906
+Path:      b'js/index.b12ea372.js'
+SHA:       41b5605e3f03a272f1f17c91a1c9203df59a19d6
+Size:      8789
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.675030649
-Modified:  1689478234.675030649
+Created:   1689515167.505399377
+Modified:  1689515167.505399377
 Inode:     291078
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.a12c098a.js'
-SHA:       b681b7d87ead80778d68ff251ed7f9a2dde0950a
-Size:      1068448
+Path:      b'js/index.b862d533.js'
+SHA:       84155baa6831b822324d3b71d53c2da8e799e6ad
+Size:      21906
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.679030695
-Modified:  1689478234.679030695
+Created:   1689515167.505399377
+Modified:  1689515167.505399377
 Inode:     291079
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.b5155817.js'
-SHA:       11e53e58b56342d3ed07f7ad82094209a85110d0
-Size:      8789
+Path:      b'js/index.d48aa76e.js'
+SHA:       054a020e56d7af80d0110b8500a034ea21c16a9c
+Size:      4147
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.679030695
-Modified:  1689478234.679030695
+Created:   1689515167.505399377
+Modified:  1689515167.505399377
 Inode:     291080
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.c5fb6f8c.js'
-SHA:       3f9f711ce627c122b8c70ac9300d1d5a046c4690
-Size:      255125
+Path:      b'js/index.d5eedcdd.js'
+SHA:       2b879e31c999b53e51dbbb528db102aac5a0ddb5
+Size:      1818
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
+Created:   1689515167.505399377
+Modified:  1689515167.505399377
 Inode:     291081
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.deda20cc.js'
-SHA:       67e95e36239b9f21e0c968cde274e1c8074caa0f
-Size:      94070
+Path:      b'js/index.de952ab7.js'
+SHA:       0e0f1ee6c217e5da4bd965f2d9ce0ab2cac11e03
+Size:      255125
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
+Created:   1689515167.509399503
+Modified:  1689515167.509399503
 Inode:     291082
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.e036cf3b.js'
-SHA:       da6a99e6a186e30a655b7b7082699da9e6dc557f
-Size:      1818
+Path:      b'js/index.fd8734f6.js'
+SHA:       d904d142c9bf7ef514a7a46daf1a1a63daffb3ec
+Size:      5241
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
+Created:   1689515167.509399503
+Modified:  1689515167.509399503
 Inode:     291083
-Device ID: (8, 17)
+Device ID: (8, 1)
 
-Path:      b'js/index.f2a38d9e.js'
-SHA:       be4d5a11a24cb52c5bc6ad7cb0f0cba03770565d
-Size:      5241
+Path:      b'js/index.fe4c8ff8.js'
+SHA:       f1d1775a53fb6d01f3cf868d7675175acb4972e5
+Size:      94070
 Flags:     0b10100
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
+Created:   1689515167.509399503
+Modified:  1689515167.509399503
 Inode:     291084
-Device ID: (8, 17)
-
-Path:      b'js/index.fd336ece.js'
-SHA:       85d5b39f098d01c9dbc10214df393ab55c5c5685
-Size:      4248
-Flags:     0b10100
-User ID:   1001
-Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
-Inode:     291085
-Device ID: (8, 17)
+Device ID: (8, 1)
 
 Path:      b'js/vendor-lib.cb4f08bf.js'
 SHA:       bf6e10bcc54e0b8256bb0a7bbe2cdb0c2384db91
 Size:      23389
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
-Inode:     291086
-Device ID: (8, 17)
+Created:   1689515167.509399503
+Modified:  1689515167.509399503
+Inode:     291085
+Device ID: (8, 1)
 
 Path:      b'js/vendor-vue.9e61e0af.js'
 SHA:       b31cb2667f48424e34cf9517362eadf899f704ad
 Size:      94202
 Flags:     0b11001
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
-Inode:     291087
-Device ID: (8, 17)
+Created:   1689515167.509399503
+Modified:  1689515167.509399503
+Inode:     291086
+Device ID: (8, 1)
 
 Path:      b'svg/logo.184a2d7d.svg'
 SHA:       6d15191314c9b832ac41056a30bf0bf6533a29dc
 Size:      1478
 Flags:     0b10101
 User ID:   1001
 Group ID:  123
-Created:   1689478234.683030742
-Modified:  1689478234.683030742
-Inode:     291089
-Device ID: (8, 17)
+Created:   1689515167.509399503
+Modified:  1689515167.509399503
+Inode:     291088
+Device ID: (8, 1)
```

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63` & `domain-admin-1.5.1/domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/33/ea7b19add95fae6c823919ab86c3bcdcf87307` & `domain-admin-1.5.1/domain_admin/public/.git/objects/33/ea7b19add95fae6c823919ab86c3bcdcf87307`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949` & `domain-admin-1.5.1/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462` & `domain-admin-1.5.1/domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34` & `domain-admin-1.5.1/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.5.1/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad` & `domain-admin-1.5.1/domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/bf/6e10bcc54e0b8256bb0a7bbe2cdb0c2384db91` & `domain-admin-1.5.1/domain_admin/public/.git/objects/bf/6e10bcc54e0b8256bb0a7bbe2cdb0c2384db91`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b` & `domain-admin-1.5.1/domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.1/domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd` & `domain-admin-1.5.1/domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/css/ConditionFilterGroup.a91875e6.css` & `domain-admin-1.5.1/domain_admin/public/css/ConditionFilterGroup.a91875e6.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/css/index.69a97337.css` & `domain-admin-1.5.1/domain_admin/public/css/index.69a97337.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/favicon.ico` & `domain-admin-1.5.1/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/gif/user-avatar.ea67286d.gif` & `domain-admin-1.5.1/domain_admin/public/gif/user-avatar.ea67286d.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/index.html` & `domain-admin-1.5.1/domain_admin/public/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       content="width=device-width, initial-scale=1.0"
     />
     <meta
       name="referrer"
       content="no-referrer"
     />
     <title>Domain Admin-域名和SSL证书监测系统</title>
-    <script type="module" crossorigin src="./js/index.c5fb6f8c.js"></script>
+    <script type="module" crossorigin src="./js/index.de952ab7.js"></script>
     <link rel="modulepreload" crossorigin href="./js/vendor-vue.9e61e0af.js">
     <link rel="modulepreload" crossorigin href="./js/element-icon.1ce1c350.js">
     <link rel="modulepreload" crossorigin href="./js/element-plus.c20bc0dd.js">
     <link rel="modulepreload" crossorigin href="./js/vendor-lib.cb4f08bf.js">
     <link rel="stylesheet" href="./css/index.69a97337.css">
   </head>
   <body>
```

### Comparing `domain-admin-1.5.0/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg` & `domain-admin-1.5.1/domain_admin/public/jpg/chatpet-white.10f4f36c.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/jpg/chatpet.fce5580e.jpg` & `domain-admin-1.5.1/domain_admin/public/jpg/chatpet.fce5580e.jpg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/js/ConditionFilterGroup.98203553.js` & `domain-admin-1.5.1/domain_admin/public/js/ConditionFilterGroup.345e94e7.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     d as O
 } from "./element-plus.c20bc0dd.js";
 import {
     _ as D,
     R as E
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     o as d,
     c as u,
     J as I,
     U as w,
     ah as l,
     V as n,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/ConnectStatus.afc51e5e.js` & `domain-admin-1.5.1/domain_admin/public/js/ConnectStatus.b684931b.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as n,
     o as a,
     O as s,
     P as e,
     V as l
 } from "./vendor-vue.9e61e0af.js";
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/SelectGroup.c4ef5dae.js` & `domain-admin-1.5.1/domain_admin/public/js/SelectGroup.f3c9557e.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
     F as h,
     L as g,
     al as _
 } from "./vendor-vue.9e61e0af.js";
 import {
     H as f,
     _ as O
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 const S = u({
         id: "group-store",
         state: () => ({
             groupOptions: []
         }),
         getters: {
             getGroupOptions: e => e.groupOptions
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/element-icon.1ce1c350.js` & `domain-admin-1.5.1/domain_admin/public/js/element-icon.1ce1c350.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/js/element-plus.c20bc0dd.js` & `domain-admin-1.5.1/domain_admin/public/js/element-plus.c20bc0dd.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/js/event-enums.6c6f25e7.js` & `domain-admin-1.5.1/domain_admin/public/js/event-enums.6c6f25e7.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.18819e48.js` & `domain-admin-1.5.1/domain_admin/public/js/index.6e09f947.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     i as Y,
     E as M
 } from "./event-enums.6c6f25e7.js";
 import {
     S as N,
     u as z
-} from "./SelectGroup.c4ef5dae.js";
+} from "./SelectGroup.f3c9557e.js";
 import {
     _ as v,
     R as $,
     d as L,
     r as W
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as s,
     ar as P,
     Q as G,
     o as u,
     c as g,
     V as o,
@@ -33,18 +33,18 @@
 } from "./vendor-vue.9e61e0af.js";
 import {
     E as q,
     A as J,
     a as Z,
     b as ee,
     C as te
-} from "./ConditionFilterGroup.98203553.js";
+} from "./ConditionFilterGroup.345e94e7.js";
 import {
     C as oe
-} from "./ConnectStatus.afc51e5e.js";
+} from "./ConnectStatus.b684931b.js";
 import {
     F as le
 } from "./vendor-lib.cb4f08bf.js";
 import {
     a as ie
 } from "./element-plus.c20bc0dd.js";
 import "./element-icon.1ce1c350.js";
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.1a48d33b.js` & `domain-admin-1.5.1/domain_admin/public/js/index.d48aa76e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as u
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as n,
     o as _,
     c as g,
     V as a,
     P as l,
     a as c,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.4846c617.js` & `domain-admin-1.5.1/domain_admin/public/js/index.1ca9564a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     i as H,
     E as M
 } from "./event-enums.6c6f25e7.js";
 import {
     S as P,
     u as E
-} from "./SelectGroup.c4ef5dae.js";
+} from "./SelectGroup.f3c9557e.js";
 import {
     _ as v,
     R as B,
     d as $,
     r as Y
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as s,
     ar as z,
     Q as A,
     o as c,
     c as b,
     V as i,
@@ -33,15 +33,15 @@
 } from "./vendor-vue.9e61e0af.js";
 import {
     E as L,
     A as J,
     a as Z,
     b as ee,
     C as te
-} from "./ConditionFilterGroup.98203553.js";
+} from "./ConditionFilterGroup.345e94e7.js";
 import {
     F as oe
 } from "./vendor-lib.cb4f08bf.js";
 import {
     a as ie
 } from "./element-plus.c20bc0dd.js";
 import "./element-icon.1ce1c350.js";
@@ -868,15 +868,15 @@
                 this.currentRow = o, this.dialogDetailVisible = !0
             },
             handleShowAddressListgDialog(o) {
                 this.currentRow = o, this.AddressListgDialogVisible = !0
             },
             handleCertCountClick(o) {
                 let e = this.$router.resolve({
-                    name: "domain-list",
+                    name: "cert-list",
                     query: {
                         keyword: o.domain
                     }
                 });
                 window.open(e.href, "_blank")
             },
             handleRefreshRow(o) {
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.5aa6512c.js` & `domain-admin-1.5.1/domain_admin/public/js/index.0454165e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -31,15 +31,15 @@
     a8 as Vn,
     R as If,
     S as Ta,
     U as mi
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as nt
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.cb4f08bf.js";
 import "./element-plus.c20bc0dd.js";
 const Wf = {
         status: [{
             message: "\u72B6\u6001\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.730c57dc.js` & `domain-admin-1.5.1/domain_admin/public/js/index.b862d533.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     _ as C,
     R as O
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as a,
     o as p,
     c as y,
     V as o,
     P as i,
     a as _,
@@ -21,15 +21,15 @@
     Q as T,
     F as A,
     ay as N
 } from "./vendor-vue.9e61e0af.js";
 import {
     S as j,
     u as B
-} from "./SelectGroup.c4ef5dae.js";
+} from "./SelectGroup.f3c9557e.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.cb4f08bf.js";
 import "./element-plus.c20bc0dd.js";
 const F = {
         name: [{
             message: "\u540D\u79F0\u4E0D\u80FD\u4E3A\u7A7A",
             required: !0,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.a12c098a.js` & `domain-admin-1.5.1/domain_admin/public/js/index.b0fe3ecf.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as Cl
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as ue,
     o as Ue,
     c as Fe,
     V as le,
     P as _e,
     a as Re,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.b5155817.js` & `domain-admin-1.5.1/domain_admin/public/js/index.b12ea372.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as y
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as i,
     o as b,
     c as v,
     V as a,
     P as o,
     a as h,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.c5fb6f8c.js` & `domain-admin-1.5.1/domain_admin/public/js/index.de952ab7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1740,15 +1740,15 @@
         },
         redirect: {
             name: "cert-list"
         },
         children: [{
             path: "list",
             name: "cert-list",
-            component: () => __vitePreload(() => import("./index.18819e48.js"), ["index.18819e48.js", "event-enums.6c6f25e7.js", "SelectGroup.c4ef5dae.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.98203553.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "ConnectStatus.afc51e5e.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.6e09f947.js"), ["index.6e09f947.js", "event-enums.6c6f25e7.js", "SelectGroup.f3c9557e.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.345e94e7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "ConnectStatus.b684931b.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
             meta: {
                 title: "\u8BC1\u4E66\u5217\u8868",
                 icon: "Tickets"
             }
         }]
     }, {
         path: "/domain",
@@ -1760,15 +1760,15 @@
         },
         redirect: {
             name: "domain-list"
         },
         children: [{
             path: "list",
             name: "domain-list",
-            component: () => __vitePreload(() => import("./index.4846c617.js"), ["index.4846c617.js", "../css/index.563210a3.css", "event-enums.6c6f25e7.js", "SelectGroup.c4ef5dae.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.98203553.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.1ca9564a.js"), ["index.1ca9564a.js", "../css/index.563210a3.css", "event-enums.6c6f25e7.js", "SelectGroup.f3c9557e.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.345e94e7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
             meta: {
                 title: "\u57DF\u540D\u5217\u8868",
                 icon: "Coin"
             }
         }]
     }, {
         path: "/group",
@@ -1780,15 +1780,15 @@
         },
         redirect: {
             name: "group-list"
         },
         children: [{
             path: "list",
             name: "group-list",
-            component: () => __vitePreload(() => import("./index.730c57dc.js"), ["index.730c57dc.js", "vendor-vue.9e61e0af.js", "SelectGroup.c4ef5dae.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.b862d533.js"), ["index.b862d533.js", "vendor-vue.9e61e0af.js", "SelectGroup.f3c9557e.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u5206\u7EC4\u7BA1\u7406",
                 icon: "Files"
             }
         }]
     }, {
         path: "/notify",
@@ -1800,15 +1800,15 @@
         },
         redirect: {
             name: "notify-list"
         },
         children: [{
             path: "edit",
             name: "notify-list",
-            component: () => __vitePreload(() => import("./index.5aa6512c.js"), ["index.5aa6512c.js", "event-enums.6c6f25e7.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.0454165e.js"), ["index.0454165e.js", "event-enums.6c6f25e7.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u901A\u77E5\u5217\u8868",
                 icon: "Message"
             }
         }]
     }, {
         path: "/data",
@@ -1821,37 +1821,37 @@
             title: "\u6570\u636E\u7BA1\u7406",
             icon: "Box",
             roles: [RoleEnum.Admin]
         },
         children: [{
             path: "cert-list",
             name: "data-cert-list",
-            component: () => __vitePreload(() => import("./index.18819e48.js"), ["index.18819e48.js", "event-enums.6c6f25e7.js", "SelectGroup.c4ef5dae.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.98203553.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "ConnectStatus.afc51e5e.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.6e09f947.js"), ["index.6e09f947.js", "event-enums.6c6f25e7.js", "SelectGroup.f3c9557e.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.345e94e7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "ConnectStatus.b684931b.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u8BC1\u4E66",
                 icon: "Tickets"
             },
             props: {
                 role: RoleEnum.Admin
             }
         }, {
             path: "domain-list",
             name: "data-domain-list",
-            component: () => __vitePreload(() => import("./index.4846c617.js"), ["index.4846c617.js", "../css/index.563210a3.css", "event-enums.6c6f25e7.js", "SelectGroup.c4ef5dae.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.98203553.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.1ca9564a.js"), ["index.1ca9564a.js", "../css/index.563210a3.css", "event-enums.6c6f25e7.js", "SelectGroup.f3c9557e.js", "vendor-vue.9e61e0af.js", "ConditionFilterGroup.345e94e7.js", "../css/ConditionFilterGroup.a91875e6.css", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u57DF\u540D",
                 icon: "Coin"
             },
             props: {
                 role: RoleEnum.Admin
             }
         }, {
             path: "group-list",
             name: "data-group-list",
-            component: () => __vitePreload(() => import("./index.730c57dc.js"), ["index.730c57dc.js", "vendor-vue.9e61e0af.js", "SelectGroup.c4ef5dae.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.b862d533.js"), ["index.b862d533.js", "vendor-vue.9e61e0af.js", "SelectGroup.f3c9557e.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u5168\u90E8\u5206\u7EC4",
                 icon: "Files"
             },
             props: {
                 role: RoleEnum.Admin
             }
@@ -1867,42 +1867,42 @@
             title: "\u7CFB\u7EDF\u7BA1\u7406",
             icon: "Setting",
             roles: [RoleEnum.Admin]
         },
         children: [{
             path: "user-list",
             name: "admin-user-list",
-            component: () => __vitePreload(() => import("./index.b5155817.js"), ["index.b5155817.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.b12ea372.js"), ["index.b12ea372.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u7528\u6237\u7BA1\u7406",
                 icon: "User",
                 roles: [RoleEnum.Admin]
             }
         }, {
             path: "system-setup",
             name: "system-setup",
-            component: () => __vitePreload(() => import("./index.deda20cc.js"), ["index.deda20cc.js", "../css/index.d028ae37.css", "vendor-vue.9e61e0af.js", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.fe4c8ff8.js"), ["index.fe4c8ff8.js", "../css/index.d028ae37.css", "vendor-vue.9e61e0af.js", "element-plus.c20bc0dd.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js"], import.meta.url),
             meta: {
                 title: "\u7CFB\u7EDF\u8BBE\u7F6E",
                 icon: "Setting",
                 roles: [RoleEnum.Admin]
             }
         }, {
             path: "log-scheduler-list",
             name: "log-scheduler-list",
-            component: () => __vitePreload(() => import("./index.fd336ece.js"), ["index.fd336ece.js", "ConnectStatus.afc51e5e.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.2f7d52d5.js"), ["index.2f7d52d5.js", "ConnectStatus.b684931b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u76D1\u6D4B\u65E5\u5FD7",
                 icon: "Calendar",
                 roles: [RoleEnum.Admin]
             }
         }, {
             path: "log-operation-list",
             name: "log-operation-list",
-            component: () => __vitePreload(() => import("./index.a12c098a.js"), ["index.a12c098a.js", "../css/index.b285e10a.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.b0fe3ecf.js"), ["index.b0fe3ecf.js", "../css/index.b285e10a.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u64CD\u4F5C\u65E5\u5FD7",
                 icon: "Compass",
                 roles: [RoleEnum.Admin]
             }
         }]
     }, {
@@ -1915,33 +1915,33 @@
         meta: {
             hidden: !0,
             title: "\u5DE5\u5177\u7BB1"
         },
         children: [{
             path: "lab",
             name: "lab",
-            component: () => __vitePreload(() => import("./index.e036cf3b.js"), ["index.e036cf3b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.d5eedcdd.js"), ["index.d5eedcdd.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "WHOIS\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "domain-cert-list",
             name: "domain-cert-list",
-            component: () => __vitePreload(() => import("./index.1a48d33b.js"), ["index.1a48d33b.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.d48aa76e.js"), ["index.d48aa76e.js", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u5B50\u57DF\u540D\u8BC1\u4E66\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }, {
             path: "cert-info",
             name: "cert-info",
-            component: () => __vitePreload(() => import("./index.f2a38d9e.js"), ["index.f2a38d9e.js", "../css/index.a676cc2e.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
+            component: () => __vitePreload(() => import("./index.fd8734f6.js"), ["index.fd8734f6.js", "../css/index.a676cc2e.css", "vendor-vue.9e61e0af.js", "element-icon.1ce1c350.js", "vendor-lib.cb4f08bf.js", "element-plus.c20bc0dd.js"], import.meta.url),
             meta: {
                 title: "\u8BC1\u4E66\u4FE1\u606F\u67E5\u8BE2",
                 icon: "Box",
                 hidden: !0
             }
         }]
     }];
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.deda20cc.js` & `domain-admin-1.5.1/domain_admin/public/js/index.fe4c8ff8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as je
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as V,
     o as K,
     c as X,
     V as b,
     P as I,
     a as oe,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.e036cf3b.js` & `domain-admin-1.5.1/domain_admin/public/js/index.d5eedcdd.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     a as i,
     U as w,
     a9 as S,
     T as b
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as V
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.cb4f08bf.js";
 import "./element-plus.c20bc0dd.js";
 const k = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.f2a38d9e.js` & `domain-admin-1.5.1/domain_admin/public/js/index.fd8734f6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     F as k,
     a8 as N,
     az as w,
     aA as j
 } from "./vendor-vue.9e61e0af.js";
 import {
     _ as V
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import "./element-icon.1ce1c350.js";
 import "./vendor-lib.cb4f08bf.js";
 import "./element-plus.c20bc0dd.js";
 const A = {
         name: "index",
         props: {},
         components: {},
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/index.fd336ece.js` & `domain-admin-1.5.1/domain_admin/public/js/index.2f7d52d5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     C as w
-} from "./ConnectStatus.afc51e5e.js";
+} from "./ConnectStatus.b684931b.js";
 import {
     _ as m
-} from "./index.c5fb6f8c.js";
+} from "./index.de952ab7.js";
 import {
     ah as l,
     o as _,
     c as f,
     V as a,
     P as n,
     a as c,
```

### Comparing `domain-admin-1.5.0/domain_admin/public/js/vendor-lib.cb4f08bf.js` & `domain-admin-1.5.1/domain_admin/public/js/vendor-lib.cb4f08bf.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/js/vendor-vue.9e61e0af.js` & `domain-admin-1.5.1/domain_admin/public/js/vendor-vue.9e61e0af.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/commit-msg.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-commit.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-push.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-rebase.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/pre-receive.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/push-to-checkout.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/sendemail-validate.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/hooks/update.sample` & `domain-admin-1.5.1/domain_admin/public/m/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/2d/7cec3e00ed3b3b835eb233ae4bb2ea21fb5a0b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/43/c4fcdf29fe10c6256aa4e9cf00f534e6933efc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/4b/63cfa29bd94b198d895f7a64e10c20f167e65b`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/6f/9d23d38fd97c94c1dccf971fd7b7636cc075d2`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/71/4dbccc412b153f5044c269745126581e3cf373`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/7a/694f3c8aca1586dc6f0e6e9e2773e207992329`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/7a/c4cdd0b7c56c8fe9f98aaf044df58bef26b7a5`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/8e/ff5bef00cd2492d9b806988ea99996d636c126`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/93/85587145f9afbabe2aa1a489d24fd1f489e5c6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/93/db3989e7874cd6b75bc0e984690ffa16666ea6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/98/1e059e0de4604a5dec80930d8ff7cdf84e0006`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/a9/a1035a25ce05f60741e3f70716a18d93322203`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/b0/ecf609c3df960010b6f7877bc379ea45d1e9da`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/c7/ef9b19427f9af9e445bb5d63231ccd58ef5b28`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/c8/bec3f3e9b26642a8221c20a5e422bc2cada687`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/ed/50570bc6865f7dff2468d49072d7f4e4cb81d4`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/f0/a3f5a57d6bdb9961c3a56f4a992a08a0ecd671`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/f8/0169320ed23edd9889e4de7631267635bfec27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3` & `domain-admin-1.5.1/domain_admin/public/m/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/common-c7dd5d89.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/common-c7dd5d89.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/common.6194c42f.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/common.6194c42f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index-5eda257b.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/index-5eda257b.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index-958ae3a0.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/index-958ae3a0.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index-9c365a03.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/index-9c365a03.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index-ad047368.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/index-ad047368.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index-e8224928.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/index-e8224928.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index-f79acb3d.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/index-f79acb3d.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index.1a0d1182.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/index.1a0d1182.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index.1d067866.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/index.1d067866.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index.daaf9893.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/index.daaf9893.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/index.feef7c0f.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/index.feef7c0f.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/login-cb9f43ad.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/login-cb9f43ad.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/pages-cert-list-cert-list.e9ecbf65.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/pages-domain-list-domain-list.da5e6454.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/pages-login-login.09426b90.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/pages-login-login.09426b90.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js` & `domain-admin-1.5.1/domain_admin/public/m/assets/pages-user-index-user-index.d8efba8c.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/uni.06dd3c8e.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/uni.06dd3c8e.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/assets/user-index-be7005ab.css` & `domain-admin-1.5.1/domain_admin/public/m/assets/user-index-be7005ab.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/index.html` & `domain-admin-1.5.1/domain_admin/public/m/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/m/static/user-avatar.gif` & `domain-admin-1.5.1/domain_admin/public/m/static/user-avatar.gif`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.5.1/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/router/api_map.py` & `domain-admin-1.5.1/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/router/permission.py` & `domain-admin-1.5.1/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/auth_service.py` & `domain-admin-1.5.1/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/common_service.py` & `domain-admin-1.5.1/domain_admin/service/common_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/domain_info_service.py` & `domain-admin-1.5.1/domain_admin/service/domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/domain_service.py` & `domain-admin-1.5.1/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/file_service.py` & `domain-admin-1.5.1/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/group_service.py` & `domain-admin-1.5.1/domain_admin/service/group_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/group_user_service.py` & `domain-admin-1.5.1/domain_admin/service/group_user_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/notify_service.py` & `domain-admin-1.5.1/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/operation_service.py` & `domain-admin-1.5.1/domain_admin/service/operation_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/scheduler_service.py` & `domain-admin-1.5.1/domain_admin/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/system_service.py` & `domain-admin-1.5.1/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/token_service.py` & `domain-admin-1.5.1/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/service/version_service.py` & `domain-admin-1.5.1/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/templates/cert-email.html` & `domain-admin-1.5.1/domain_admin/templates/cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/templates/domain-email.html` & `domain-admin-1.5.1/domain_admin/templates/domain-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.5.1/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.5.1/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/cert_util/cert_openssl_v2.py` & `domain-admin-1.5.1/domain_admin/utils/cert_util/cert_openssl_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.5.1/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.5.1/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/datetime_util.py` & `domain-admin-1.5.1/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/domain_util.py` & `domain-admin-1.5.1/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/email_util.py` & `domain-admin-1.5.1/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/json/default.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/json/default.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/json/json_encoder.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/json/json_encoder.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/flask_ext/json/json_provider.py` & `domain-admin-1.5.1/domain_admin/utils/flask_ext/json/json_provider.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/icp_util.py` & `domain-admin-1.5.1/domain_admin/utils/icp_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/ip_util.py` & `domain-admin-1.5.1/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/json_util.py` & `domain-admin-1.5.1/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/open_api/crtsh_api.py` & `domain-admin-1.5.1/domain_admin/utils/open_api/crtsh_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/open_api/ding_talk_api.py` & `domain-admin-1.5.1/domain_admin/utils/open_api/ding_talk_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/open_api/feishu_api.py` & `domain-admin-1.5.1/domain_admin/utils/open_api/feishu_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/open_api/work_weixin_api.py` & `domain-admin-1.5.1/domain_admin/utils/open_api/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.5.1/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/secret_util.py` & `domain-admin-1.5.1/domain_admin/utils/secret_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/text_util.py` & `domain-admin-1.5.1/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/time_util.py` & `domain-admin-1.5.1/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/whois_util/config.py` & `domain-admin-1.5.1/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/whois_util/util.py` & `domain-admin-1.5.1/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.5.1/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.5.1/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.5.0/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.5.1/domain_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.5.0
+Version: 1.5.1
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain,ssl,cert,web,monitor
 Platform: any
@@ -647,20 +647,19 @@
 - 暗黑模式
 - `已完成` 支持内网用户自己设置过期时间
 - `已完成` 增加筛选功能: 筛选域名状态、证书状态、网站状态
 - `已完成` 增加批量删除域名的功能
 
 - v1.5.0（开发中）
     - 新增网站监控 [issues#17](https://github.com/mouday/domain-admin/issues/17)
-
-- v1.4.x(开发中)
     - SSL证书申请
     - SSL证书部署
     - admin拥有所有权限
-
+    - 用户密码重置 
+    
 证书测试：[https://badssl.com/](https://badssl.com/)
 
 获取证书列表
 
 ```js
 JSON.stringify([...document.querySelectorAll('a')].map(a=>a.href))
 ```
```

### Comparing `domain-admin-1.5.0/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.5.1/domain_admin.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -90,82 +90,82 @@
 domain_admin/public/.git/hooks/push-to-checkout.sample
 domain_admin/public/.git/hooks/sendemail-validate.sample
 domain_admin/public/.git/hooks/update.sample
 domain_admin/public/.git/info/exclude
 domain_admin/public/.git/logs/HEAD
 domain_admin/public/.git/logs/refs/heads/dist
 domain_admin/public/.git/logs/refs/remotes/origin/dist
-domain_admin/public/.git/objects/11/e53e58b56342d3ed07f7ad82094209a85110d0
+domain_admin/public/.git/objects/05/4a020e56d7af80d0110b8500a034ea21c16a9c
+domain_admin/public/.git/objects/0e/0f1ee6c217e5da4bd965f2d9ce0ab2cac11e03
 domain_admin/public/.git/objects/19/7f5cf73cf11d43d915904e0d8aad4736a77d63
+domain_admin/public/.git/objects/1b/3eab78b7dfba767ded92178c81c404f5c21052
+domain_admin/public/.git/objects/1d/3e7887c6d2b61648a0ec4ae187a97314a3d9a5
 domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-domain_admin/public/.git/objects/24/933b4eedb8202eacc8a8dc76466bb8ff28efcd
-domain_admin/public/.git/objects/2a/495a2b7d8f5ff034faec7f33caab9440ed4304
+domain_admin/public/.git/objects/2b/5704558111e371903e48b7fedf70d24dad55bf
+domain_admin/public/.git/objects/2b/879e31c999b53e51dbbb528db102aac5a0ddb5
 domain_admin/public/.git/objects/33/ea7b19add95fae6c823919ab86c3bcdcf87307
 domain_admin/public/.git/objects/35/eeddd87c8cb15685d288c8eda40c337c7d5667
 domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
-domain_admin/public/.git/objects/3f/9f711ce627c122b8c70ac9300d1d5a046c4690
+domain_admin/public/.git/objects/41/b5605e3f03a272f1f17c91a1c9203df59a19d6
+domain_admin/public/.git/objects/51/b89a9c3bf4fb6075399ba7bacc0f1594493956
 domain_admin/public/.git/objects/52/c1926de72b181c9b7faf597fb8f71f48565462
 domain_admin/public/.git/objects/55/1103b11c4b699a3b4107d3a2ab173dfe238556
 domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-domain_admin/public/.git/objects/67/e95e36239b9f21e0c968cde274e1c8074caa0f
 domain_admin/public/.git/objects/6c/3e3059f9ec00c015681abca34b751c3439513d
 domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-domain_admin/public/.git/objects/71/01c7e7cd243bb0c4a7caf901ce1005911a8432
-domain_admin/public/.git/objects/7a/1141eeeacfc2052b0496001fffad61c6672ffd
 domain_admin/public/.git/objects/7f/64d8af0501887e805dc9ccf8228f4fb5e73fdb
-domain_admin/public/.git/objects/85/d5b39f098d01c9dbc10214df393ab55c5c5685
+domain_admin/public/.git/objects/84/155baa6831b822324d3b71d53c2da8e799e6ad
 domain_admin/public/.git/objects/89/0f3ed83973272c63b56a722a88fe25160d11d2
 domain_admin/public/.git/objects/8c/f880f5a9481ef71cd22e08d59e7d366775b360
-domain_admin/public/.git/objects/94/8be774e1f2613f4fa1b82ae88043ef92d70761
-domain_admin/public/.git/objects/9a/4957917630d72546f62ab236f9e916c0e8670b
-domain_admin/public/.git/objects/a0/b8ee977ea74de0720a00aad1b41570c2488aea
-domain_admin/public/.git/objects/ab/b5db9b4b7005df3a44582c0e992b3a1da365cc
+domain_admin/public/.git/objects/a0/0aeea345a67ff29a66605c34e468c397bcecf6
+domain_admin/public/.git/objects/ad/f592e42021579d5e29d616ab778f5549b949a7
 domain_admin/public/.git/objects/b3/1cb2667f48424e34cf9517362eadf899f704ad
-domain_admin/public/.git/objects/b6/81b7d87ead80778d68ff251ed7f9a2dde0950a
-domain_admin/public/.git/objects/be/4d5a11a24cb52c5bc6ad7cb0f0cba03770565d
-domain_admin/public/.git/objects/be/a294c5fea5d8882221f1810c2f6d85827a062b
+domain_admin/public/.git/objects/b8/bbbb563dcaa4e5e8a878d603dcc0821eadb842
 domain_admin/public/.git/objects/be/c3dc9a28420fa1fbb7115f5acb47dc690dd4db
 domain_admin/public/.git/objects/bf/6e10bcc54e0b8256bb0a7bbe2cdb0c2384db91
-domain_admin/public/.git/objects/c0/5315f3d882bac87d0845ebd85af8097c722b5f
 domain_admin/public/.git/objects/c4/c46ae2c464a49661d7793709077759039f0b5e
-domain_admin/public/.git/objects/cb/f418bdf2a49f64c14ebe734fb6d6dce4c00366
-domain_admin/public/.git/objects/da/6a99e6a186e30a655b7b7082699da9e6dc557f
+domain_admin/public/.git/objects/d9/04d142c9bf7ef514a7a46daf1a1a63daffb3ec
+domain_admin/public/.git/objects/df/90cac9bc9a446000e264e59d549b7b0144fbdc
 domain_admin/public/.git/objects/e1/13bfd922675ce50e68cdf88cd94d16130ad58b
-domain_admin/public/.git/objects/fb/d49bf5e92b08848a3c75b285c90c0100d7b440
+domain_admin/public/.git/objects/e2/ae3e466505ab377291c9bc893b36ea4e4cc346
+domain_admin/public/.git/objects/ea/014768708683bab0f086bbe7bbbee4bd721482
+domain_admin/public/.git/objects/f1/d1775a53fb6d01f3cf868d7675175acb4972e5
+domain_admin/public/.git/objects/fa/b7c448af6beaf517ef73175a858b241978b57d
 domain_admin/public/.git/objects/fd/bd32c675f85af4ed57021ac0638a21a3c6cad3
+domain_admin/public/.git/objects/ff/3abe67801fd71004bf50541b8e22677539048b
 domain_admin/public/.git/objects/ff/9c65dfdc7a16150c07745e0030a9d6373920cd
 domain_admin/public/.git/refs/heads/dist
 domain_admin/public/.git/refs/remotes/origin/dist
 domain_admin/public/css/ConditionFilterGroup.a91875e6.css
 domain_admin/public/css/index.563210a3.css
 domain_admin/public/css/index.69a97337.css
 domain_admin/public/css/index.a676cc2e.css
 domain_admin/public/css/index.b285e10a.css
 domain_admin/public/css/index.d028ae37.css
 domain_admin/public/gif/user-avatar.ea67286d.gif
 domain_admin/public/jpg/chatpet-white.10f4f36c.jpg
 domain_admin/public/jpg/chatpet.fce5580e.jpg
-domain_admin/public/js/ConditionFilterGroup.98203553.js
-domain_admin/public/js/ConnectStatus.afc51e5e.js
-domain_admin/public/js/SelectGroup.c4ef5dae.js
+domain_admin/public/js/ConditionFilterGroup.345e94e7.js
+domain_admin/public/js/ConnectStatus.b684931b.js
+domain_admin/public/js/SelectGroup.f3c9557e.js
 domain_admin/public/js/element-icon.1ce1c350.js
 domain_admin/public/js/element-plus.c20bc0dd.js
 domain_admin/public/js/event-enums.6c6f25e7.js
-domain_admin/public/js/index.18819e48.js
-domain_admin/public/js/index.1a48d33b.js
-domain_admin/public/js/index.4846c617.js
-domain_admin/public/js/index.5aa6512c.js
-domain_admin/public/js/index.730c57dc.js
-domain_admin/public/js/index.a12c098a.js
-domain_admin/public/js/index.b5155817.js
-domain_admin/public/js/index.c5fb6f8c.js
-domain_admin/public/js/index.deda20cc.js
-domain_admin/public/js/index.e036cf3b.js
-domain_admin/public/js/index.f2a38d9e.js
-domain_admin/public/js/index.fd336ece.js
+domain_admin/public/js/index.0454165e.js
+domain_admin/public/js/index.1ca9564a.js
+domain_admin/public/js/index.2f7d52d5.js
+domain_admin/public/js/index.6e09f947.js
+domain_admin/public/js/index.b0fe3ecf.js
+domain_admin/public/js/index.b12ea372.js
+domain_admin/public/js/index.b862d533.js
+domain_admin/public/js/index.d48aa76e.js
+domain_admin/public/js/index.d5eedcdd.js
+domain_admin/public/js/index.de952ab7.js
+domain_admin/public/js/index.fd8734f6.js
+domain_admin/public/js/index.fe4c8ff8.js
 domain_admin/public/js/vendor-lib.cb4f08bf.js
 domain_admin/public/js/vendor-vue.9e61e0af.js
 domain_admin/public/m/index.html
 domain_admin/public/m/.git/FETCH_HEAD
 domain_admin/public/m/.git/HEAD
 domain_admin/public/m/.git/config
 domain_admin/public/m/.git/description
```

### Comparing `domain-admin-1.5.0/setup.py` & `domain-admin-1.5.1/setup.py`

 * *Files identical despite different names*

