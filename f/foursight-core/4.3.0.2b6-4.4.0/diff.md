# Comparing `tmp/foursight_core-4.3.0.2b6.tar.gz` & `tmp/foursight_core-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.2b6.tar", max compression
+gzip compressed data, was "foursight_core-4.4.0.tar", max compression
```

## Comparing `foursight_core-4.3.0.2b6.tar` & `foursight_core-4.4.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-07-02 11:28:50.142682 foursight_core-4.3.0.2b6/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/app.py
--rw-r--r--   0        0        0   103608 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/app_utils.py
--rw-r--r--   0        0        0     1283 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/boto_s3.py
--rw-r--r--   0        0        0     1305 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/boto_sqs.py
--rw-r--r--   0        0        0     2589 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-07-02 11:28:50.150683 foursight_core-4.3.0.2b6/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     7293 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/decorators.py
--rw-r--r--   0        0        0    15846 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/deploy.py
--rw-r--r--   0        0        0     8169 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/environment.py
--rw-r--r--   0        0        0    11948 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5597 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3061 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6098 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6373 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     4096 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5214 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    87984 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    35908 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11953 2023-07-02 11:28:50.154682 foursight_core-4.3.0.2b6/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1862228 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/routes.py
--rw-r--r--   0        0        0    22941 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/run_result.py
--rw-r--r--   0        0        0     6380 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     5442 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1500 2023-07-02 11:28:50.166683 foursight_core-4.3.0.2b6/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-16 13:33:02.440657 foursight_core-4.4.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-16 13:33:02.444657 foursight_core-4.4.0/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-07-16 13:33:02.444657 foursight_core-4.4.0/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-07-16 13:33:02.444657 foursight_core-4.4.0/foursight_core/app.py
+-rw-r--r--   0        0        0   103901 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/boto_s3.py
+-rw-r--r--   0        0        0     1305 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/boto_sqs.py
+-rw-r--r--   0        0        0     2589 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     7293 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15846 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8235 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/environment.py
+-rw-r--r--   0        0        0    11948 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5641 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     7218 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3061 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6098 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6373 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     4096 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0    10609 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5214 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    98198 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    36818 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    12028 2023-07-16 13:33:02.448657 foursight_core-4.4.0/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1868943 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/routes.py
+-rw-r--r--   0        0        0    22941 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6380 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     5442 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-07-16 13:33:02.460657 foursight_core-4.4.0/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1471 2023-07-16 13:33:02.460657 foursight_core-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 foursight_core-4.4.0/PKG-INFO
```

### Comparing `foursight_core-4.3.0.2b6/LICENSE.txt` & `foursight_core-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/abstract_connection.py` & `foursight_core-4.4.0/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/app_utils.py` & `foursight_core-4.4.0/foursight_core/app_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,26 +169,27 @@
         Generate environment information from the envs bucket in s3.
         Returns a dictionary keyed by environment name with value of a sub-dict
         with the fields needed to initiate a connection.
 
         :param env: allows you to specify a single env to be initialized
         :param envs: allows you to specify multiple envs to be initialized
         """
+        logger.warning(f'In init_environments with args {env} {envs}')
         stage_name = self.stage.get_stage()
         return self.environment.get_environment_and_bucket_info_in_batch(stage=stage_name, env=env, envs=envs)
 
     def init_connection(self, environ, _environments=None):
         """
         Initialize the fourfront/s3 connection using the FSConnection object
         and the given environment.
         Returns an FSConnection object or raises an error.
         """
         environments = self.init_environments(environ) if _environments is None else _environments
         if not environments:
-            environ = self.get_default_env();
+            environ = self.get_default_env()
             environments = self.init_environments(environ) if _environments is None else _environments
         logger.warning("environments = %s" % str(environments))
         # if still not there, return an error
         if environ not in environments:
             error_res = {
                 'status': 'error',
                 'description': f'environment {environ} is not valid!',
@@ -368,17 +369,19 @@
         # previously related to support of a local "faux" login; removed. Should
         # just delete this entire block including this comment next time around.
         jwt_decoded = self.get_decoded_jwt_token(env, request_dict)
         if jwt_decoded:
             try:
                 if env is None:
                     return False  # we have no env to check auth
-                for env_info in self.init_environments(env).values():
+                envs = self.init_environments(env)
+                for env_info in envs.values():
+                    connection = self.init_connection(env, envs)
                     user_res = ff_utils.get_metadata('users/' + jwt_decoded.get('email').lower(),
-                                                     ff_env=env_info['ff_env'],
+                                                     key=connection.ff_keys,
                                                      add_on='frame=object&datastore=database')
                     logger.warning("foursight_core.check_authorization: env_info ...")
                     logger.warning(env_info)
                     logger.warning("foursight_core.check_authorization: user_res ...")
                     logger.warning(user_res)
                     groups = user_res.get('groups')
                     if not groups:
@@ -1065,18 +1068,19 @@
 
     def view_user(self, request, environ, is_admin=False, domain="", context="/", email=None):
         html_resp = Response('Foursight viewing suite')
         html_resp.headers = {'Content-Type': 'text/html'}
         request_dict = request.to_dict()
         stage_name = self.stage.get_stage()
         users = []
+        connection = self.init_connection(environ)
         for this_email in email.split(","):
             try:
                 this_user = ff_utils.get_metadata('users/' + this_email.lower(),
-                                                  ff_env=full_env_name(environ),
+                                                  key=connection.ff_keys,
                                                   add_on='frame=object&datastore=database')
                 users.append({"email": this_email, "record": this_user})
             except Exception as e:
                 users.append({"email": this_email, "record": {"error": str(e)}})
         template = self.jin_env.get_template('user.html')
         html_resp.body = template.render(
             request=request,
@@ -1114,15 +1118,17 @@
     def view_users(self, request, environ, is_admin=False, domain="", context="/"):
         html_resp = Response('Foursight viewing suite')
         html_resp.headers = {'Content-Type': 'text/html'}
         request_dict = request.to_dict()
         stage_name = self.stage.get_stage()
         users = []
         # TODO: Support paging.
-        user_records = ff_utils.get_metadata('users/', ff_env=full_env_name(environ), add_on='frame=object&limit=10000&datastore=database')
+        connection = self.init_connection(environ)
+        user_records = ff_utils.get_metadata('users/', key=connection.ff_keys,
+                                             add_on='frame=object&limit=10000&datastore=database')
         for user_record in user_records["@graph"]:
             last_modified = user_record.get("last_modified")
             if last_modified:
                 last_modified = last_modified.get("date_modified")
             # TODO
             # roles = []
             # project_roles = user_record.get("project_roles")
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/boto_s3.py` & `foursight_core-4.4.0/foursight_core/boto_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/boto_sqs.py` & `foursight_core-4.4.0/foursight_core/boto_sqs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/buckets.py` & `foursight_core-4.4.0/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/check_schema.py` & `foursight_core-4.4.0/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/check_utils.py` & `foursight_core-4.4.0/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.4.0/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.4.0/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/ecs_checks.py` & `foursight_core-4.4.0/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.4.0/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.4.0/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.4.0/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/scaling_checks.py` & `foursight_core-4.4.0/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/checks/test_checks.py` & `foursight_core-4.4.0/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/decorators.py` & `foursight_core-4.4.0/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/deploy.py` & `foursight_core-4.4.0/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/environment.py` & `foursight_core-4.4.0/foursight_core/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return infer_foursight_from_env(envname=env) in valid_envs
 
     @classmethod
     def get_environment_info_from_s3(cls, env_name: EnvName) -> dict:
         return s3Utils.get_synthetic_env_config(env_name)
 
     def get_environment_and_bucket_info(self, env_name: EnvName, stage: ChaliceStage) -> dict:
-
+        logger.warning(f'Getting env info from s3 for {env_name}')
         env_info = self.get_environment_info_from_s3(env_name)
 
         portal_url = env_info['fourfront']
         es_url = env_info['es']
         ff_env = env_info['ff_env']
 
         bucket_name = get_foursight_bucket(envname=env_name, stage=stage)
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/es_connection.py` & `foursight_core-4.4.0/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/exceptions.py` & `foursight_core-4.4.0/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/fs_connection.py` & `foursight_core-4.4.0/foursight_core/fs_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,17 @@
                 self.redis_url = fs_environ_info['redis']
             elif 'REDIS_HOST' in os.environ:  # temporary patch in until env config is fully sorted - Will
                 self.redis_url = os.environ['REDIS_HOST']
             if self.redis_url:
                 self.redis = RedisBase(create_redis_client(url=self.redis_url))
             else:
                 PRINT("Redis URL was not specified in any way so running without Redis.")
-        except redis.exceptions.ConnectionError:
-            PRINT(f"Cannot connect to Redis ({self.redis_url}); but can run without it so continuing.")
+        except redis.exceptions.ConnectionError as e:
+            PRINT(f"Error {str(e)} \n"
+                  f"Cannot connect to Redis ({self.redis_url}); but can run without it so continuing.")
             self.redis = None
             self.redis_url = None
         if self.redis:
             PRINT(f"Redis server is being used: {self.redis_url}")
         else:
             PRINT(f"Redis server is not being used.")
         if not test:
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/identity.py` & `foursight_core-4.4.0/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/mapping.json` & `foursight_core-4.4.0/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/package.py` & `foursight_core-4.4.0/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/auth.py` & `foursight_core-4.4.0/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/auth0_config.py` & `foursight_core-4.4.0/foursight_core/react/api/auth0_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 import requests
 from dcicutils.function_cache_decorator import function_cache
 from dcicutils.misc_utils import get_error_message
 from .misc_utils import get_request_domain, is_running_locally
 
@@ -110,15 +111,22 @@
 
     @function_cache(nocache={})
     def get_config_raw_data(self) -> dict:
         """
         Returns raw data (dictionary) from the Auth0 config URL.
         """
         try:
-            return requests.get(self.get_config_url()).json() or {}
+            auth0_config_response = requests.get(self.get_config_url()).json() or {}
+            allowed_connections = auth0_config_response.get("auth0Options", {}).get("allowedConnections")
+            if isinstance(allowed_connections, str):
+                # Slight temporary hack to deal with fact that at some points in
+                # time the allowedConnections property from the /auth0_config Portal
+                # endpoint returned a JSON-ized string of a ist rather than a list.
+                auth0_config_response["auth0Options"]["allowedConnections"] = json.loads(allowed_connections)
+            return auth0_config_response
         except Exception as e:
             logger.error(f"Exception fetching Auth0 config ({self.get_config_url()}): {get_error_message(e)}")
             return {}
 
     def get_client(self) -> str:
         return self.get_config_data()["client"]
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/aws_network.py` & `foursight_core-4.4.0/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/aws_s3.py` & `foursight_core-4.4.0/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.4.0/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/checks.py` & `foursight_core-4.4.0/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/cognito.py` & `foursight_core-4.4.0/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/encryption.py` & `foursight_core-4.4.0/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/envs.py` & `foursight_core-4.4.0/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/gac.py` & `foursight_core-4.4.0/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/misc_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/misc_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,7 +235,44 @@
     :param value_name: Name of the given value property in the result list of key/value objects; default to "Value".
     :returns: List of key/value objects from the given dictionary as described above.
     """
     result = []
     for key in dictionary:
         result.append({key_name: key, value_name: dictionary[key]})
     return result
+
+
+def longest_common_initial_substring(string_list: list) -> str:
+    """
+    Returns the longest common initial substring among all of the strings in the given list.
+    """
+    if not string_list:
+        return ""
+    min_length = min(len(s) for s in string_list)
+    for i in range(min_length):
+        if any(string_list[j][i] != string_list[0][i] for j in range(1, len(string_list))):
+            return string_list[0][:i]
+    return string_list[0][:min_length]
+
+
+def name_value_list_to_dict(items: list,
+                            name_property_name: str = "name",
+                            value_property_name: str = "value"):
+    """
+    Give a list that looks like this:
+
+      [ { "name": "abc", "value": 123 },
+        { "name": "def", "value": 456 } ]
+
+    Returns a dictionary that looks like this:
+
+      { "abc": 123, "def": 456 }
+
+    If there are duplicate names then takes the value of the last one in the list.
+    """
+    result = {}
+    for item in items:
+        name = item.get(name_property_name)
+        if name:
+            value = item.get(value_property_name)
+            result[name] = value
+    return result
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/react_api.py` & `foursight_core-4.4.0/foursight_core/react/api/react_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 )
 from .encryption import Encryption
 from .encoding_utils import base64_decode_to_json
 from .gac import Gac
 from .misc_utils import (
     get_base_url,
     is_running_locally,
+    longest_common_initial_substring,
+    name_value_list_to_dict,
     sort_dictionary_by_case_insensitive_keys
 )
 from .portal_access_key_utils import get_portal_access_key_info
 from .react_routes import ReactRoutes
 from .react_api_base import ReactApiBase
 from .react_ui import ReactUi
 
@@ -1655,57 +1657,209 @@
 
     def reactapi_aws_secrets(self, secrets_name: str) -> Response:
         return self.create_success_response(Gac.get_secrets(secrets_name))
 
     def reactapi_aws_ecs_clusters(self) -> Response:
         ecs = ECSUtils()
         clusters = ecs.list_ecs_clusters()
-        clusters.sort()
+        def ecs_cluster_arn_to_name(cluster_arn: str) -> str:
+            cluster_arn_parts = cluster_arn.split("/", 1)
+            return cluster_arn_parts[1] if len(cluster_arn_parts) > 1 else cluster_arn
+
+        clusters = [{"cluster_name": ecs_cluster_arn_to_name(arn), "cluster_arn": arn} for arn in clusters]
+        clusters = sorted(clusters, key=lambda item: item["cluster_name"])
         return self.create_success_response(clusters)
 
-    def reactapi_aws_ecs_cluster(self, cluster_name: str) -> Response:
-        # Given cluster_name may be either cluster name or ARN.
-        # We URL-decode because it is not uncommon for the cluster name to contain a slash.
-        cluster_name = urllib.parse.unquote(cluster_name)
+    def reactapi_aws_ecs_cluster(self, cluster_arn: str) -> Response:
+        # Given cluster_name may actually be either a cluster name or its ARN,
+        # e.g. either c4-ecs-cgap-supertest-stack-CGAPDockerClusterForCgapSupertest-YZMGi06YOoSh or
+        # arn:aws:ecs:us-east-1:466564410312:cluster/c4-ecs-cgap-supertest-stack-CGAPDockerClusterForCgapSupertest-YZMGi06YOoSh
+        # URL-decode because the ARN may contain a slash.
+        cluster_arn = urllib.parse.unquote(cluster_arn)
         ecs = ECSUtils()
-        cluster = ecs.client.describe_clusters(clusters=[cluster_name])["clusters"][0]
+        cluster = ecs.client.describe_clusters(clusters=[cluster_arn])["clusters"][0]
         response = {
-            "arn": cluster["clusterArn"],
-            "name": cluster["clusterName"],
+            "cluster_arn": cluster["clusterArn"],
+            "cluster_name": cluster["clusterName"],
             "status": cluster["status"],
             "services": []
         }
         most_recent_deployment_at = None
-        service_arns = ecs.list_ecs_services(cluster_name=cluster_name)
+        service_arns = ecs.list_ecs_services(cluster_name=cluster_arn)
         for service_arn in service_arns:
-            service = ecs.client.describe_services(cluster=cluster_name, services=[service_arn])["services"][0]
+            service = ecs.client.describe_services(cluster=cluster_arn, services=[service_arn])["services"][0]
             deployments = []
             most_recent_update_at = None
+            # Typically we have just one deployment record, but if there are more than one, then the
+            # one with a status of PRIMARY (of which there should be at most one), is the active one,
+            # and we will place that first in the list; all others will go after that.
             for deployment in service.get("deployments", []):
                 if (not most_recent_update_at or
                     (deployment.get("updatedAt") and deployment.get("updatedAt") > most_recent_update_at)):
                     most_recent_update_at = deployment.get("updatedAt")
-                deployments.append({
-                    "id": deployment.get("id"),
-                    "task": deployment.get("taskDefinition"),
+                deployment_status = deployment.get("status")
+                deployment_info = {
+                    "deployment_id": deployment.get("id"),
+                    "task_arn": deployment.get("taskDefinition"),
+                    "task_name": self._ecs_task_definition_arn_to_name(deployment.get("taskDefinition")),
+                    "task_display_name": self._ecs_task_definition_arn_to_name(deployment.get("taskDefinition")),
+                    "status": deployment_status,
+                    "counts": {"running": deployment.get("runningCount"),
+                               "pending": deployment.get("pendingCount"),
+                               "expected": deployment.get("desiredCount")},
+                    "rollout": {"state": deployment.get("rolloutState"),
+                                "reason": deployment.get("rolloutStateReason")},
                     "created": convert_utc_datetime_to_utc_datetime_string(deployment.get("createdAt")),
                     "updated": convert_utc_datetime_to_utc_datetime_string(deployment.get("updatedAt"))
-                })
+                }
+                if deployment_status and deployment_status.upper() == "PRIMARY":
+                    deployments.insert(0, deployment_info)
+                else:
+                    deployments.append(deployment_info)
             if (not most_recent_deployment_at or
                 (most_recent_update_at and most_recent_update_at > most_recent_deployment_at)):
                 most_recent_deployment_at = most_recent_update_at
+            if len(deployments) > 1:
+                task_name_common_prefix = longest_common_initial_substring([deployment["task_name"] for deployment in deployments])
+                if task_name_common_prefix:
+                    for deployment in deployments:
+                        deployment["task_display_name"] = deployment["task_name"][len(task_name_common_prefix):]
             response["services"].append({
-                "arn": service_arn,
-                "name": service.get("serviceName"),
+                "service_arn": service_arn,
+                "service_name": service.get("serviceName"),
+                "service_display_name": service.get("serviceName"),
+                "task_arn": service.get("taskDefinition"),
+                "task_name": self._ecs_task_definition_arn_to_name(service.get("taskDefinition")),
+                "task_display_name": self._ecs_task_definition_arn_to_name(service.get("taskDefinition")),
                 "deployments": deployments
             })
+        if len(response["services"]) > 1:
+            service_name_common_prefix = (
+                longest_common_initial_substring([service["service_name"] for service in response["services"]]))
+            if service_name_common_prefix:
+                for service in response["services"]:
+                    service["service_display_name"] = service["service_name"][len(service_name_common_prefix):]
+            task_name_common_prefix = (
+                longest_common_initial_substring([service["task_name"] for service in response["services"]]))
+            if task_name_common_prefix:
+                for service in response["services"]:
+                    service["task_display_name"] = service["task_name"][len(task_name_common_prefix):]
+
         if most_recent_deployment_at:
-            response["most_recent_deployed"] = convert_utc_datetime_to_utc_datetime_string(most_recent_deployment_at)
+            response["most_recent_deployment_at"] = convert_utc_datetime_to_utc_datetime_string(most_recent_deployment_at)
+        return self.create_success_response(response)
+
+    def reactapi_aws_ecs_task_arns(self, latest: bool = True) -> Response:
+        # If latest is True then only looks for the non-revisioned task ARNs.
+        ecs = boto3.client('ecs')
+        task_definition_arns = ecs.list_task_definitions()['taskDefinitionArns'] # TODO: ecs_utils.list_ecs_tasks
+        if latest:
+            task_definition_arns = list(set([self._ecs_task_definition_arn_to_name(task_definition_arn)
+                                             for task_definition_arn in task_definition_arns]))
+        task_definition_arns.sort()
+        return task_definition_arns
+
+    def reactapi_aws_ecs_tasks(self, latest: bool = True) -> Response:
+        task_definitions = []
+        ecs = boto3.client('ecs')
+        task_definition_arns = ecs.list_task_definitions()['taskDefinitionArns']
+        if latest:
+            task_definition_arns = list(set([self._ecs_task_definition_arn_to_name(task_definition_arn)
+                                             for task_definition_arn in task_definition_arns]))
+        for task_definition_arn in task_definition_arns:
+            task_definition = self._reactapi_aws_ecs_task(task_definition_arn)
+            task_containers = task_definition["task_containers"]
+            task_container_names = [task_container["task_container_name"] for task_container in task_containers]
+            if task_container_names:
+                # If the "name" value of all of the task containers are then same then we
+                # will take this to be the the task display name, e.g. "DeploymentAction".
+                if all(task_container_name == task_container_names[0] for task_container_name in task_container_names):
+                    task_definition["task_display_name"] = task_container_names[0]
+            task_definitions.append(task_definition)
+        # Here we have the flattened out list of task definitions, by revisions,
+        # but we want them (the revisions) to be grouped by task_family, so do that now.
+        response = []
+        for task_definition in task_definitions:
+            task_family = task_definition["task_family"]
+            task_definition_response = [td for td in response if td["task_family"] == task_family]
+            if not task_definition_response:
+                task_definition_response = {
+                    "task_family": task_family,
+                    "task_name": task_definition["task_name"],
+                    "task_display_name": task_definition["task_display_name"],
+                    "task_revisions": []
+                }
+                response.append(task_definition_response)
+            else:
+                task_definition_response = task_definition_response[0]
+            task_definition_response["task_revisions"].append(task_definition)
+        response.sort(key=lambda value: value["task_family"])
         return self.create_success_response(response)
 
+    def reactapi_aws_ecs_task(self, task_definition_arn: str) -> Response:
+        return self.create_success_response(self._reactapi_aws_ecs_task(task_definition_arn))
+
+    def _reactapi_aws_ecs_task(self, task_definition_arn: str) -> Response:
+        # Note that the task_definition_arn can be either the specific task definition revision ARN,
+        # i.e. the one with the trailing ":<revision-number>", or the plain task definition ARN,
+        # i.e. without that trailing revision suffix. If it is the without the revision suffix,
+        # then the latest (most recent, i.e. the revision with the highest number) is returned;
+        # and the ARN prefix, e.g. "arn:aws:ecs:us-east-1:643366669028:task-definition", may be
+        # also be omitted. URL-decode because the ARN may contain a slash.
+        task_definition_arn = urllib.parse.unquote(task_definition_arn)
+        ecs = boto3.client('ecs')
+        task_definition = ecs.describe_task_definition(taskDefinition=task_definition_arn)["taskDefinition"]
+        task_containers = []
+        for task_container in task_definition.get("containerDefinitions", []):
+            task_container_log = task_container.get("logConfiguration", {}).get("options", {})
+            task_containers.append({
+                "task_container_name": task_container["name"],
+                "task_container_image": task_container["image"],
+                "task_container_env": obfuscate_dict(name_value_list_to_dict(task_container["environment"])),
+                "task_container_log_group": task_container_log.get("awslogs-group"),
+                "task_container_log_region": task_container_log.get("awslogs-region"),
+                "task_container_log_stream_prefix": task_container_log.get("awslogs-stream-prefix")
+            })
+        task_definition = {
+            "task_arn": task_definition["taskDefinitionArn"],
+            # The values of the task_family and task_name below should be exactly the same.
+            "task_family": task_definition["family"],
+            "task_name": self._ecs_task_definition_arn_to_name(task_definition_arn),
+            "task_display_name": task_definition["family"],
+            "task_revision": self._ecs_task_definition_revision(task_definition["taskDefinitionArn"]),
+            "task_containers": task_containers
+        }
+        task_container_names = [task_container["task_container_name"] for task_container in task_containers]
+        if task_container_names:
+            # If the "name" value of all of the task containers are then same then we
+            # will take this to be the the task display name, e.g. "DeploymentAction".
+            if all(task_container_name == task_container_names[0] for task_container_name in task_container_names):
+                task_definition["task_display_name"] = task_container_names[0]
+        return task_definition
+
+    @staticmethod
+    def _ecs_task_definition_arn_to_name(task_definition_arn: str) -> str:
+        """
+        Given something like this:
+        - arn:aws:ecs:us-east-1:466564410312:task-definition/c4-ecs-cgap-supertest-stack-CGAPDeployment-of2dr96JX1ds:1
+        this function would return this: 
+        - c4-ecs-cgap-supertest-stack-CGAPDeployment-of2dr96JX1ds
+        """
+        if not task_definition_arn:
+            return ""
+        task_definition_arn_parts = task_definition_arn.split("/", 1)
+        task_definition_name = task_definition_arn_parts[1] if len(task_definition_arn_parts) > 1 else task_definition_arn
+        task_definition_name_parts = task_definition_name.rsplit(":", 1)
+        return task_definition_name_parts[0] if len(task_definition_name_parts) > 1 else task_definition_name
+
+    @staticmethod
+    def _ecs_task_definition_revision(task_definition_arn: str) -> str:
+        task_definition_arn_parts = task_definition_arn.rsplit(":", 1)
+        return task_definition_arn_parts[1] if len(task_definition_arn_parts) > 1 else task_definition_arn
+
     def reactapi_reload_lambda(self, request: dict) -> Response:
         """
         Called from react_routes for endpoint: GET /__reloadlambda__
         Kicks off a reload of the given lambda name. For troubleshooting only.
         """
         ignored(request)
         app.core.reload_lambda()
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/react_api_base.py` & `foursight_core-4.4.0/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.4.0/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/react_routes.py` & `foursight_core-4.4.0/foursight_core/react/api/react_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -647,17 +647,33 @@
     def reactapi_route_aws_secret_names_noenv() -> Response:  # noqa: implicit @staticmethod via @route
         return app.core.reactapi_aws_secret_names()
 
     @route("/aws/ecs/clusters", authorize=True)
     def reactapi_route_aws_ecs_clusters() -> Response:  # noqa: implicit @staticmethod via @route
         return app.core.reactapi_aws_ecs_clusters()
 
-    @route("/aws/ecs/clusters/{cluster_name}", authorize=True)
-    def reactapi_route_aws_ecs_cluster(cluster_name: str) -> Response:  # noqa: implicit @staticmethod via @route
-        return app.core.reactapi_aws_ecs_cluster(cluster_name=cluster_name)
+    @route("/aws/ecs/clusters/{cluster_arn}", authorize=True)
+    def reactapi_route_aws_ecs_cluster(cluster_arn: str) -> Response:  # noqa: implicit @staticmethod via @route
+        return app.core.reactapi_aws_ecs_cluster(cluster_arn=cluster_arn)
+
+    @route("/aws/ecs/tasks", authorize=True)
+    def reactapi_route_aws_ecs_tasks() -> Response:  # noqa: implicit @staticmethod via @route
+        return app.core.reactapi_aws_ecs_task_arns(latest=False)
+
+    @route("/aws/ecs/tasks/{task_definition_arn}", authorize=True)
+    def reactapi_route_aws_ecs_task(task_definition_arn: str) -> Response:  # noqa: implicit @staticmethod via @route
+        if task_definition_arn.lower() == "latest":
+            return app.core.reactapi_aws_ecs_task_arns(latest=True)
+        elif task_definition_arn.lower() == "details":
+            return app.core.reactapi_aws_ecs_tasks(latest=False)
+        return app.core.reactapi_aws_ecs_task(task_definition_arn)
+
+    @route("/aws/ecs/tasks/latest/details", authorize=True)
+    def reactapi_route_aws_ecs_task() -> Response:  # noqa: implicit @staticmethod via @route
+        return app.core.reactapi_aws_ecs_tasks(latest=True)
 
     # ----------------------------------------------------------------------------------------------
     # Foursight React UI (static file) routes, serving the HTML/CSS/JavaScript/React files.
     # Note that ALL of these are UNPROTECTED routes.
     # ----------------------------------------------------------------------------------------------
 
     # TODO: See if there is a better way to deal with variadic paths.
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/react_ui.py` & `foursight_core-4.4.0/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.4.0/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/ui/index.html` & `foursight_core-4.4.0/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.4.0/foursight_core/react/ui/static/css/main.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-.html-scroll{overflow-y:scroll}.container{max-width:1900px;padding-top:10px}.control-form{display:inline;margin-right:20px;margin-top:-8px}.boxstyle{padding:2px 10px}.boxstyle,.group-boxstyle{border:1px solid #ccc;border-radius:8px;margin-bottom:5px}.group-boxstyle{background-color:#f8f8f8;padding:0}.group-boxstyle:hover{background-color:#f2f2f2}.login-w-hover{background-color:#f8f8f8;border:1px solid #ccc;border-radius:8px;font-weight:350}.login-w-hover:hover{background-color:#d9d9d9}.commonstyle{margin:0 10px 5px}.collapse-div{clear:both;overflow:hidden}.own-line{display:block}.action-icon,.in-line{display:inline-block}.action-icon{border-radius:50%;height:11px;width:11px}.assc-action-done{background-color:#55aa57}.assc-action-fail{background-color:#b84947}.assc-action-pend{background-color:#e7c418}.assc-action-ready{background-color:#b6b5b5}.info{background-color:#d6eaf8;color:#263a48}.check-done,.check-pass{background-color:#dff0d8;color:#3c763d}.check-pend,.check-warn{background-color:#fcf8e3;color:#8a6d3b}.check-fail{background-color:#f2dede;color:#a94442}.check-error{background-color:#fbdcbd;color:#b75c00}.check-ignore{display:none}.center-element{text-align:center}.opacity-transition{transition:opacity .5s}.title-image-hover,.title-image-hover:active,.title-image-hover:visited{opacity:.7;text-decoration:none}.title-image-hover:focus,.title-image-hover:hover{opacity:1;text-decoration:none}.title-hover,.title-hover:active,.title-hover:visited{color:inherit}.title-hover:focus,.title-hover:hover{color:#000;text-decoration:none}.top-level-list{padding:0}.no-border{border:none}dl{margin-bottom:0}dd{margin-bottom:5px;margin-left:20px}.dropdown-button{background-color:inherit;border:none;color:inherit;cursor:pointer}.dropdown{display:inline-block;position:relative}.dropdown-content{background-color:inherit;box-shadow:10px 10px 10px #476f86;display:none;min-width:160px;position:absolute;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;z-index:1}.dropdown-content a{background-color:inherit;color:inherit}.dropdown-content a,.dropdown-content span{display:block;padding:4px 80px 4px 8px;text-align:left;text-decoration:none}.dropdown-content span{color:#000;cursor:default}.dropdown-content a:hover{background-color:#365e75;color:#ff0;cursor:pointer}.dropdown-content span:hover{color:blue}.dropdown:hover .dropdown-content{display:block}.dropdown:hover .dropdown-button{color:#000}.check-box{background-color:#dff0d8;color:#3c763d;-webkit-filter:brightness(.95);filter:brightness(.95)}.check-box:hover{-webkit-filter:brightness(1.05);filter:brightness(1.05)}.check-run-button{background:#09430c;background:var(--box-fg);border:1px solid var(--box-fg-darken);border-radius:12px;color:#fff;cursor:pointer;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-run-button.red,.check-run-button.red:hover{background:red}.check-run-button.red:active{background:#ff0;color:red}.check-action-confirm-button{background:#dfe;background:var(--box-bg);border:1px solid red;border-radius:12px;color:red;cursor:pointer;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-run-button:disabled{background:gray;color:#fff}.check-run-button.disabled{cursor:not-allowed}.check-run-button.disabled,.check-run-button.disabled:hover{background:gray;color:#fff!important}.check-run-button.disabled:active{background:gray;color:#fff}.check-run-button:hover{background:#09430c;background:var(--box-fg);color:#ff0}.check-run-button:active{background:#ff0;color:darkred!important}.check-run-wait-button{background:#09430c;background:var(--box-fg);border-radius:12px;color:#ff0;cursor:not-allowed;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-config-button{border:1px solid #006400;border-radius:14px;cursor:pointer}.check-config-button,.check-config-wait-button{background:inherit;color:inherit;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-config-wait-button{border:1px solid #006400;border-radius:12px;cursor:not-allowed}.tool-tip{position:relative}.tool-tip:before{background:#000;border-radius:10px;color:#fff;content:attr(data-text);display:none;font-family:tahoma;font-size:10pt;font-style:italic;font-weight:400;left:100%;margin-left:15px;min-width:200px;padding:8px 10px 8px 15px;position:absolute;text-align:left;top:50%;-webkit-transform:translateY(-50%);transform:translateY(-50%);width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;z-index:99}.tool-tip:hover:before{display:block;z-index:99}.tool-tip.left:before{left:auto;margin:initial;margin-right:15px;right:100%;z-index:99}.tool-tip:after{border:10px solid transparent;border-right-color:#000;content:"";display:none;left:100%;margin-left:-2px;position:absolute;top:50%;-webkit-transform:translateY(-50%);transform:translateY(-50%);z-index:99}.tool-tip:hover:after,.tool-tip:hover:before{display:block}.App{text-align:center}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion:no-preference){.App-logo{-webkit-animation:App-logo-spin 20s linear infinite;animation:App-logo-spin 20s linear infinite}}.App-header{align-items:center;background-color:#282c34;color:#fff;display:flex;flex-direction:column;font-size:calc(10px + 2vmin);justify-content:center;min-height:100vh}.App-link{color:#61dafb}@-webkit-keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@font-face{font-family:Sansation Bold;src:url(https://allfont.ru/cache/fonts/sansation-bold_1ed7ffb329f73655e972f658a6514075.ttf)}.title-font{font-family:Sansation Bold,Arial}:root{--foursight-fourfront-box-bg:#dfe;--foursight-fourfront-box-fg:#09430c;--foursight-cgap-box-bg:#def;--foursight-cgap-box-fg:#000069;--box-fg:var(--foursight-fourfront-box-fg);--box-bg:var(--foursight-fourfront-box-bg)}.box{background:#dfe;background:var(--box-bg);border:1px solid #09430c;border:1px solid var(--box-fg);border-radius:0 10px 10px 10px;color:#09430c;color:var(--box-fg);padding:.6em .8em;vertical-align:middle}.box.margin{margin-top:1.8pt}.box.bigmargin{margin-top:3.6pt}.box.noborder{border:0}.box.thickborder{border:2px solid #09430c;border:2px solid var(--box-fg)}.box.lighten{background:var(--box-bg-lighten)}.box.darken{background:var(--box-bg-darken)}.box.warning{background-color:#fcf8e3;color:#8a6d3b}.box.error{background-color:#ffeeeb;border-color:darkred;color:darkred}.bg{background:#dfe;background:var(--box-bg)}.fgbg{background:#09430c;background:var(--box-fg)}.fg{color:#09430c;color:var(--box-fg)}.td{color:inherit;padding-bottom:4pt;padding-right:8pt;vertical-align:top}.td.thin{width:1%}ul{padding-left:12pt}.input{background:var(--box-bg-lighten);border:1px solid gray;border-radius:4px;height:14pt;margin-left:0;padding:.7em .3em;width:30em}.input:focus{border:1px solid #09430c;border:1px solid var(--box-fg);box-shadow:0 0 2px #09430c;box-shadow:0 0 2px var(--box-fg);outline:none}.input::-webkit-input-placeholder{font-style:italic;opacity:.4}.input::placeholder{font-style:italic;opacity:.4}.input:read-only{background:#dfe;background:var(--box-bg);border:0;box-shadow:0 0 1px #09430c;box-shadow:0 0 1px var(--box-fg);outline:none}.button{background:#09430c;background:var(--box-fg);border:1px solid #09430c;border:1px solid var(--box-fg);border-radius:6px;color:#dfe;color:var(--box-bg);min-width:4em;padding:.1em .4em .25em}.button:active{background:#ff0;color:red}.button:disabled{background:gray;color:#fff;cursor:not-allowed}.button.cancel{background:#dfe;background:var(--box-bg);color:#09430c;color:var(--box-fg);-webkit-filter:brightness(1.02);filter:brightness(1.02)}.button.cancel:active{background:#ff0;color:red}.button.delete{background:red;color:#ff0}.button.delete:active{background:#ff0;color:red}.select{background:var(--box-bg-lighten);border-radius:3px}form{display:inline}.pagination-control *{margin:0}.page-item .page-link,.pagination-control .page-item,.pagination-control .page-link{background:var(--box-bg-lighten);color:#09430c;color:var(--box-fg)}.page-item .active .page-link,.pagination .active .page-link,.pagination.active:hover .page-link{background:#09430c;background:var(--box-fg);color:#dfe;color:var(--box-bg)}.pagination.active:hover .page-link{border-color:#09430c;border-color:var(--box-fg)}.refresh{padding-bottom:15pt;padding-left:2.8pt}.refresh,.refreshing{background:#fff;border:1px solid #09430c;border:1px solid var(--box-fg);border-radius:4pt;color:#09430c;color:var(--box-fg);cursor:pointer;height:16pt;max-height:16pt;max-width:16pt;user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;-webkit-user-select:none;width:16pt}.refreshing{padding-bottom:13.2pt;padding-left:.4pt;padding-top:1.6pt}.refresh:hover{background:#09430c;background:var(--box-fg);border:1px solid #dfe;border:1px solid var(--box-bg);color:#fff}.refresh:active{background:#ff0;border:1px solid red;color:red}.pointer{cursor:pointer}.signin-as-button{background:#ffffe0;border:1px solid #a9a9a9;border-radius:2pt;padding:8pt 0 8pt 10pt;text-align:left;white-space:nowrap;width:100%}.signin-as-button:hover{background:var(--box-bg-lighten)}.signin-as-button:active{background:#ff0}#accounts-file-upload{display:none}.border{border:1px solid}.border-thick{border:2px solid var(--box-fg)}.lightened{-webkit-filter:brightness(1.1);filter:brightness(1.1)}.darkened{-webkit-filter:brightness(.9);filter:brightness(.9)}.vspace-tiny{margin-top:.1em}.vspace-small{margin-top:.2em}.vspace-normal{margin-top:.3em}.vspace-medium{margin-top:.5em}.vspace-large{margin-top:1em}.padding-medium{padding:.5em!important}.padding-small{padding:.2em .5em!important}.mono{font-family:monospace;font-size:.9em}.hline{border-top:1px solid var(--box-fg);height:1px;margin-bottom:.4em;margin-top:.4em}.cursor-hand{cursor:pointer}body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;font-family:tahoma,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;font-size:12pt;margin:0}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}:root{--rt-color-white:#fff;--rt-color-dark:#222;--rt-color-success:#8dc572;--rt-color-error:#be6464;--rt-color-warning:#f0ad4e;--rt-color-info:#337ab7;--rt-opacity:0.9}.core-styles-module_tooltip__3vRRp{left:0;opacity:0;pointer-events:none;position:absolute;top:0;transition:opacity .3s ease-out;visibility:hidden;will-change:opacity,visibility}.core-styles-module_fixed__pcSol{position:fixed}.core-styles-module_arrow__cvMwQ{background:inherit;position:absolute}.core-styles-module_noArrow__xock6{display:none}.core-styles-module_clickable__ZuTTB{pointer-events:auto}.core-styles-module_show__Nt9eE{opacity:.9;opacity:var(--rt-opacity);visibility:visible}.styles-module_tooltip__mnnfp{border-radius:3px;font-size:90%;padding:8px 16px;width:-webkit-max-content;width:max-content}.styles-module_arrow__K0L3T{height:8px;-webkit-transform:rotate(45deg);transform:rotate(45deg);width:8px}.styles-module_dark__xNqje{background:#222;background:var(--rt-color-dark);color:#fff;color:var(--rt-color-white)}.styles-module_light__Z6W-X{background-color:#fff;background-color:var(--rt-color-white);color:#222;color:var(--rt-color-dark)}.styles-module_success__A2AKt{background-color:#8dc572;background-color:var(--rt-color-success);color:#fff;color:var(--rt-color-white)}.styles-module_warning__SCK0X{background-color:#f0ad4e;background-color:var(--rt-color-warning);color:#fff;color:var(--rt-color-white)}.styles-module_error__JvumD{background-color:#be6464;background-color:var(--rt-color-error);color:#fff;color:var(--rt-color-white)}.styles-module_info__BWdHW{background-color:#337ab7;background-color:var(--rt-color-info);color:#fff;color:var(--rt-color-white)}
+.html-scroll{overflow-y:scroll}.container{max-width:1900px;padding-top:10px}.control-form{display:inline;margin-right:20px;margin-top:-8px}.boxstyle{padding:2px 10px}.boxstyle,.group-boxstyle{border:1px solid #ccc;border-radius:8px;margin-bottom:5px}.group-boxstyle{background-color:#f8f8f8;padding:0}.group-boxstyle:hover{background-color:#f2f2f2}.login-w-hover{background-color:#f8f8f8;border:1px solid #ccc;border-radius:8px;font-weight:350}.login-w-hover:hover{background-color:#d9d9d9}.commonstyle{margin:0 10px 5px}.collapse-div{clear:both;overflow:hidden}.own-line{display:block}.action-icon,.in-line{display:inline-block}.action-icon{border-radius:50%;height:11px;width:11px}.assc-action-done{background-color:#55aa57}.assc-action-fail{background-color:#b84947}.assc-action-pend{background-color:#e7c418}.assc-action-ready{background-color:#b6b5b5}.info{background-color:#d6eaf8;color:#263a48}.check-done,.check-pass{background-color:#dff0d8;color:#3c763d}.check-pend,.check-warn{background-color:#fcf8e3;color:#8a6d3b}.check-fail{background-color:#f2dede;color:#a94442}.check-error{background-color:#fbdcbd;color:#b75c00}.check-ignore{display:none}.center-element{text-align:center}.opacity-transition{transition:opacity .5s}.title-image-hover,.title-image-hover:active,.title-image-hover:visited{opacity:.7;text-decoration:none}.title-image-hover:focus,.title-image-hover:hover{opacity:1;text-decoration:none}.title-hover,.title-hover:active,.title-hover:visited{color:inherit}.title-hover:focus,.title-hover:hover{color:#000;text-decoration:none}.top-level-list{padding:0}.no-border{border:none}dl{margin-bottom:0}dd{margin-bottom:5px;margin-left:20px}.dropdown-button{background-color:inherit;border:none;color:inherit;cursor:pointer}.dropdown{display:inline-block;position:relative}.dropdown-content{background-color:inherit;box-shadow:10px 10px 10px #476f86;display:none;min-width:160px;position:absolute;width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;z-index:1}.dropdown-content a{background-color:inherit;color:inherit}.dropdown-content a,.dropdown-content span{display:block;padding:4px 80px 4px 8px;text-align:left;text-decoration:none}.dropdown-content span{color:#000;cursor:default}.dropdown-content a:hover{background-color:#365e75;color:#ff0;cursor:pointer}.dropdown-content span:hover{color:blue}.dropdown:hover .dropdown-content{display:block}.dropdown:hover .dropdown-button{color:#000}.check-box{background-color:#dff0d8;color:#3c763d;-webkit-filter:brightness(.95);filter:brightness(.95)}.check-box:hover{-webkit-filter:brightness(1.05);filter:brightness(1.05)}.check-run-button{background:#09430c;background:var(--box-fg);border:1px solid var(--box-fg-darken);border-radius:12px;color:#fff;cursor:pointer;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-run-button.red,.check-run-button.red:hover{background:red}.check-run-button.red:active{background:#ff0;color:red}.check-action-confirm-button{background:#dfe;background:var(--box-bg);border:1px solid red;border-radius:12px;color:red;cursor:pointer;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-run-button:disabled{background:gray;color:#fff}.check-run-button.disabled{cursor:not-allowed}.check-run-button.disabled,.check-run-button.disabled:hover{background:gray;color:#fff!important}.check-run-button.disabled:active{background:gray;color:#fff}.check-run-button:hover{background:#09430c;background:var(--box-fg);color:#ff0}.check-run-button:active{background:#ff0;color:darkred!important}.check-run-wait-button{background:#09430c;background:var(--box-fg);border-radius:12px;color:#ff0;cursor:not-allowed;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-config-button{border:1px solid #006400;border-radius:14px;cursor:pointer}.check-config-button,.check-config-wait-button{background:inherit;color:inherit;padding:2pt 12pt 3pt 8pt;-webkit-user-select:none;user-select:none}.check-config-wait-button{border:1px solid #006400;border-radius:12px;cursor:not-allowed}.tool-tip{position:relative}.tool-tip:before{background:#000;border-radius:10px;color:#fff;content:attr(data-text);display:none;font-family:tahoma;font-size:10pt;font-style:italic;font-weight:400;left:100%;margin-left:15px;min-width:200px;padding:8px 10px 8px 15px;position:absolute;text-align:left;top:50%;-webkit-transform:translateY(-50%);transform:translateY(-50%);width:-webkit-fit-content;width:-moz-fit-content;width:fit-content;z-index:99}.tool-tip:hover:before{display:block;z-index:99}.tool-tip.left:before{left:auto;margin:initial;margin-right:15px;right:100%;z-index:99}.tool-tip:after{border:10px solid transparent;border-right-color:#000;content:"";display:none;left:100%;margin-left:-2px;position:absolute;top:50%;-webkit-transform:translateY(-50%);transform:translateY(-50%);z-index:99}.tool-tip:hover:after,.tool-tip:hover:before{display:block}.App{text-align:center}.App-logo{height:40vmin;pointer-events:none}@media (prefers-reduced-motion:no-preference){.App-logo{-webkit-animation:App-logo-spin 20s linear infinite;animation:App-logo-spin 20s linear infinite}}.App-header{align-items:center;background-color:#282c34;color:#fff;display:flex;flex-direction:column;font-size:calc(10px + 2vmin);justify-content:center;min-height:100vh}.App-link{color:#61dafb}@-webkit-keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@keyframes App-logo-spin{0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}}@font-face{font-family:Sansation Bold;src:url(https://allfont.ru/cache/fonts/sansation-bold_1ed7ffb329f73655e972f658a6514075.ttf)}.title-font{font-family:Sansation Bold,Arial}:root{--foursight-fourfront-box-bg:#dfe;--foursight-fourfront-box-fg:#09430c;--foursight-cgap-box-bg:#def;--foursight-cgap-box-fg:#000069;--box-fg:var(--foursight-fourfront-box-fg);--box-bg:var(--foursight-fourfront-box-bg)}.box{background:#dfe;background:var(--box-bg);border:1px solid #09430c;border:1px solid var(--box-fg);border-radius:0 10px 10px 10px;color:#09430c;color:var(--box-fg);padding:.6em .8em;vertical-align:middle}.box.margin{margin-top:1.8pt}.box.bigmargin{margin-top:3.6pt}.box.smallpadding{padding:.4em .4em 0}.box.noborder{border:0}.box.thickborder{border:2px solid #09430c;border:2px solid var(--box-fg)}.box.lighten{background:var(--box-bg-lighten)}.box.darken{background:var(--box-bg-darken)}.box.nobackground{background:inherit}.box.warning{background-color:#fcf8e3;color:#8a6d3b}.box.error{background-color:#ffeeeb;border-color:darkred;color:darkred}.bg{background:#dfe;background:var(--box-bg)}.fgbg{background:#09430c;background:var(--box-fg)}.fg{color:#09430c;color:var(--box-fg)}.td{color:inherit;padding-bottom:4pt;padding-right:8pt;vertical-align:top}.td.thin{width:1%}ul{padding-left:12pt}.input{background:var(--box-bg-lighten);border:1px solid gray;border-radius:4px;height:14pt;margin-left:0;padding:.7em .3em;width:30em}.input:focus{border:1px solid #09430c;border:1px solid var(--box-fg);box-shadow:0 0 2px #09430c;box-shadow:0 0 2px var(--box-fg);outline:none}.input::-webkit-input-placeholder{font-style:italic;opacity:.4}.input::placeholder{font-style:italic;opacity:.4}.input:read-only{background:#dfe;background:var(--box-bg);border:0;box-shadow:0 0 1px #09430c;box-shadow:0 0 1px var(--box-fg);outline:none}.button{background:#09430c;background:var(--box-fg);border:1px solid #09430c;border:1px solid var(--box-fg);border-radius:6px;color:#dfe;color:var(--box-bg);min-width:4em;padding:.1em .4em .25em}.button:active{background:#ff0;color:red}.button:disabled{background:gray;color:#fff;cursor:not-allowed}.button.cancel{background:#dfe;background:var(--box-bg);color:#09430c;color:var(--box-fg);-webkit-filter:brightness(1.02);filter:brightness(1.02)}.button.cancel:active{background:#ff0;color:red}.button.delete{background:red;color:#ff0}.button.delete:active{background:#ff0;color:red}.select{background:var(--box-bg-lighten);border-radius:3px}form{display:inline}.pagination-control *{margin:0}.page-item .page-link,.pagination-control .page-item,.pagination-control .page-link{background:var(--box-bg-lighten);color:#09430c;color:var(--box-fg)}.page-item .active .page-link,.pagination .active .page-link,.pagination.active:hover .page-link{background:#09430c;background:var(--box-fg);color:#dfe;color:var(--box-bg)}.pagination.active:hover .page-link{border-color:#09430c;border-color:var(--box-fg)}.refresh{padding-bottom:15pt;padding-left:2.8pt}.refresh,.refreshing{background:#fff;border:1px solid #09430c;border:1px solid var(--box-fg);border-radius:4pt;color:#09430c;color:var(--box-fg);cursor:pointer;height:16pt;max-height:16pt;max-width:16pt;user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;-webkit-user-select:none;width:16pt}.refreshing{padding-bottom:13.2pt;padding-left:.4pt;padding-top:1.6pt}.refresh:hover{background:#09430c;background:var(--box-fg);border:1px solid #dfe;border:1px solid var(--box-bg);color:#fff}.refresh:active{background:#ff0;border:1px solid red;color:red}.pointer{cursor:pointer}.signin-as-button{background:#ffffe0;border:1px solid #a9a9a9;border-radius:2pt;padding:8pt 0 8pt 10pt;text-align:left;white-space:nowrap;width:100%}.signin-as-button:hover{background:var(--box-bg-lighten)}.signin-as-button:active{background:#ff0}#accounts-file-upload{display:none}.border{border:1px solid}.border-thick{border:2px solid var(--box-fg)}.lightened{-webkit-filter:brightness(1.1);filter:brightness(1.1)}.darkened{-webkit-filter:brightness(.9);filter:brightness(.9)}.vspace-tiny{margin-top:.1em}.vspace-small{margin-top:.2em}.vspace-normal{margin-top:.3em}.vspace-medium{margin-top:.5em}.vspace-large{margin-top:1em}.padding-medium{padding:.5em!important}.padding-small{padding:.2em .5em!important}.mono{font-family:monospace;font-size:.9em}.hline{border-top:1px solid var(--box-fg);height:1px;margin-bottom:.4em;margin-top:.4em}.cursor-hand{cursor:pointer}body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;font-family:tahoma,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;font-size:12pt;margin:0}code{font-family:source-code-pro,Menlo,Monaco,Consolas,Courier New,monospace}:root{--rt-color-white:#fff;--rt-color-dark:#222;--rt-color-success:#8dc572;--rt-color-error:#be6464;--rt-color-warning:#f0ad4e;--rt-color-info:#337ab7;--rt-opacity:0.9}.core-styles-module_tooltip__3vRRp{left:0;opacity:0;pointer-events:none;position:absolute;top:0;transition:opacity .3s ease-out;visibility:hidden;will-change:opacity,visibility}.core-styles-module_fixed__pcSol{position:fixed}.core-styles-module_arrow__cvMwQ{background:inherit;position:absolute}.core-styles-module_noArrow__xock6{display:none}.core-styles-module_clickable__ZuTTB{pointer-events:auto}.core-styles-module_show__Nt9eE{opacity:.9;opacity:var(--rt-opacity);visibility:visible}.styles-module_tooltip__mnnfp{border-radius:3px;font-size:90%;padding:8px 16px;width:-webkit-max-content;width:max-content}.styles-module_arrow__K0L3T{height:8px;-webkit-transform:rotate(45deg);transform:rotate(45deg);width:8px}.styles-module_dark__xNqje{background:#222;background:var(--rt-color-dark);color:#fff;color:var(--rt-color-white)}.styles-module_light__Z6W-X{background-color:#fff;background-color:var(--rt-color-white);color:#222;color:var(--rt-color-dark)}.styles-module_success__A2AKt{background-color:#8dc572;background-color:var(--rt-color-success);color:#fff;color:var(--rt-color-white)}.styles-module_warning__SCK0X{background-color:#f0ad4e;background-color:var(--rt-color-warning);color:#fff;color:var(--rt-color-white)}.styles-module_error__JvumD{background-color:#be6464;background-color:var(--rt-color-error);color:#fff;color:var(--rt-color-white)}.styles-module_info__BWdHW{background-color:#337ab7;background-color:var(--rt-color-info);color:#fff;color:var(--rt-color-white)}
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.4.0/foursight_core/react/ui/static/js/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.57815041.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.3d14a79e.js.LICENSE.txt */ ! function() {
     var e = {
             3339: function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.RawSha256 = void 0;
                 var r = n(3277),
@@ -42303,21 +42303,25 @@
                         return void 0 !== e && null !== e && e.constructor === String && e.length > 0
                     },
                     FormatBytes: function(e) {
                         for (var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 2, n = 0; e > 1024; n++) e /= 1024;
                         return parseFloat(e.toFixed(t)) + " " + ["B", "KB", "MB", "GB", "TB", "PB"][n]
                     },
                     LongestCommonInitialSubstring: function(e) {
+                        var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                         if (!Array.isArray(e) || e.length <= 1) return "";
-                        for (var t = e[0], n = "", r = 0; r < t.length; r++) {
-                            for (var o = t[r], i = 1; i < e.length; i++)
-                                if (e[i][r] !== o) return n;
-                            n += o
+                        "function" == typeof t && (e = e.map((function(e) {
+                            return t(e)
+                        })));
+                        for (var n = e[0], r = "", o = 0; o < n.length; o++) {
+                            for (var i = n[o], a = 1; a < e.length; a++)
+                                if (e[a][o] !== i) return r;
+                            r += i
                         }
-                        return n
+                        return r
                     }
                 },
                 wt = bt;
 
             function xt(e) {
                 return void 0 !== e && null !== e && e.constructor === Object
             }
@@ -44369,14 +44373,17 @@
                                 if (n) {
                                     t.selectNode(n);
                                     var r = window.getSelection();
                                     r.removeAllRanges(), r.addRange(t), document.execCommand("copy"), r.removeAllRanges()
                                 }
                             }
                         }
+                    },
+                    CopyText: function(e) {
+                        navigator.clipboard.writeText(e)
                     }
                 },
                 ho = n(5223),
                 go = n.n(ho),
                 yo = n(3021),
                 mo = n.n(yo),
                 vo = n(8334),
@@ -46884,16 +46891,95 @@
                             })]
                         }), e.tooltip && (0, wo.jsx)(oa, {
                             id: e.href,
                             text: e.tooltip
                         })]
                     })
                 },
-                ca = function(e) {
-                    var n = Fa(),
+                ca = {
+                    FormatDateTime: function(e) {
+                        var n = e.verbose,
+                            r = void 0 !== n && n,
+                            o = e.timezone,
+                            i = void 0 === o || o,
+                            a = l((0, t.useState)(new Date), 2),
+                            s = a[0],
+                            u = a[1];
+                        return (0, t.useEffect)((function() {
+                            var e = setInterval((function() {
+                                return u(new Date)
+                            }), 1100);
+                            return function() {
+                                return clearInterval(e)
+                            }
+                        }), []), (0, wo.jsx)(wo.Fragment, {
+                            children: uo.FormatDateTime(s, r, i)
+                        })
+                    },
+                    FormatDuration: function(e) {
+                        var n = e.start,
+                            r = void 0 === n ? null : n,
+                            o = e.end,
+                            i = void 0 === o ? null : o,
+                            a = e.verbose,
+                            s = void 0 !== a && a,
+                            u = e.fallback,
+                            c = void 0 === u ? "" : u,
+                            d = e.prefix,
+                            p = void 0 === d ? "" : d,
+                            f = e.suffix,
+                            h = void 0 === f ? "" : f,
+                            g = e.tooltip,
+                            y = void 0 !== g && g;
+                        "datetime" === p && (p = uo.FormatDateTime(r || i) + " |");
+                        var m = l((0, t.useState)(new Date), 2),
+                            v = m[0],
+                            M = m[1];
+                        return (0, t.useEffect)((function() {
+                            var e = setInterval((function() {
+                                M(new Date)
+                            }), 1100);
+                            return function() {
+                                return clearInterval(e)
+                            }
+                        }), []), (0, wo.jsx)(wo.Fragment, {
+                            children: (0, wo.jsxs)("span", {
+                                id: y ? "tooltip-timestamp-".concat(r || i) : "",
+                                "data-text": uo.FormatDateTime(r || i),
+                                children: [uo.FormatDuration(r || v, i || v, s, c, p, h), (0, wo.jsx)(oa, {
+                                    id: "tooltip-timestamp-".concat(r || i),
+                                    text: uo.FormatDateTime(r || i)
+                                })]
+                            })
+                        })
+                    }
+                },
+                da = ca,
+                pa = !1,
+                fa = !0,
+                ha = {
+                    Now: function() {
+                        return new Date
+                    },
+                    Format: function(e) {
+                        return uo.FormatDateTime(e, pa, fa, true)
+                    },
+                    Format24: function(e) {
+                        return uo.FormatDateTime(e, pa, fa, true)
+                    },
+                    Format12: function(e) {
+                        return uo.FormatDateTime(e, pa, fa, false)
+                    },
+                    FormatVerbose: function(e) {
+                        return uo.FormatDateTime(e, true, fa, false)
+                    },
+                    Live: da.FormatDateTime
+                },
+                ga = function(e) {
+                    var n = Wa(),
                         r = e.accessKey,
                         o = e.error ? "darkred" : "inhert",
                         i = {
                             fontSize: "11pt",
                             color: o,
                             verticalAlign: "top",
                             paddingBottom: "2pt",
@@ -46982,28 +47068,28 @@
                                 }), (0, wo.jsxs)("tr", {
                                     children: [(0, wo.jsx)("td", {
                                         style: a,
                                         children: "Creation Date:"
                                     }), (0, wo.jsx)("td", {
                                         style: i,
                                         children: r.created_at ? (0, wo.jsxs)(wo.Fragment, {
-                                            children: [r.created_at, "\xa0", po.RightArrow, "\xa0", (0, wo.jsx)("small", {
+                                            children: [ha.Format(r.created_at), "\xa0", po.RightArrow, "\xa0", (0, wo.jsx)("small", {
                                                 children: uo.Ago(r.created_at, !0, !1)
                                             })]
                                         }) : (0, wo.jsx)(wo.Fragment, {
                                             children: "Not available"
                                         })
                                     })]
                                 }), (0, wo.jsxs)("tr", {
                                     children: [(0, wo.jsx)("td", {
                                         style: a,
                                         children: "Expiration Date:"
                                     }), (0, wo.jsxs)("td", {
                                         style: i,
-                                        children: [r.expires_at, r.expires_at ? (0, wo.jsx)(wo.Fragment, {
+                                        children: [ha.Format(r.expires_at), r.expires_at ? (0, wo.jsx)(wo.Fragment, {
                                             children: r.expired ? (0, wo.jsxs)(wo.Fragment, {
                                                 children: ["\xa0\xa0", po.RightArrow, "\xa0\xa0", (0, wo.jsx)("b", {
                                                     children: (0, wo.jsx)("u", {
                                                         children: "Expired"
                                                     })
                                                 }), "\xa0\xa0", po.LeftArrow, "\xa0\xa0", (0, wo.jsx)("small", {
                                                     children: uo.Ago(r.expires_at, !0, !1)
@@ -47085,15 +47171,15 @@
                                         })
                                     })]
                                 })]
                             })
                         })
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                da = function(e) {
+                ya = function(e) {
                     var t, n, r = e.header;
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "container",
                             style: {
                                 width: "800pt"
                             },
@@ -47140,23 +47226,23 @@
                                             }), " contact your system adminstrator to resolve this issue"]
                                         }), "\xa0\xa0:-("]
                                     })]
                                 }), (0, wo.jsx)(aa, {
                                     top: "6pt",
                                     bottom: "6pt",
                                     color: "darkred"
-                                }), (0, wo.jsx)(ca, {
+                                }), (0, wo.jsx)(ga, {
                                     accessKey: null === r || void 0 === r ? void 0 : r.portal_access_key,
                                     error: !0
                                 })]
                             })
                         })
                     })
                 },
-                pa = function(e) {
+                ma = function(e) {
                     var n = e.certificate,
                         r = e.error ? "darkred" : "inhert",
                         o = {
                             fontSize: "11pt",
                             color: r,
                             verticalAlign: "top",
                             paddingBottom: "2pt",
@@ -47415,15 +47501,15 @@
                                         })
                                     })]
                                 })]
                             })
                         })
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                fa = function(e) {
+                va = function(e) {
                     var t, n, r, o = e.header;
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "container",
                             style: {
                                 width: "800pt"
                             },
@@ -47467,134 +47553,134 @@
                                             }), " contact your system adminstrator to resolve this issue"]
                                         }), "\xa0\xa0:-("]
                                     })]
                                 }), (0, wo.jsx)(aa, {
                                     top: "6pt",
                                     bottom: "6pt",
                                     color: "darkred"
-                                }), (0, wo.jsx)(pa, {
+                                }), (0, wo.jsx)(ma, {
                                     certificate: null === o || void 0 === o || null === (r = o.portal) || void 0 === r ? void 0 : r.ssl_certificate,
                                     error: !0
                                 })]
                             })
                         })
                     })
                 },
-                ha = function(e) {
+                Ma = function(e) {
                     return null === e || void 0 === e ? void 0 : e.portal_access_key_error
                 },
-                ga = function(e) {
+                ja = function(e) {
                     var t;
                     return null === e || void 0 === e || null === (t = e.portal) || void 0 === t ? void 0 : t.ssl_certificate_error
                 },
-                ya = function(e) {
-                    var t = Fa();
+                ba = function(e) {
+                    var t = Wa();
                     return (0, wo.jsxs)(wo.Fragment, {
-                        children: [ha(t) && (0, wo.jsx)(da, {
+                        children: [Ma(t) && (0, wo.jsx)(ya, {
                             header: t
-                        }), ga(t) && (0, wo.jsx)(fa, {
+                        }), ja(t) && (0, wo.jsx)(va, {
                             header: t
                         })]
                     })
                 };
-            ya.IsFatalError = function(e) {
-                return ga(e) || ha(e)
+            ba.IsFatalError = function(e) {
+                return ja(e) || Ma(e)
             };
-            var ma = ya;
+            var wa = ba;
 
-            function va(e) {
+            function xa(e) {
                 var t = tn.PreferredName(tn.Default(e), e);
                 if (tn.IsKnown(t, e)) {
                     var n = $r.Path($r.CurrentLogicalPath(), t);
                     n !== window.location.href && (window.location.href = n)
                 }
             }
 
-            function Ma() {
+            function Na() {
                 var e = window.location.pathname.substring(1).split("/");
                 return e.length >= 2 && ("api" !== e[0] || "react" !== e[1]) && ("react" === e[0] ? (window.location.pathname = "/api/".concat(e.join("/")), !0) : ("api" === e[0] && e.shift(), window.location.pathname = "/api/react/".concat(e.join("/")), !0))
             }
 
-            function ja(e) {
+            function Ia(e) {
                 tn.IsKnown(tn.Current(), e) && Bt.SetLastUrl(window.location.href)
             }
 
-            function ba() {
+            function Da() {
                 return Bt.LastUrl() || $r.HomeUrl()
             }
-            var wa = {
+            var La = {
                 AuthorizationRequired: function(e) {
                     var t = e.children,
-                        n = Fa();
-                    return ma.IsFatalError(n) ? (0, wo.jsx)(ze, {
+                        n = Wa();
+                    return wa.IsFatalError(n) ? (0, wo.jsx)(ze, {
                         to: $r.Path("/error"),
                         replace: !0
-                    }) : Ma() ? void 0 : co.IsLoggedIn(n) ? tn.IsKnown(tn.Current(), n) ? tn.IsAllowed(tn.Current(), n) ? (ja(), t) : (0, wo.jsx)(ze, {
+                    }) : Na() ? void 0 : co.IsLoggedIn(n) ? tn.IsKnown(tn.Current(), n) ? tn.IsAllowed(tn.Current(), n) ? (Ia(), t) : (0, wo.jsx)(ze, {
                         to: $r.Path("/env"),
                         replace: !0
-                    }) : va(n) : (0, wo.jsx)(ze, {
+                    }) : xa(n) : (0, wo.jsx)(ze, {
                         to: $r.Path("/login"),
                         replace: !0
                     })
                 },
                 KnownEnvRequired: function(e) {
                     var t = e.children,
-                        n = Fa();
-                    if (ma.IsFatalError(n)) {
+                        n = Wa();
+                    if (wa.IsFatalError(n)) {
                         var r = tn.PreferredName(tn.Default(n), n);
                         return (0, wo.jsx)(ze, {
                             to: $r.Path("/error", r),
                             replace: !0
                         })
                     }
-                    if (!Ma()) return n.loading ? t : tn.IsKnown(tn.Current(), n) ? (ja(), t) : va(n)
+                    if (!Na()) return n.loading ? t : tn.IsKnown(tn.Current(), n) ? (Ia(), t) : xa(n)
                 },
                 LastPath: function() {
-                    var e = ba(),
+                    var e = Da(),
                         t = $r.BaseUrl();
                     return e.startsWith(t) ? $r.Path(e.substring(t.length), !1) : e
                 },
-                LastUrl: ba,
-                NoteLastUrl: ja,
+                LastUrl: Da,
+                NoteLastUrl: Ia,
                 Unprotected: function(e) {
                     return e.children
                 }
             };
-            var xa = function() {
-                    Bt.DeleteAuth(), Bt.SetRedirect(wa.LastUrl()), window.location.replace(rn.Url("/logout"))
+            var Sa = function() {
+                    Bt.DeleteAuth(), Bt.SetRedirect(La.LastUrl()), window.location.replace(rn.Url("/logout"))
                 },
-                Na = n(599),
-                Ia = {
+                ka = n(599),
+                Ca = {
                     Format: function(e) {
                         var t;
-                        return null === (t = Na.stringify(e)) || void 0 === t ? void 0 : t.trimLeft()
+                        return null === (t = ka.stringify(e)) || void 0 === t ? void 0 : t.trimLeft()
                     }
                 },
-                Da = function() {
+                Ea = function() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null;
                     return "function" === typeof e && (e = e()), {
                         value: e,
                         __listeners: new Set
                     }
                 },
-                La = function(e) {
+                Ta = function(e) {
                     var n = l((0, t.useState)(), 2)[1];
                     return (0, t.useEffect)((function() {
                         return e.__listeners.add(n),
                             function() {
                                 return e.__listeners.delete(n)
                             }
                     }), [e.value, e.__listeners]), [e.value, function(t) {
                         e.value = t, e.__listeners.forEach((function(e) {
                             return e({})
                         }))
                     }]
                 },
-                Sa = Bt.TestMode.FetchSleep(),
-                ka = function(e, n) {
+                Aa = Bt.TestMode.FetchSleep(),
+                za = function(e, n) {
                     var r = Dt.IsObject(e) ? e.initial : Dt.IsObject(n) ? n.initial : null,
                         o = l((0, t.useState)(r), 2),
                         i = o[0],
                         a = o[1],
                         s = l((0, t.useState)(!1), 2),
                         u = s[0],
                         d = s[1],
@@ -47603,45 +47689,45 @@
                         g = f[1],
                         y = l((0, t.useState)(!1), 2),
                         m = y[0],
                         v = y[1],
                         M = l((0, t.useState)(null), 2),
                         j = M[0],
                         b = M[1],
-                        w = Ta(),
-                        x = Aa();
+                        w = Ua(),
+                        x = Pa();
 
                     function N() {
-                        return _a(e, n, arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null, a, d, g, v, b, w, x, arguments.length > 2 && void 0 !== arguments[2] && arguments[2])
+                        return Ba(e, n, arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null, a, d, g, v, b, w, x, arguments.length > 2 && void 0 !== arguments[2] && arguments[2])
                     }
                     var I = N(),
                         D = {
                             loading: u,
                             data: i,
                             status: h,
                             error: j,
                             timeout: m,
                             set: a,
                             __usefetch_response: !0
                         };
                     return D.fetch = function(e, t) {
-                            Oa(N(e, t, !0), this && !0 === this.__usefetch_response ? this.data : void 0, this)
+                            Fa(N(e, t, !0), this && !0 === this.__usefetch_response ? this.data : void 0, this)
                         }.bind(D), D.refresh = function(e, t) {
-                            Oa(nt(nt({}, N(e, t, !0)), {}, {
+                            Fa(nt(nt({}, N(e, t, !0)), {}, {
                                 nocache: !0
                             }), this && !0 === this.__usefetch_response ? this.data : void 0, this)
                         }.bind(D), D.update = function(e) {
                             var t;
                             void 0 === e && (e = this), !0 === (null === (t = e) || void 0 === t ? void 0 : t.__usefetch_response) && (e = e.data),
                                 function(e, t) {
                                     var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : void 0;
                                     Object.is(t, n) ? Dt.IsObject(t) ? e(nt({}, t)) : Dt.IsArray(t) ? e(Dt.CopyArrayProperties(t, p(t))) : Dt.IsFunction(t) ? e(t()) : e(t) : e(t)
                                 }(a, e, this && this.__usefetch_response ? this.data : void 0)
                         }.bind(D), D.uncache = function(e, t) {
-                            I.cache && za[e] && delete za[e]
+                            I.cache && Ra[e] && delete Ra[e]
                         }.bind(D),
                         function(e) {
                             e.__response = !0, Object.defineProperty(e, "length", {
                                 get: function() {
                                     if (this && this.__response) return Dt.IsArray(this.data) ? this.data.length : void 0
                                 }.bind(e)
                             }), Object.defineProperty(e, "null", {
@@ -47724,24 +47810,24 @@
                                     var r = this.get(n);
                                     Dt.IsArray(r) && r.forEach(e)
                                 }
                             }.bind(e), e.json = function() {
                                 var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                                 if (this && this.__response) return Dt.IsBoolean(e) && e ? no.Format(this.data) : no.Str(this.data)
                             }.bind(e), e.yaml = function() {
-                                if (this && this.__response) return Ia.Format(this.data)
+                                if (this && this.__response) return Ca.Format(this.data)
                             }.bind(e)
                         }(D), (0, t.useEffect)((function() {
-                            Oa(I, void 0, D)
+                            Fa(I, void 0, D)
                         }), [I.url]), D
                 },
-                Ca = Da(new Map),
-                Ea = Da([]),
-                Ta = function() {
-                    var e = l(La(Ca), 2),
+                Oa = Ea(new Map),
+                _a = Ea([]),
+                Ua = function() {
+                    var e = l(Ta(Oa), 2),
                         t = e[0],
                         n = e[1];
                     return {
                         value: t,
                         add: function(e) {
                             var r = Jr()();
                             return e.id = r, e.timestamp = new Date, t.set(r, e), n(t), r
@@ -47751,36 +47837,36 @@
                             return t.delete(e), n(t), r
                         },
                         clear: function() {
                             t.clear(), n(t)
                         }
                     }
                 },
-                Aa = function() {
-                    var e = l(La(Ea), 2),
+                Pa = function() {
+                    var e = l(Ta(_a), 2),
                         t = e[0],
                         n = e[1];
                     return {
                         value: t,
                         add: function(e, r) {
                             e.data = r, e.duration = new Date - e.timestamp, t.length >= 25 && t.shift(), t.push(e), n(t)
                         },
                         clear: function() {
                             t.length = 0, n(t)
                         }
                     }
                 },
-                za = {};
+                Ra = {};
 
-            function Oa(e) {
+            function Fa(e) {
                 var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0,
                     n = arguments.length > 2 ? arguments[2] : void 0;
                 if (!e.nofetch && wt.HasValue(e.url)) {
                     if (e.cache && !e.nocache) {
-                        var r = za[e.url];
+                        var r = Ra[e.url];
                         if (r) return to.Info("FETCH FOUND CACHED RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(r.status)), e.onData(r.data, r.data), e.setData(r.data), e.setStatus(r.status), e.setLoading(!1), e.setTimeout(!1), e.setError(null), n || (n = {
                             data: r.data,
                             loading: !1,
                             status: r.status,
                             timeout: !1,
                             error: null
                         }), e.onSuccess(n), void e.onDone(n)
@@ -47820,51 +47906,51 @@
                                         loading: !1,
                                         data: d,
                                         status: c,
                                         error: t,
                                         timeout: p
                                     }
                                 }
-                                401 === c ? (to.Info("FETCH UNAUTHENTICATED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.nologout || (f(), xa())) : 403 === c ? (to.Info("FETCH UNAUTHORIZED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.noredirect || "/env" !== $r.CurrentLogicalPath() && (f(), window.location.pathname = $r.Path("/env"))) : "ECONNABORTED" === t.code ? (to.Info("FETCH TIMEOUT ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), p = !0, c || (c = 504)) : "ERR_NETWORK" === t.code ? (to.Info("FETCH NETWORK ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), c || (c = 404)) : to.Info("FETCH ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c));
+                                401 === c ? (to.Info("FETCH UNAUTHENTICATED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.nologout || (f(), Sa())) : 403 === c ? (to.Info("FETCH UNAUTHORIZED ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), e.noredirect || "/env" !== $r.CurrentLogicalPath() && (f(), window.location.pathname = $r.Path("/env"))) : "ECONNABORTED" === t.code ? (to.Info("FETCH TIMEOUT ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), p = !0, c || (c = 504)) : "ERR_NETWORK" === t.code ? (to.Info("FETCH NETWORK ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c)), c || (c = 404)) : to.Info("FETCH ERROR: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(c));
                                 var h = f();
                                 s(r), void 0 !== (d = e.onError(h)) && (n && (n.data = d), e.setData(d)), e.onDone(h)
                             }(t, i)
                     }))
                 }
 
                 function a(r, o) {
                     var i = r.status;
                     to.Info("FETCH RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(i), r.data);
                     var a = e.onData(r.data, t);
-                    void 0 === a && (a = r.data), n && (n.status = i, n.data = a, n.loading = !1), e.setStatus(i), e.setData(a), e.setLoading(!1), s(o, a), e.onSuccess(n), e.onDone(n), e.cache && (to.Info("FETCH CACHING RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(i)), za[e.url] = {
+                    void 0 === a && (a = r.data), n && (n.status = i, n.data = a, n.loading = !1), e.setStatus(i), e.setData(a), e.setLoading(!1), s(o, a), e.onSuccess(n), e.onDone(n), e.cache && (to.Info("FETCH CACHING RESPONSE: ".concat(e.method, " ").concat(e.url, " -> HTTP ").concat(i)), Ra[e.url] = {
                         data: a,
                         status: i
                     })
                 }
 
                 function s(t) {
                     var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                     e.fetched.add(e.fetching.remove(t), n)
                 }
             }
 
-            function _a(e, t, n, r, o, i, a, s, u, l, c, d) {
+            function Ba(e, t, n, r, o, i, a, s, u, l, c, d) {
                 var p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k, C, E, T, A, z, O, _, U, P, R, F, B;
                 return Dt.IsObject(e) && (t = e, e = null), Dt.IsObject(n) && (r = n, n = null), t = {
                     url: Dt.First([n, null === (p = r) || void 0 === p ? void 0 : p.url, e, null === (f = t) || void 0 === f ? void 0 : f.url, ""], wt.HasValue),
                     method: Dt.First([null === (h = r) || void 0 === h ? void 0 : h.method, null === (g = t) || void 0 === g ? void 0 : g.method, "GET"], wt.HasValue),
                     payload: Dt.First([null === (y = r) || void 0 === y ? void 0 : y.payload, null === (m = t) || void 0 === m ? void 0 : m.payload, null], Dt.IsJson),
                     timeout: Dt.First([null === (v = r) || void 0 === v ? void 0 : v.timeout, null === (M = t) || void 0 === M ? void 0 : M.timeout, 3e4], Dt.IsInteger),
                     initial: Dt.First([null === (j = r) || void 0 === j ? void 0 : j.initial, null === (b = t) || void 0 === b ? void 0 : b.initial, null], (function(e) {
                         return !Dt.IsNull(e)
                     })),
                     nofetch: Dt.First([null === (w = r) || void 0 === w ? void 0 : w.nofetch, null === (x = t) || void 0 === x ? void 0 : x.nofetch, !1], Dt.IsBoolean),
                     nologout: Dt.First([null === (N = r) || void 0 === N ? void 0 : N.nologout, null === (I = t) || void 0 === I ? void 0 : I.nologout, !1], Dt.IsBoolean),
                     noredirect: Dt.First([null === (D = r) || void 0 === D ? void 0 : D.noredirect, null === (L = t) || void 0 === L ? void 0 : L.noredirect, !1], Dt.IsBoolean),
-                    delay: Dt.First([null === (S = r) || void 0 === S ? void 0 : S.delay, null === (k = t) || void 0 === k ? void 0 : k.delay, Sa > 0 ? Sa : 0], Dt.IsInteger),
+                    delay: Dt.First([null === (S = r) || void 0 === S ? void 0 : S.delay, null === (k = t) || void 0 === k ? void 0 : k.delay, Aa > 0 ? Aa : 0], Dt.IsInteger),
                     cache: Dt.First([null === (C = r) || void 0 === C ? void 0 : C.cache, null === (E = t) || void 0 === E ? void 0 : E.cache, null], Dt.IsBoolean),
                     nocache: Dt.First([null === (T = r) || void 0 === T ? void 0 : T.nocache, null === (A = t) || void 0 === A ? void 0 : A.nocache, null], Dt.IsBoolean),
                     onData: Dt.First([null === (z = r) || void 0 === z ? void 0 : z.onData, null === (O = t) || void 0 === O ? void 0 : O.onData, function() {}], Dt.IsFunction),
                     onSuccess: Dt.First([null === (_ = r) || void 0 === _ ? void 0 : _.onSuccess, null === (U = t) || void 0 === U ? void 0 : U.onSuccess, function() {}], Dt.IsFunction),
                     onError: Dt.First([null === (P = r) || void 0 === P ? void 0 : P.onError, null === (R = t) || void 0 === R ? void 0 : R.onError, function() {}], Dt.IsFunction),
                     onDone: Dt.First([null === (F = r) || void 0 === F ? void 0 : F.onDone, null === (B = t) || void 0 === B ? void 0 : B.onDone, function() {}], Dt.IsFunction),
                     setData: o,
@@ -47872,106 +47958,27 @@
                     setStatus: a,
                     setTimeout: s,
                     setError: u,
                     fetching: l,
                     fetched: c
                 }, d && delete t.nofetch, !wt.HasValue(t.url) || t.url.startsWith("https://") || t.url.startsWith("http://") || (t.url.startsWith("//") ? t.url = rn.Url(t.url.substring(1), !1) : t.url = rn.Url(t.url)), t
             }
-            var Ua = ka,
-                Pa = function(e, t) {
-                    return ka(e, nt(nt({}, t), {}, {
+            var Ya = za,
+                Qa = function(e, t) {
+                    return za(e, nt(nt({}, t), {}, {
                         nofetch: !0
                     }))
                 },
-                Ra = t.createContext({}),
-                Fa = function() {
-                    var e = (0, t.useContext)(Ra);
+                Ga = t.createContext({}),
+                Wa = function() {
+                    var e = (0, t.useContext)(Ga);
                     return e ? e[0] : {}
                 },
-                Ba = {
-                    FormatDateTime: function(e) {
-                        var n = e.verbose,
-                            r = void 0 !== n && n,
-                            o = e.timezone,
-                            i = void 0 === o || o,
-                            a = l((0, t.useState)(new Date), 2),
-                            s = a[0],
-                            u = a[1];
-                        return (0, t.useEffect)((function() {
-                            var e = setInterval((function() {
-                                return u(new Date)
-                            }), 1100);
-                            return function() {
-                                return clearInterval(e)
-                            }
-                        }), []), (0, wo.jsx)(wo.Fragment, {
-                            children: uo.FormatDateTime(s, r, i)
-                        })
-                    },
-                    FormatDuration: function(e) {
-                        var n = e.start,
-                            r = void 0 === n ? null : n,
-                            o = e.end,
-                            i = void 0 === o ? null : o,
-                            a = e.verbose,
-                            s = void 0 !== a && a,
-                            u = e.fallback,
-                            c = void 0 === u ? "" : u,
-                            d = e.prefix,
-                            p = void 0 === d ? "" : d,
-                            f = e.suffix,
-                            h = void 0 === f ? "" : f,
-                            g = e.tooltip,
-                            y = void 0 !== g && g;
-                        "datetime" === p && (p = uo.FormatDateTime(r || i) + " |");
-                        var m = l((0, t.useState)(new Date), 2),
-                            v = m[0],
-                            M = m[1];
-                        return (0, t.useEffect)((function() {
-                            var e = setInterval((function() {
-                                M(new Date)
-                            }), 1100);
-                            return function() {
-                                return clearInterval(e)
-                            }
-                        }), []), (0, wo.jsx)(wo.Fragment, {
-                            children: (0, wo.jsxs)("span", {
-                                id: y ? "tooltip-timestamp-".concat(r || i) : "",
-                                "data-text": uo.FormatDateTime(r || i),
-                                children: [uo.FormatDuration(r || v, i || v, s, c, p, h), (0, wo.jsx)(oa, {
-                                    id: "tooltip-timestamp-".concat(r || i),
-                                    text: uo.FormatDateTime(r || i)
-                                })]
-                            })
-                        })
-                    }
-                },
-                Ya = Ba,
-                Qa = !1,
-                Ga = !0,
-                Wa = {
-                    Now: function() {
-                        return new Date
-                    },
-                    Format: function(e) {
-                        return uo.FormatDateTime(e, Qa, Ga, true)
-                    },
-                    Format24: function(e) {
-                        return uo.FormatDateTime(e, Qa, Ga, true)
-                    },
-                    Format12: function(e) {
-                        return uo.FormatDateTime(e, Qa, Ga, false)
-                    },
-                    FormatVerbose: function(e) {
-                        return uo.FormatDateTime(e, true, Ga, false)
-                    },
-                    Live: Ya.FormatDateTime
-                },
                 Ha = function() {
-                    return [Array.from(La(Ca)[0].values())]
+                    return [Array.from(Ta(Oa)[0].values())]
                 },
                 Va = function(e) {
                     return {
                         __get: function(t, n, r, o) {
                             var i = e.findIndex((function(e) {
                                 return e.type === t
                             }));
@@ -48174,15 +48181,15 @@
                     }
                 };
 
             function es(e) {
                 return /^\*+$/.test(e)
             }
             var ts = function(e) {
-                    var t = Ua("/aws/secrets", {
+                    var t = Ya("/aws/secrets", {
                         cache: !0
                     });
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
                                 children: "AWS Secrets"
                             })
@@ -48213,25 +48220,25 @@
                                     })]
                                 })
                             }))]
                         })]
                     })
                 },
                 ns = function(e) {
-                    var t, n, r, o, i = Ua("/info", {
+                    var t, n, r, o, i = Ya("/info", {
                         cache: !0
                     });
                     return (0, wo.jsx)(os, {
                         name: null === (t = i.data) || void 0 === t || null === (n = t.gac) || void 0 === n ? void 0 : n.name,
                         values: null === (r = i.data) || void 0 === r || null === (o = r.gac) || void 0 === o ? void 0 : o.values,
                         hide: e.hide
                     })
                 },
                 rs = function(e) {
-                    var t = Ua(e.name ? "/aws/secrets/".concat(e.name) : null, {
+                    var t = Ya(e.name ? "/aws/secrets/".concat(e.name) : null, {
                         cache: !1
                     });
                     return e.name ? (0, wo.jsx)(os, {
                         name: e.name,
                         values: null === t || void 0 === t ? void 0 : t.data,
                         hide: e.hide,
                         embedded: e.embedded
@@ -48320,26 +48327,26 @@
                             color: "red"
                         },
                         children: "Expired"
                     }) : t.expires_at ? t.expires_soon ? (0, wo.jsxs)("span", {
                         style: {
                             color: "red"
                         },
-                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", Wa.Format(t.expires_at)]
+                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", ha.Format(t.expires_at)]
                     }) : (0, wo.jsxs)(wo.Fragment, {
-                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", Wa.Format(t.expires_at)]
+                        children: ["Expires ", uo.FromNow(t.expires_at), " ", po.RightArrow, " ", ha.Format(t.expires_at)]
                     }) : (0, wo.jsx)(wo.Fragment, {
                         children: "No expiration"
                     }) : (0, wo.jsx)(wo.Fragment, {
                         children: "\u2013"
                     })
                 },
                 ss = function(e) {
                     var t = e.url,
-                        n = Ua(t ? "/certificates?hostname=".concat(t) : null);
+                        n = Ya(t ? "/certificates?hostname=".concat(t) : null);
                     Jr()();
                     return t && t.startsWith("https://") && (0, wo.jsxs)("small", {
                         children: [(0, wo.jsx)("small", {
                             style: {
                                 marginLeft: "3pt",
                                 marginRight: "3pt"
                             },
@@ -48614,15 +48621,15 @@
                             })
                         })]
                     })
                 },
                 hs = function(e) {
                     var n, r, o, i, a, s, u = e.header,
                         c = e.info,
-                        d = (e.foursightUrl, Ua("/portal_access_key")),
+                        d = (e.foursightUrl, Ya("/portal_access_key")),
                         p = l((0, t.useState)(!1), 2),
                         f = p[0],
                         h = p[1],
                         g = l((0, t.useState)(!1), 2);
                     g[0], g[1];
                     if (!c || c.loading) return (0, wo.jsx)("small", {
                         children: (0, wo.jsx)("i", {
@@ -48915,19 +48922,19 @@
                                             text: "Location of Portal access key in AWS S3.",
                                             position: "bottom"
                                         })]
                                     })]
                                 })]
                             }), (0, wo.jsx)(fs, {}), (0, wo.jsx)(ls, {
                                 title: "Foursight Deployed",
-                                value: "".concat(Wa.Format(c.get("foursight.deployed")), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("foursight.deployed"))),
+                                value: "".concat(ha.Format(c.get("foursight.deployed")), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("foursight.deployed"))),
                                 show: !!c.get("foursight.deployed")
                             }), (0, wo.jsx)(ls, {
                                 title: "Portal Deployed",
-                                value: "".concat(Wa.Format(c.get("portal.started")), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("portal.started")))
+                                value: "".concat(ha.Format(c.get("portal.started")), " ").concat(po.RightArrow, " ").concat(uo.Ago(c.get("portal.started")))
                             })]
                         })
                     })
                 },
                 gs = function(e) {
                     var t = e.info;
                     return !t || t.loading ? (0, wo.jsx)(wo.Fragment, {}) : (0, wo.jsx)("table", {
@@ -49007,15 +49014,15 @@
                 ys = function(e) {
                     var n, r, o, i, a, s, u = e.account,
                         l = e.header,
                         c = e.foursightUrl,
                         d = e.all,
                         p = e.decrementAccountCount,
                         f = e.brighten,
-                        h = Ua("/accounts/".concat(u.id), {
+                        h = Ya("/accounts/".concat(u.id), {
                             onDone: function() {
                                 return p()
                             },
                             cache: !0,
                             nofetch: !0
                         });
                     return (0, t.useEffect)((function() {
@@ -49181,37 +49188,37 @@
                                         border: "1px",
                                         borderTop: "solid"
                                     }
                                 }), (0, wo.jsx)("pre", {
                                     style: {
                                         background: "inherit"
                                     },
-                                    children: Ia.Format(h.data)
+                                    children: Ca.Format(h.data)
                                 })]
                             })]
                         })
                     }) : null
                 },
                 ms = function(e) {
                     var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m = e.header,
-                        v = Ua(rn.Url("/accounts"), {
+                        v = Ya(rn.Url("/accounts"), {
                             method: "POST",
                             nofetch: !0
                         }),
-                        M = Ua(rn.Url("/accounts_file"), {
+                        M = Ya(rn.Url("/accounts_file"), {
                             nocache: !0
                         }),
                         j = l($e(), 2),
                         b = j[0],
                         w = j[1],
                         x = b.get("all"),
                         N = l((0, t.useState)("true" === (null === x || void 0 === x ? void 0 : x.toLowerCase()) || "1" === x), 2),
                         I = N[0],
                         D = N[1],
-                        L = Ua("/accounts", {
+                        L = Ya("/accounts", {
                             cache: !0
                         }),
                         S = l((0, t.useState)(0), 2),
                         k = S[0],
                         C = S[1],
                         E = l((0, t.useState)(!0), 2),
                         T = E[0],
@@ -49442,24 +49449,24 @@
                                         })
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-copy",
                                         text: "Click to copy this accounts info JSON data to the clipboard.",
                                         position: "left"
                                     })]
                                 }), 200 == L.status ? (0, wo.jsxs)(wo.Fragment, {
-                                    children: ["\xa0\xa0", Ia.Format(M.data)]
+                                    children: ["\xa0\xa0", Ca.Format(M.data)]
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: 404 == L.status ? (0, wo.jsx)(wo.Fragment, {
                                         children: no.Format([{
                                             name: "example-account-name",
                                             foursight_url: "https://example-foursight-url/api",
                                             stage: "dev-or-prod"
                                         }])
                                     }) : (0, wo.jsx)(wo.Fragment, {
-                                        children: Ia.Format({})
+                                        children: Ca.Format({})
                                     })
                                 })]
                             })]
                         }), L.length > 0 ? (0, wo.jsxs)(wo.Fragment, {
                             children: [null === L || void 0 === L ? void 0 : L.map((function(e, n) {
                                 return (0, wo.jsx)(t.Fragment, {
                                     children: (0, wo.jsx)(ys, {
@@ -49498,33 +49505,33 @@
                                     children: "No accounts info found."
                                 })
                             })
                         })]
                     })
                 },
                 vs = function(e) {
-                    var t = Fa();
+                    var t = Wa();
                     return (0, wo.jsx)("div", {
                         className: "container",
                         children: (0, wo.jsx)(ms, {
                             header: t
                         })
                     })
                 },
                 Ms = function() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                         t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null,
-                        n = Ta(),
-                        r = Aa();
+                        n = Ua(),
+                        r = Pa();
 
                     function o(o, i) {
-                        return _a(e, t, o, i, (function() {}), (function() {}), (function() {}), (function() {}), (function() {}), n, r, !0)
+                        return Ba(e, t, o, i, (function() {}), (function() {}), (function() {}), (function() {}), (function() {}), n, r, !0)
                     }
                     return function(e, t) {
-                        return Oa(o(e, t))
+                        return Fa(o(e, t))
                     }
                 },
                 js = {
                     fontSize: "11pt",
                     verticalAlign: "top",
                     paddingBottom: "2pt",
                     paddingRight: "10pt",
@@ -49618,15 +49625,15 @@
                                     children: "Clear"
                                 })
                             })]
                         })
                     })
                 },
                 xs = function(e) {
-                    var n = Ua("//__functioncache__"),
+                    var n = Ya("//__functioncache__"),
                         r = Ms(),
                         o = l((0, t.useState)(!1), 2),
                         i = o[0],
                         a = o[1],
                         s = nt(nt({}, js), {}, {
                             verticalAlign: "bottom",
                             fontWeight: "bold",
@@ -49944,21 +49951,21 @@
                                 })
                             })]
                         }), M]
                     })
                 },
                 Is = function(e) {
                     var n = je().environ,
-                        r = Ua(rn.Url("/aws/s3/buckets", n), {
+                        r = Ya(rn.Url("/aws/s3/buckets", n), {
                             initial: []
                         }),
-                        o = Ua({
+                        o = Ya({
                             initial: []
                         }),
-                        i = Ua({
+                        i = Ya({
                             initial: []
                         }),
                         a = l((0, t.useState)(""), 2),
                         s = a[0],
                         u = a[1];
 
                     function c() {
@@ -50232,15 +50239,15 @@
                                                             }), (0, wo.jsxs)("td", {
                                                                 align: "right",
                                                                 children: [e.size, "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     whiteSpace: "nowrap"
                                                                 },
-                                                                children: [Wa.Format(e.modified), "\xa0\xa0"]
+                                                                children: [ha.Format(e.modified), "\xa0\xa0"]
                                                             })]
                                                         }, n), n < r.keys.length - 1 && (0, wo.jsxs)(wo.Fragment, {
                                                             children: [(0, wo.jsx)("tr", {
                                                                 children: (0, wo.jsx)("td", {
                                                                     style: {
                                                                         paddingTop: "4pt"
                                                                     }
@@ -50352,15 +50359,15 @@
                                             style: {
                                                 cursor: "copy",
                                                 float: "right",
                                                 fontFamily: "monospace"
                                             },
                                             src: on.Clipboard(),
                                             height: "19"
-                                        }), Ia.Format(t.content)]
+                                        }), Ca.Format(t.content)]
                                     })]
                                 })
                             })
                         },
                         L = function(e) {
                             var t = e.condition,
                                 n = e.color,
@@ -50430,27 +50437,27 @@
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                Ds = Da((function() {
+                Ds = Ea((function() {
                     return Bt.IsReadOnlyMode()
                 })),
                 Ls = function() {
-                    var e = l(La(Ds), 2),
+                    var e = l(Ta(Ds), 2),
                         t = e[0],
                         n = e[1];
                     return [t, function(e) {
                         n(e), Bt.SetReadOnlyMode(e)
                     }]
                 },
                 Ss = function() {
-                    var e, t = null === (e = Ua("/checks_validation").data) || void 0 === e ? void 0 : e.actions_with_no_associated_check;
+                    var e, t = null === (e = Ya("/checks_validation").data) || void 0 === e ? void 0 : e.actions_with_no_associated_check;
                     return t ? (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsxs)("div", {
                             className: "box error thickborder",
                             style: {
                                 width: "60%",
                                 fontSize: "small"
                             },
@@ -50518,15 +50525,15 @@
                         children: n
                     })
                 },
                 Es = {
                     Ago: uo.Ago,
                     Format: uo.FormatDuration,
                     FromNow: uo.FromNow,
-                    Live: Ya.FormatDuration
+                    Live: da.FormatDuration
                 };
 
             function Ts(e) {
                 e.update()
             }
 
             function As(e) {
@@ -50821,19 +50828,19 @@
                                         url: rn.Url("/checks/".concat(t, "/history/latest")),
                                         nocache: o
                                     })
                                 }(e, null === t || void 0 === t ? void 0 : t.action, n, r)
                             }
                         })
                     }
-                    r.__result = Ua({
+                    r.__result = Ya({
                         cache: !0
-                    }), r.__resultByUuid = Ua({
+                    }), r.__resultByUuid = Ya({
                         cache: !0
-                    }), r.__resultByAction = Ua({
+                    }), r.__resultByAction = Ya({
                         cache: !0
                     }), (0, t.useEffect)((function() {
                         c(r, o, i)
                     }), []), (0, t.useEffect)((function() {
                         r.__showingResults = !0, c(r, o, i)
                     }), []);
                     var d = l((0, t.useState)(!0), 2),
@@ -51220,15 +51227,15 @@
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
                                         children: i.__result.get("timestamp")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result ".concat(i.name),
                                         text: "Click to " + (i.__showingResultDetails ? "hide" : "show") + " latest result."
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
-                                        text: Es.Format(i.__result.get("timestamp"), Wa.Now(), !0, null, null, "ago")
+                                        text: Es.Format(i.__result.get("timestamp"), ha.Now(), !0, null, null, "ago")
                                     })]
                                 }), i.__showingResultDetails && (0, wo.jsx)(wo.Fragment, {
                                     children: i.__result.get("uuid") ? (0, wo.jsx)(wo.Fragment, {
                                         children: d ? (0, wo.jsx)(wo.Fragment, {
                                             children: i.__result.get("action") ? (0, wo.jsxs)(wo.Fragment, {
                                                 children: ["\xa0|\xa0", (0, wo.jsx)("span", {
                                                     id: "tooltip-view-latest-result-summary ".concat(i.name),
@@ -51512,15 +51519,15 @@
                         }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsx)(Lo, {
                                 condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                                 color: ln.GetForegroundColor(),
                                 label: "Loading latest result "
                             })
                         }) : (0, wo.jsx)(wo.Fragment, {
-                            children: Ia.Format(n.__resultByUuid.get())
+                            children: Ca.Format(n.__resultByUuid.get())
                         })]
                     }) : i ? (0, wo.jsxs)("pre", {
                         className: "box lighten",
                         style: {
                             wordWrap: "break-word",
                             paddingBottom: "4pt",
                             marginBottom: "3px",
@@ -51568,15 +51575,15 @@
                         }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsx)(Lo, {
                                 condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                                 color: ln.GetForegroundColor(),
                                 label: "Loading latest result "
                             })
                         }) : (0, wo.jsx)(wo.Fragment, {
-                            children: Ia.Format(n.__resultByAction.get())
+                            children: Ca.Format(n.__resultByAction.get())
                         })]
                     }) : (0, wo.jsxs)("pre", {
                         className: "box lighten",
                         style: {
                             color: "PASS" === (null === (t = n.__result.get("status")) || void 0 === t ? void 0 : t.toUpperCase()) ? "inherit" : "darkred",
                             wordWrap: "break-word",
                             paddingBottom: "4pt",
@@ -51642,15 +51649,15 @@
                             color: ln.GetForegroundColor(),
                             label: "Loading latest result "
                         }) : n.__result.empty ? (0, wo.jsx)("div", {
                             style: {
                                 marginTop: "1pt"
                             },
                             children: "No result."
-                        }) : Ia.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
+                        }) : Ca.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
                 tu = function(e) {
                     var t = e.check,
                         n = e.env,
                         r = e.groupList,
                         o = e.historyList,
@@ -51972,15 +51979,15 @@
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: Wa.Format(n.__queuedCheckRun + "+00:00")
+                                        children: ha.Format(n.__queuedCheckRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
@@ -52079,15 +52086,15 @@
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: Wa.Format(n.__queuedActionRun + "+00:00")
+                                        children: ha.Format(n.__queuedActionRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
@@ -52245,15 +52252,15 @@
                         })
                     }
 
                     function y() {
                         g(!0)
                     }
                     return i.__resultHistory = function() {
-                        return Ua({
+                        return Ya({
                             url: rn.Url("/checks/".concat(i.name, "/history")),
                             nofetch: !0,
                             cache: !0
                         })
                     }(), (0, t.useEffect)((function() {
                         g()
                     }), []), (0, wo.jsxs)("div", {
@@ -52400,15 +52407,15 @@
                                                                 id: "tooltip-history-timestamp-".concat(i.name, "-").concat(n),
                                                                 onClick: function() {
                                                                     u(i, e, l(e), a)
                                                                 },
                                                                 style: {
                                                                     cursor: "pointer"
                                                                 },
-                                                                children: Wa.Format(d(e))
+                                                                children: ha.Format(d(e))
                                                             }), (0, wo.jsx)(oa, {
                                                                 id: "tooltip-history-timestamp-".concat(i.name, "-").concat(n),
                                                                 text: uo.Ago(d(e)),
                                                                 position: "right",
                                                                 shape: "squared"
                                                             }), "\xa0\xa0"]
                                                         }), (0, wo.jsxs)("td", {
@@ -52500,15 +52507,15 @@
                                                                             marginRight: "2pt",
                                                                             fontSize: "large",
                                                                             fontWeight: "bold",
                                                                             cursor: "pointer"
                                                                         },
                                                                         children: "X"
                                                                     })]
-                                                                }), Ia.Format(e.__result)]
+                                                                }), Ca.Format(e.__result)]
                                                             })
                                                         })
                                                     })
                                                 })]
                                             }, n)
                                         }))
                                     })]
@@ -53020,25 +53027,25 @@
                                 })]
                             })
                         })
                     })
                 },
                 cu = function(e) {
                     var n = je().environ,
-                        r = Ua({
+                        r = Ya({
                             initial: []
                         }),
-                        o = Ua({
+                        o = Ya({
                             initial: []
                         }),
-                        i = Ua(rn.Url("/info")),
+                        i = Ya(rn.Url("/info")),
                         a = l((0, t.useState)(!1), 2),
                         s = a[0],
                         u = a[1];
-                    var c = Ua({
+                    var c = Ya({
                             url: rn.Url("/checks/grouped/schedule", n),
                             nofetch: !0,
                             cache: !0,
                             onData: function(e) {
                                 return e.sort((function(e, t) {
                                     return e.group > t.group ? 1 : e.group < t.group ? -1 : 0
                                 })), e.length > 0 && Us(function(e) {
@@ -53046,27 +53053,27 @@
                                         var r, o;
                                         (!t || (null === (r = e[n]) || void 0 === r || null === (o = r.checks) || void 0 === o ? void 0 : o.length) < t.checks.length) && (t = e[n])
                                     }
                                     return t
                                 }(e), 0, o), e
                             }
                         }),
-                        d = Ua({
+                        d = Ya({
                             url: rn.Url("/lambdas", n),
                             cache: !0,
                             onData: function(e) {
                                 return e.sort((function(e, t) {
                                     return e.lambda_name > t.lambda_name ? 1 : e.lambda_name < t.lambda_name ? -1 : 0
                                 })), e
                             }
                         });
                     (0, t.useEffect)((function() {
                         f(), c.fetch(s ? rn.Url("/checks/grouped/schedule") : rn.Url("/checks/grouped"))
                     }), [s]);
-                    var p = Ua();
+                    var p = Ya();
 
                     function f() {
                         p.refresh(rn.Url("/checks_status", n))
                     }
 
                     function h(e, t, n, r) {
                         Rs(e, n) ? Ps(e, n, r) : Us(e, 0, n)
@@ -53217,15 +53224,15 @@
                                                 }
                                             })]
                                         }, e.group)
                                     }))
                                 })]
                             })
                         },
-                        m = Ua(null),
+                        m = Ya(null),
                         v = l((0, t.useState)(!1), 2),
                         M = v[0],
                         j = v[1];
 
                     function b() {
                         return !m.empty
                     }
@@ -53326,15 +53333,15 @@
                                                 })]
                                             }), m.yaml()]
                                         })
                                     })
                                 })]
                             })
                         },
-                        C = Ua(rn.Url("/checks/history/recent?limit=20", n), {
+                        C = Ya(rn.Url("/checks/history/recent?limit=20", n), {
                             nofetch: !0,
                             cache: !0
                         }),
                         E = l((0, t.useState)(!1), 2),
                         T = E[0],
                         A = E[1];
 
@@ -53537,15 +53544,15 @@
                                                                 style: {
                                                                     width: "20%"
                                                                 },
                                                                 children: [ks.Format(e.timestamp), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                                     children: uo.Format(e.timestamp)
                                                                 }), (0, wo.jsx)(oa, {
                                                                     id: "recent-runs-timestamp ".concat(i),
-                                                                    text: Es.Format(e.timestamp, Wa.Now(), !0, null, null, "agoy")
+                                                                    text: Es.Format(e.timestamp, ha.Now(), !0, null, null, "agoy")
                                                                 }), "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     width: "45%"
                                                                 },
                                                                 children: [(0, wo.jsx)("b", {
                                                                     style: {
@@ -53914,15 +53921,15 @@
                                                 children: [(0, wo.jsx)("td", {
                                                     style: c,
                                                     children: "Updated:"
                                                 }), (0, wo.jsx)("td", {
                                                     style: l,
                                                     children: (0, wo.jsx)("span", {
                                                         id: "tooltip-lambda-updated-".concat(u.lambda_name),
-                                                        children: Wa.Format(u.lambda_modified)
+                                                        children: ha.Format(u.lambda_modified)
                                                     })
                                                 }), (0, wo.jsx)(oa, {
                                                     id: "tooltip-lambda-updated-".concat(u.lambda_name),
                                                     text: uo.Ago(u.lambda_modified),
                                                     position: "right",
                                                     shape: "squared"
                                                 })]
@@ -54334,15 +54341,15 @@
                                     })
                                 })
                             })
                         })
                     })
                 },
                 gu = function(e) {
-                    var n, r = (n = e.check, Ua({
+                    var n, r = (n = e.check, Ya({
                             url: rn.Url("/checks/".concat(n.name)),
                             nofetch: !0,
                             cache: !0
                         })),
                         o = l((0, t.useState)(!1), 2),
                         i = o[0],
                         a = o[1];
@@ -54402,15 +54409,15 @@
                                     })]
                                 })
                             })
                         })
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
                 yu = function(e) {
-                    var n = Ua(),
+                    var n = Ya(),
                         r = l((0, t.useState)([]), 2),
                         o = r[0],
                         i = r[1];
 
                     function a(e) {
                         return void 0 !== o.find((function(t) {
                             return t.group === e.group
@@ -55415,16 +55422,16 @@
                         v = y[1],
                         M = l((0, t.useState)(Math.floor(h / d)), 2),
                         j = M[0],
                         b = M[1],
                         w = l((0, t.useState)(Math.max(1, j + 1)), 2),
                         x = w[0],
                         N = w[1],
-                        I = Ua(),
-                        D = Ua();
+                        I = Ya(),
+                        D = Ya();
 
                     function L(e, t, n) {
                         p(e), g(t), v(n)
                     }
 
                     function S(e, t, n) {
                         wt.HasValue(n) || (n = "timestamp.desc"), u(nt(nt({}, s), {}, {
@@ -55639,15 +55646,15 @@
                                                             id: "tooltip-timestamp-".concat(n),
                                                             onClick: function() {
                                                                 return E(i, e, a(e))
                                                             },
                                                             style: {
                                                                 cursor: "pointer"
                                                             },
-                                                            children: Wa.Format(u(e))
+                                                            children: ha.Format(u(e))
                                                         }), (0, wo.jsx)(oa, {
                                                             id: "tooltip-timestamp-".concat(n),
                                                             text: uo.Ago(u(e)),
                                                             position: "right",
                                                             shape: "squared"
                                                         }), "\xa0\xa0"]
                                                     }), (0, wo.jsxs)("td", {
@@ -55741,15 +55748,15 @@
                                                                             marginRight: "2pt",
                                                                             fontSize: "large",
                                                                             fontWeight: "bold",
                                                                             cursor: "pointer"
                                                                         },
                                                                         children: "X"
                                                                     })]
-                                                                }), Ia.Format(e.__result)]
+                                                                }), Ca.Format(e.__result)]
                                                             })
                                                         })
                                                     })
                                                 })]
                                             }, a(e))
                                         }))
                                     })]
@@ -55934,31 +55941,31 @@
                                     })]
                                 })]
                             })
                         })
                     })
                 },
                 Iu = function() {
-                    var e = l((0, t.useContext)(Ra), 2),
+                    var e = l((0, t.useContext)(Ga), 2),
                         n = (e[0], e[1]),
-                        r = Pa();
+                        r = Qa();
                     return function(e) {
                         return r.refresh(rn.Url("/header", e), {
                             onData: function(e) {
                                 return n(e)
                             },
                             cache: !0
                         })
                     }
                 },
                 Du = function(e) {
-                    var t, n, r = Fa(),
+                    var t, n, r = Wa(),
                         o = Iu(),
-                        i = Ua(co.IsLoggedIn() ? rn.Url("/info") : null);
-                    wa.NoteLastUrl(r);
+                        i = Ya(co.IsLoggedIn() ? rn.Url("/info") : null);
+                    La.NoteLastUrl(r);
                     var a = Me();
 
                     function s() {
                         return tn.IsKnown(tn.Current(), r)
                     }
 
                     function u(e) {
@@ -56292,15 +56299,15 @@
                                     marginTop: "8pt"
                                 }
                             })]
                         })
                     })
                 },
                 Lu = function(e) {
-                    var t = Fa();
+                    var t = Wa();
                     return t.loading ? null : (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("br", {}), (0, wo.jsx)("table", {
                             width: "100%",
                             children: (0, wo.jsxs)("tbody", {
                                 children: [(0, wo.jsx)("tr", {
                                     style: {
                                         backgroundColor: "darkred",
@@ -56333,30 +56340,30 @@
                                     children: (0, wo.jsx)("td", {})
                                 })]
                             })
                         })]
                     })
                 },
                 Su = function(e) {
-                    var t = Fa();
+                    var t = Wa();
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "container",
                             id: "login_container",
                             children: (0, wo.jsxs)("div", {
                                 className: "boxstyle check-error",
                                 style: {
                                     margin: "20pt",
                                     padding: "10pt"
                                 },
                                 children: [(0, wo.jsx)("b", {
                                     children: "Forbidden response from server."
                                 }), ".  ", (0, wo.jsx)("br", {}), "You seem to be logged in but the server does not seem to think so. ", (0, wo.jsx)("br", {}), "Try ", (0, wo.jsx)("span", {
                                     onClick: function() {
-                                        return xa()
+                                        return Sa()
                                     },
                                     style: {
                                         cursor: "pointer"
                                     },
                                     children: (0, wo.jsx)("u", {
                                         children: "logging out"
                                     })
@@ -56414,15 +56421,15 @@
                         }), (0, wo.jsx)(Tu, {
                             header: t
                         })]
                     })
                 },
                 Eu = function() {
                     l($e(), 1)[0];
-                    var e = Ua("/certificates");
+                    var e = Ya("/certificates");
                     if (e.loading) return (0, wo.jsx)(wo.Fragment, {});
                     var t = e.find((function(e) {
                         return "Portal" === e.name
                     }));
                     return t && t.expires_soon ? (0, wo.jsxs)(Au, {
                         children: [(0, wo.jsx)("b", {
                             children: "Warning: SSL certificate for associated Portal will expire soon"
@@ -56433,15 +56440,15 @@
                             },
                             children: "View"
                         })]
                     }) : void 0
                 },
                 Tu = function(e) {
                     e.header;
-                    var t = Ua("/portal_access_key");
+                    var t = Ya("/portal_access_key");
                     if (t.loading) return (0, wo.jsx)(wo.Fragment, {});
                     if (t) {
                         var n, r;
                         if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, wo.jsxs)(Au, {
                             children: [(0, wo.jsx)("b", {
                                 children: "Warning: Access key for associated Portal will expire soon"
                             }), "\xa0", po.RightArrow, "\xa0 ", t.data.expires_at, " \xa0", po.RightArrow, "\xa0", uo.FromNow(t.data.expires_at, !0, !1), "\xa0", po.RightArrow, "\xa0", (0, wo.jsx)(qe, {
@@ -56680,15 +56687,15 @@
                             children: "\xa0|\xa0"
                         }), (0, wo.jsx)(Ou, {
                             header: t
                         })]
                     })
                 },
                 Uu = function(e) {
-                    var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k = Fa(),
+                    var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k = Wa(),
                         C = Iu(),
                         E = Me(),
                         T = l(Ha(), 1)[0],
                         A = tn.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
                         z = ln.LightenDarkenColor(ln.GetBackgroundColor(), -10);
                     return (0, wo.jsx)(wo.Fragment, {
                         children: k.loading ? (0, wo.jsxs)("div", {
@@ -56970,15 +56977,15 @@
                                                 style: {
                                                     paddingRight: "10pt",
                                                     whiteSpace: "nowrap",
                                                     color: "#D6EAF8"
                                                 },
                                                 align: "right",
                                                 children: [(0, wo.jsx)("small", {
-                                                    children: (0, wo.jsx)(Wa.Live, {
+                                                    children: (0, wo.jsx)(ha.Live, {
                                                         verbose: !0,
                                                         timezone: !1
                                                     })
                                                 }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, wo.jsxs)(wo.Fragment, {
                                                     children: ["\xa0|\xa0", (0, wo.jsx)(qe, {
                                                         id: "tooltip-header-account",
                                                         to: $r.Path("/login"),
@@ -56997,15 +57004,15 @@
                                                 }), co.IsLoggedIn(k) ? (0, wo.jsxs)("span", {
                                                     children: ["\xa0|\xa0", (0, wo.jsx)("span", {
                                                         style: {
                                                             cursor: "pointer",
                                                             color: "#D6EAF8"
                                                         },
                                                         onClick: function() {
-                                                            return xa()
+                                                            return Sa()
                                                         },
                                                         children: "LOGOUT"
                                                     })]
                                                 }) : (0, wo.jsxs)("span", {
                                                     children: ["\xa0|\xa0", (0, wo.jsx)(qe, {
                                                         to: $r.Path("/login?auth", tn.Current(k)),
                                                         style: {
@@ -57409,33 +57416,33 @@
                 Pu = function(e) {
                     var n = e.children,
                         r = l((0, t.useState)({
                             loading: !0
                         }), 2),
                         o = r[0],
                         i = r[1];
-                    return Ua("/header", {
+                    return Ya("/header", {
                         onData: function(e) {
                             e.loading = !1, i(e), tn.IsFoursightFourfront(e) ? ln.SetFoursightFourfront() : ln.SetFoursightCgap()
                         },
                         onError: function(e) {
                             i((function(e) {
                                 return nt(nt({}, e), {
                                     error: !0
                                 })
                             }))
                         },
                         cache: !0
-                    }), (0, wo.jsx)(Ra.Provider, {
+                    }), (0, wo.jsx)(Ga.Provider, {
                         value: [o, i],
                         children: n
                     })
                 },
                 Ru = function(e) {
-                    var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w = Fa(),
+                    var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w = Wa(),
                         x = (tn.IsFoursightFourfront(w) ? "foursight" : "foursight-cgap") + ": " + (null === w || void 0 === w || null === (n = w.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === w || void 0 === w || null === (r = w.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === w || void 0 === w || null === (o = w.versions) || void 0 === o ? void 0 : o.dcicutils),
                         N = {
                             id: "".concat(null === (i = w.app) || void 0 === i || null === (a = i.credentials) || void 0 === a ? void 0 : a.aws_account_name, ":").concat(null === w || void 0 === w || null === (s = w.app) || void 0 === s ? void 0 : s.stage),
                             name: null === (u = w.app) || void 0 === u || null === (c = u.credentials) || void 0 === c ? void 0 : c.aws_account_name,
                             stage: null === (d = w.app) || void 0 === d ? void 0 : d.stage
                         },
                         I = l((0, t.useState)(!1), 2),
@@ -57654,20 +57661,20 @@
                                         children: "View session"
                                     })]
                                 }), (0, wo.jsx)(aa, {
                                     top: "6pt",
                                     bottom: "7pt"
                                 }), (0, wo.jsxs)("small", {
                                     children: ["To ", (0, wo.jsx)("b", {
-                                        onClick: xa,
+                                        onClick: Sa,
                                         children: (0, wo.jsx)(ia, {
                                             children: "logout"
                                         })
                                     }), " click ", (0, wo.jsx)("b", {
-                                        onClick: xa,
+                                        onClick: Sa,
                                         children: (0, wo.jsx)(ia, {
                                             children: (0, wo.jsx)("u", {
                                                 children: "here"
                                             })
                                         })
                                     }), "."]
                                 })]
@@ -58002,26 +58009,26 @@
                                     }), O, _]
                                 }))]
                             }) : (0, wo.jsx)("span", {})
                         })
                     })
                 },
                 Yu = function() {
-                    var e, n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k, C, E, T, A, z, O, _, U, P, R, F, B, Y, Q, G, W, H, V, Z, q, J, K, X, $, ee = Fa(),
-                        te = Ua("/info"),
+                    var e, n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k, C, E, T, A, z, O, _, U, P, R, F, B, Y, Q, G, W, H, V, Z, q, J, K, X, $, ee = Wa(),
+                        te = Ya("/info"),
                         ne = l((0, t.useState)(!1), 2),
                         re = ne[0],
                         oe = ne[1],
                         ie = l((0, t.useState)(!1), 2),
                         ae = ie[0],
                         se = ie[1],
                         ue = l((0, t.useState)(!1), 2),
                         le = ue[0],
                         ce = ue[1],
-                        de = Ua("/portal_access_key"),
+                        de = Ya("/portal_access_key"),
                         pe = Ms();
                     return te.error ? (0, wo.jsx)(ua, {
                         error: te.error,
                         message: "Error loading info from Foursight API"
                     }) : (0, wo.jsxs)("div", {
                         className: "container",
                         children: [(0, wo.jsxs)(Fu, {
@@ -58324,15 +58331,15 @@
                                             return fo.Copy("authtoken")
                                         },
                                         style: {
                                             float: "right",
                                             height: "20px",
                                             cursor: "copy"
                                         }
-                                    }), Ia.Format(co.Token())]
+                                    }), Ca.Format(co.Token())]
                                 })]
                             }) : (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("small", {
                                     onClick: function() {
                                         return oe(!0)
                                     },
                                     style: {
@@ -58417,15 +58424,15 @@
                                     border: "0",
                                     margin: "0",
                                     padding: "8",
                                     paddingBottom: "8",
                                     marginTop: "0"
                                 },
                                 children: (0, wo.jsxs)("span", {
-                                    children: [Ia.Format(te.get("buckets.info")), (null === (F = te.get("buckets.info")) || void 0 === F ? void 0 : F.length) > 1 ? (0, wo.jsx)("div", {
+                                    children: [Ca.Format(te.get("buckets.info")), (null === (F = te.get("buckets.info")) || void 0 === F ? void 0 : F.length) > 1 ? (0, wo.jsx)("div", {
                                         style: {
                                             height: "1px",
                                             marginTop: "6px",
                                             marginBottom: "6px",
                                             background: "black"
                                         }
                                     }) : (0, wo.jsx)("span", {})]
@@ -58440,15 +58447,15 @@
                                 style: {
                                     border: "0",
                                     margin: "0",
                                     paddingTop: "8",
                                     paddingBottom: "8",
                                     marginTop: "0"
                                 },
-                                children: Ia.Format(te.get("buckets.ecosystem"))
+                                children: Ca.Format(te.get("buckets.ecosystem"))
                             })
                         }), te.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && te.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsxs)(Fu, {
                                 info: te,
                                 title: "Logs",
                                 children: [(0, wo.jsx)(Bu, {
                                     name: "Log Group",
@@ -58489,15 +58496,15 @@
                             }), (0, wo.jsx)(Bu, {
                                 name: "Size",
                                 value: te.get("app.lambda.lambda_code_size"),
                                 monospace: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "Modified",
-                                value: Wa.Format(te.get("app.lambda.lambda_modified")),
+                                value: ha.Format(te.get("app.lambda.lambda_modified")),
                                 monospace: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "Role",
                                 value: te.get("app.lambda.lambda_role"),
                                 monospace: !0,
                                 size: "2"
@@ -58562,15 +58569,15 @@
                             }), (0, wo.jsx)(oa, {
                                 id: "tooltip-info-clear",
                                 position: "bottom",
                                 size: "small",
                                 text: "Click to clear any server-side caches."
                             }), (0, wo.jsx)(Bu, {
                                 name: "App Deployed At",
-                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : Wa.Format(null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
+                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : ha.Format(null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
                                 monospace: !0,
                                 copy: !0,
                                 optional: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "App Launched At",
                                 value: (null === (Q = ee.app) || void 0 === Q ? void 0 : Q.launched) + Es.Format(null === (G = ee.app) || void 0 === G ? void 0 : G.launched, new Date, !0, "just now", "|", "ago"),
@@ -65231,16 +65238,16 @@
                 }(),
                 Jp = new qp(null);
             ec.register(Jp);
             var Kp = "#FEFEFE",
                 Xp = function(e) {
                     var t = e.hide,
                         n = je().environ,
-                        r = Fa(),
-                        o = Ua(rn.Url("/cognito_config", !1), {
+                        r = Wa(),
+                        o = Ya(rn.Url("/cognito_config", !1), {
                             cache: !0,
                             onData: function(e) {
                                 var t = {
                                     region: e.region,
                                     userPoolId: e.userpool,
                                     userPoolWebClientId: e.client,
                                     mandatorySignIn: !0,
@@ -65441,15 +65448,15 @@
                     var t = l($e(), 1)[0],
                         n = t.get("code"),
                         r = t.get("state"),
                         o = sessionStorage.getItem("oauth_state"),
                         i = sessionStorage.getItem("ouath_pkce_key"),
                         a = Me(),
                         s = "".concat(rn.Url("/cognito/callback", !1), "?code=").concat(n, "&code_verifier=").concat(i, "&state=").concat(r, "&state_verifier=").concat(o),
-                        u = Ua(s, {
+                        u = Ya(s, {
                             onDone: function(e) {
                                 var t, n, r = null === (t = e.data) || void 0 === t ? void 0 : t.authtoken,
                                     o = null === (n = e.data) || void 0 === n ? void 0 : n.expires;
                                 Bt.Set("authtoken", r, o);
                                 var i = Bt.Redirect();
                                 if (wt.HasValue(i)) i = Gt.FromUrl(i);
                                 else if (i = Bt.LastUrl(), wt.HasValue(i)) i = Gt.FromUrl(i);
@@ -65478,23 +65485,23 @@
                                 })
                             })
                         })
                     }
                 },
                 of = n(9712),
                 af = function(e) {
-                    var n, r, o, i, a, s, u, c, d, p, f, h = Fa(),
+                    var n, r, o, i, a, s, u, c, d, p, f, h = Wa(),
                         g = l((0, t.useState)(!1), 2),
                         y = g[0],
                         m = g[1],
                         v = l((0, t.useState)(!1), 2),
                         M = v[0],
                         j = v[1],
                         b = (null === (n = l($e(), 1)[0].get("auth")) || void 0 === n ? void 0 : n.length) >= 0,
-                        w = Ua(rn.Url("/auth0_config", !1)),
+                        w = Ya(rn.Url("/auth0_config", !1)),
                         x = l((0, t.useState)(!1), 2),
                         N = x[0],
                         I = x[1],
                         D = l((0, t.useState)($r.IsCognitoEnabled()), 2),
                         L = D[0],
                         S = D[1];
 
@@ -65507,15 +65514,15 @@
                     }
 
                     function E() {
                         S(!1), $r.DisableCognito()
                     }
 
                     function T() {
-                        document.getElementById("login_container").style.display = "none", document.getElementById("login_auth_container").style.display = "block", document.getElementById("login_auth_cancel").style.display = "block", Bt.SetRedirect(wa.LastUrl()),
+                        document.getElementById("login_container").style.display = "none", document.getElementById("login_auth_container").style.display = "block", document.getElementById("login_auth_cancel").style.display = "block", Bt.SetRedirect(La.LastUrl()),
                             function() {
                                 var e, t, n, r, o, i, a, s = {
                                     container: "login_auth_container",
                                     auth: {
                                         redirectUrl: null === w || void 0 === w || null === (e = w.data) || void 0 === e ? void 0 : e.callback,
                                         responseType: "code",
                                         sso: null === w || void 0 === w || null === (t = w.data) || void 0 === t ? void 0 : t.sso,
@@ -65677,23 +65684,23 @@
                                                         }), "\xa0", (0, wo.jsx)("br", {}), "Click ", (0, wo.jsx)("span", {
                                                             style: {
                                                                 textDecoration: "underline",
                                                                 fontWeight: "bold",
                                                                 cursor: "pointer"
                                                             },
                                                             onClick: function() {
-                                                                return xa()
+                                                                return Sa()
                                                             },
                                                             children: "here"
                                                         }), " to ", (0, wo.jsx)("span", {
                                                             style: {
                                                                 cursor: "pointer"
                                                             },
                                                             onClick: function() {
-                                                                return xa()
+                                                                return Sa()
                                                             },
                                                             children: "logout"
                                                         }), "."]
                                                     })]
                                                 }), (0, wo.jsx)("td", {
                                                     style: {
                                                         paddingLeft: "12pt",
@@ -65813,15 +65820,15 @@
                                                     return fo.Copy("authtoken")
                                                 },
                                                 style: {
                                                     float: "right",
                                                     height: "20px",
                                                     cursor: "copy"
                                                 }
-                                            }), Ia.Format(co.Token())]
+                                            }), Ca.Format(co.Token())]
                                         }), (0, wo.jsxs)("pre", {
                                             className: "box",
                                             style: {
                                                 filter: "brightness(1.1)",
                                                 background: "inherit",
                                                 fontWeight: "bold",
                                                 marginTop: "-3pt",
@@ -65871,15 +65878,15 @@
                                             className: "box",
                                             style: {
                                                 filter: "brightness(1.1)",
                                                 background: "inherit",
                                                 fontWeight: "bold",
                                                 marginTop: "6pt"
                                             },
-                                            children: Ia.Format(null === h || void 0 === h ? void 0 : h.auth)
+                                            children: Ca.Format(null === h || void 0 === h ? void 0 : h.auth)
                                         })]
                                     })]
                                 })]
                             })
                         }) : (0, wo.jsxs)(t.Fragment, {
                             children: [(0, wo.jsxs)("div", {
                                 className: "container",
@@ -66083,15 +66090,15 @@
                                                     return fo.Copy("authtoken")
                                                 },
                                                 style: {
                                                     float: "right",
                                                     height: "20px",
                                                     cursor: "copy"
                                                 }
-                                            }), Ia.Format(Bt.AuthToken())]
+                                            }), Ca.Format(Bt.AuthToken())]
                                         }), (0, wo.jsxs)("pre", {
                                             className: "box",
                                             style: {
                                                 filter: "brightness(1.1)",
                                                 background: "inherit",
                                                 color: "darkred",
                                                 fontWeight: "bold",
@@ -66164,15 +66171,15 @@
                                                     return fo.Copy("authtoken")
                                                 },
                                                 style: {
                                                     float: "right",
                                                     height: "20px",
                                                     cursor: "copy"
                                                 }
-                                            }), Ia.Format(null === h || void 0 === h ? void 0 : h.auth)]
+                                            }), Ca.Format(null === h || void 0 === h ? void 0 : h.auth)]
                                         })]
                                     })]
                                 })]
                             }), w.loading ? (0, wo.jsx)(wo.Fragment, {
                                 children: "Loading Auth0 configuration ..."
                             }) : (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("br", {}), (0, wo.jsx)("br", {}), (0, wo.jsx)("br", {}), (0, wo.jsxs)("div", {
@@ -66211,23 +66218,23 @@
                                     }), 10), "")]
                                 })]
                             })]
                         })
                     })
                 },
                 sf = function(e) {
-                    var n = Fa(),
+                    var n = Wa(),
                         r = je().environCompare,
                         o = l((0, t.useState)(!1), 2),
                         i = o[0],
                         a = o[1],
                         s = l((0, t.useState)("all"), 2),
                         u = s[0],
                         c = s[1],
-                        d = Ua(rn.Url("/gac/".concat(r), tn.Current())),
+                        d = Ya(rn.Url("/gac/".concat(r), tn.Current())),
                         p = Me();
 
                     function f(e, t) {
                         var n, r;
                         return null === t || void 0 === t || null === (n = t.gac_diffs) || void 0 === n || null === (r = n.same) || void 0 === r ? void 0 : r.includes(e)
                     }
 
@@ -66574,14 +66581,15 @@
                             background: e.toggled ? "var(--box-fg)" : "inherit",
                             color: e.toggled ? "var(--box-bg)" : "inherit",
                             fontSize: "10pt",
                             fontWeight: "bold",
                             border: "1pt black solid",
                             borderRadius: "3px",
                             padding: "0px 1px 2px 1px",
+                            marginLeft: "2pt",
                             marginTop: "-1px",
                             marginRight: "-4px",
                             float: "right",
                             cursor: "pointer",
                             userSelect: "none"
                         },
                         n = Jr()();
@@ -66631,15 +66639,15 @@
                             position: "bottom",
                             size: "small",
                             text: "Click to ".concat(e.toggled ? "hide" : "show", " raw ").concat(e.yaml ? "YAML" : "JSON", " data.")
                         })]
                     })
                 },
                 lf = function(e) {
-                    var n, r = l((0, t.useState)(!1), 2),
+                    var n, r = l((0, t.useState)(e.showJson), 2),
                         o = r[0],
                         i = r[1],
                         a = function() {
                             return i(!o)
                         },
                         s = (0, t.useRef)(null);
                     return e.disabled ? (0, wo.jsx)(wo.Fragment, {
@@ -66685,15 +66693,15 @@
                                     fontFamily: "monospace",
                                     whiteSpace: "pre",
                                     background: "inherit",
                                     width: "100%",
                                     maxWidth: null === s || void 0 === s || null === (n = s.current) || void 0 === n ? void 0 : n.offsetWidth
                                 },
                                 children: e.yaml ? (0, wo.jsx)(wo.Fragment, {
-                                    children: Ia.Format(e.data)
+                                    children: Ca.Format(e.data)
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: no.Format(e.data)
                                 })
                             })]
                         }) : (0, wo.jsx)(wo.Fragment, {})]
                     })
                 },
@@ -66772,34 +66780,46 @@
                                 children: "Security Groups"
                             })]
                         })]
                     })
                 },
                 hf = function(e) {
                     var t = e.showEcsClusters,
-                        n = e.toggleEcsClusters;
+                        n = e.toggleEcsClusters,
+                        r = e.showEcsTasks,
+                        o = e.toggleEcsTasks;
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
                                 children: "AWS Elastic Container Service"
                             })
-                        }), (0, wo.jsx)("div", {
+                        }), (0, wo.jsxs)("div", {
                             className: "box margin",
                             style: {
                                 width: "100%",
                                 marginBottom: "6pt"
                             },
-                            children: (0, wo.jsx)("div", {
+                            children: [(0, wo.jsx)("div", {
                                 className: "pointer",
                                 style: {
                                     fontWeight: t() ? "bold" : "normal"
                                 },
                                 onClick: n,
                                 children: "Clusters"
-                            })
+                            }), (0, wo.jsx)(aa, {
+                                top: "2pt",
+                                bottom: "2pt"
+                            }), (0, wo.jsx)("div", {
+                                className: "pointer",
+                                style: {
+                                    fontWeight: r() ? "bold" : "normal"
+                                },
+                                onClick: o,
+                                children: "Task Definitions"
+                            })]
                         })]
                     })
                 },
                 gf = function(e) {
                     var t = e.showGac,
                         n = e.toggleGac,
                         r = e.showEcosystem,
@@ -66836,15 +66856,15 @@
                         })]
                     })
                 },
                 yf = function(e) {
                     var t, n, r = e.keyedState,
                         o = e.hide,
                         i = "true" === (null === (t = $e()[0]) || void 0 === t || null === (n = t.get("all")) || void 0 === n ? void 0 : n.toLowerCase()),
-                        a = Ua("/aws/vpcs".concat(i ? "/all" : ""), {
+                        a = Ya("/aws/vpcs".concat(i ? "/all" : ""), {
                             cache: !0
                         });
                     return (0, wo.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
                             marginBottom: "8pt"
@@ -67142,15 +67162,15 @@
                     var t, n, r = e.vpcId,
                         o = e.type,
                         i = e.hide,
                         a = e.notitle,
                         s = e.keyedState,
                         u = "true" === (null === (t = $e()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                         l = r ? "?vpc=".concat(r) : "",
-                        c = Ua("/aws/subnets".concat(u ? "/all" : "").concat(l), {
+                        c = Ya("/aws/subnets".concat(u ? "/all" : "").concat(l), {
                             cache: !0
                         });
                     return (0, wo.jsxs)("div", {
                         style: {
                             marginBottom: "8pt"
                         },
                         children: [!a && (0, wo.jsxs)("div", {
@@ -67352,15 +67372,15 @@
                 jf = function(e) {
                     var t, n = e.vpcId,
                         r = e.notitle,
                         o = e.keyedState,
                         i = e.hide,
                         a = "true" === (null === (t = $e()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                         s = n ? "?vpc=".concat(n) : "",
-                        u = Ua("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
+                        u = Ya("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
                             cache: !0
                         });
                     return (0, wo.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
                             marginBottom: "8pt"
@@ -67611,15 +67631,15 @@
                         })
                     })
                 },
                 wf = function(e) {
                     var t = e.securityGroupId,
                         n = e.direction,
                         r = "inbound" === n ? "?direction=inbound" : "outbound" === n ? "?direction=outbound" : "",
-                        o = Ua("/aws/security_group_rules/".concat(t).concat(r), {
+                        o = Ya("/aws/security_group_rules/".concat(t).concat(r), {
                             cache: !0
                         });
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [o.loading && (0, wo.jsx)("div", {
                             className: "box lighten",
                             style: {
                                 paddingBottom: "10pt"
@@ -67805,15 +67825,15 @@
                                     children: "No tags."
                                 })
                             })
                         })
                     })
                 },
                 If = function(e) {
-                    var t = Ua("/aws/stacks", {
+                    var t = Ya("/aws/stacks", {
                         cache: !0
                     });
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
                                 children: "AWS Stacks"
                             })
@@ -67850,15 +67870,15 @@
                 Df = function(e) {
                     var t, n, r, o, i, a, s, u, c, d, p, f, h = e.stackName,
                         g = e.keyedState,
                         y = e.hide,
                         m = l(Xa(g), 2),
                         v = m[0],
                         M = m[1],
-                        j = Ua("/aws/stacks/".concat(h), {
+                        j = Ya("/aws/stacks/".concat(h), {
                             cache: !0
                         }),
                         b = function(e) {
                             return v[e]
                         },
                         w = function(e) {
                             return M(et({}, e, !v[e]))
@@ -67972,23 +67992,23 @@
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
                                             style: cf,
                                             children: "Created:"
                                         }), (0, wo.jsx)("td", {
                                             style: df,
-                                            children: null === (s = j.data) || void 0 === s ? void 0 : s.created
+                                            children: ha.Format(null === (s = j.data) || void 0 === s ? void 0 : s.created)
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
                                             style: cf,
                                             children: "Updated:"
                                         }), (0, wo.jsx)("td", {
                                             style: df,
-                                            children: null === (u = j.data) || void 0 === u ? void 0 : u.updated
+                                            children: ha.Format(null === (u = j.data) || void 0 === u ? void 0 : u.updated)
                                         })]
                                     }), (0, wo.jsx)(aa, {
                                         top: "2pt",
                                         bottom: "2pt",
                                         table: 2
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
@@ -68165,15 +68185,15 @@
                                     })]
                                 })
                             })
                         })]
                     })
                 },
                 Lf = function(e) {
-                    var t, n = Ua("/aws/stacks/".concat(e.stackName, "/outputs"), {
+                    var t, n = Ya("/aws/stacks/".concat(e.stackName, "/outputs"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
                             wordBreak: "break-all"
@@ -68218,15 +68238,15 @@
                                     })))
                                 })
                             })
                         })
                     })
                 },
                 Sf = function(e) {
-                    var t, n = Ua("/aws/stacks/".concat(e.stackName, "/parameters"), {
+                    var t, n = Ya("/aws/stacks/".concat(e.stackName, "/parameters"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
                             wordBreak: "break-all"
@@ -68271,15 +68291,15 @@
                                     })))
                                 })
                             })
                         })
                     })
                 },
                 kf = function(e) {
-                    var t, n = Ua("/aws/stacks/".concat(e.stackName, "/resources"), {
+                    var t, n = Ya("/aws/stacks/".concat(e.stackName, "/resources"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
                             wordBreak: "break-all"
@@ -68327,15 +68347,15 @@
                                     })))
                                 })
                             })
                         })
                     })
                 },
                 Cf = function(e) {
-                    var t = Ua("/aws/stacks/".concat(e.stackName, "/template"), {
+                    var t = Ya("/aws/stacks/".concat(e.stackName, "/template"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%"
                         },
@@ -68358,23 +68378,23 @@
                                         maxWidth: "100%",
                                         border: "0",
                                         background: "var(--box-bg-lighten)",
                                         marginLeft: "-6pt",
                                         marginTop: "-6pt",
                                         marginBottom: "-6pt"
                                     },
-                                    children: Dt.IsObject(t.data) ? Ia.Format(t.data) : t.data
+                                    children: Dt.IsObject(t.data) ? Ca.Format(t.data) : t.data
                                 })
                             })
                         })
                     })
                 },
                 Ef = function(e) {
                     var t, n, r, o, i = e.hide,
-                        a = Ua("/info", {
+                        a = Ya("/info", {
                             cache: !0
                         });
                     return (0, wo.jsxs)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
                             marginBottom: "8pt"
@@ -68395,93 +68415,246 @@
                                 onClick: i,
                                 children: po.X
                             })]
                         }), (0, wo.jsxs)("pre", {
                             className: "box margin",
                             children: [a.loading && (0, wo.jsx)(Lo, {
                                 label: "Loading Ecosystem"
-                            }), !a.loading && Ia.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
+                            }), !a.loading && Ca.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
                         })]
                     })
                 },
                 Tf = function(e) {
-                    var t, n, r, o, i = Ua("//aws/ecs/clusters/".concat(encodeURIComponent(e.cluster)), {
-                        cache: !0
-                    });
-                    return (0, wo.jsx)("div", {
-                        className: "box",
+                    var t = e.keyedState,
+                        n = e.hide,
+                        r = Ya("//aws/ecs/clusters");
+                    return (0, wo.jsxs)("div", {
                         style: {
-                            background: "inherit",
-                            marginTop: "2pt",
-                            marginBottom: "3pt",
-                            overflow: "auto"
+                            marginBottom: "8pt"
                         },
-                        children: (0, wo.jsx)(lf, {
-                            data: i.data,
-                            yaml: !0,
-                            both: !0,
-                            children: (0, wo.jsxs)("small", {
-                                children: [e.clusterDisplayName != (null === (t = i.data) || void 0 === t ? void 0 : t.name) && (0, wo.jsxs)(wo.Fragment, {
-                                    children: [(0, wo.jsx)("b", {
-                                        children: "Name"
-                                    }), ": ", null === (n = i.data) || void 0 === n ? void 0 : n.name, (0, wo.jsx)("br", {})]
-                                }), (0, wo.jsx)("b", {
-                                    children: "ARN"
-                                }), ": ", null === (r = i.data) || void 0 === r ? void 0 : r.arn, " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("b", {
-                                    children: "Deployed"
-                                }), ": ", null === (o = i.data) || void 0 === o ? void 0 : o.most_recent_deployed]
-                            })
-                        })
+                        children: [(0, wo.jsxs)("div", {
+                            children: [(0, wo.jsx)("b", {
+                                children: "AWS ESC Clusters"
+                            }), "\xa0\xa0", !r.loading && (0, wo.jsxs)("small", {
+                                children: ["(", null === r || void 0 === r ? void 0 : r.length, ")"]
+                            }), (0, wo.jsx)("b", {
+                                style: {
+                                    float: "right",
+                                    fontSize: "small",
+                                    marginTop: "2pt",
+                                    marginRight: "4pt",
+                                    cursor: "pointer"
+                                },
+                                onClick: n,
+                                children: po.X
+                            })]
+                        }), (0, wo.jsxs)("div", {
+                            style: {
+                                width: "100%"
+                            },
+                            className: "box lighten nomargin",
+                            children: [r.loading && (0, wo.jsx)("div", {
+                                children: (0, wo.jsx)(Lo, {
+                                    label: "Loading ECS clusters"
+                                })
+                            }), r.map((function(e, n) {
+                                return (0, wo.jsxs)("div", {
+                                    children: [(0, wo.jsx)(Af, {
+                                        cluster: e,
+                                        keyedState: null === t || void 0 === t ? void 0 : t.keyed(null === e || void 0 === e ? void 0 : e.cluster_name)
+                                    }), n < r.length - 1 && (0, wo.jsx)(aa, {
+                                        top: "2pt",
+                                        bottom: "2pt",
+                                        dotted: !0
+                                    })]
+                                }, null === e || void 0 === e ? void 0 : e.cluster_name)
+                            }))]
+                        })]
                     })
                 },
                 Af = function(e) {
-                    var t, n = l(Xa(e.keyedState), 2),
-                        r = n[0],
-                        o = n[1],
-                        i = function() {
-                            return r["detail"]
-                        },
-                        a = e.commonInitialSubstring ? null === (t = e.cluster) || void 0 === t ? void 0 : t.replace(e.commonInitialSubstring, "") : e.cluster;
+                    var t, n, r, o = l(Xa(e.keyedState), 2),
+                        i = o[0],
+                        a = o[1],
+                        s = function() {
+                            return i["detail"]
+                        };
                     return (0, wo.jsxs)("div", {
                         children: [(0, wo.jsx)("span", {
                             onClick: function() {
-                                return o(et({}, e = "detail", !r[e]));
+                                return a(et({}, e = "detail", !i[e]));
                                 var e
                             },
                             className: "pointer",
                             style: {
-                                fontWeight: i() ? "bold" : "inherit"
+                                fontWeight: s() ? "bold" : "inherit"
                             },
-                            children: a
+                            children: null === (t = e.cluster) || void 0 === t ? void 0 : t.cluster_name
                         }), (0, wo.jsx)(la, {
-                            href: "https://us-east-1.console.aws.amazon.com/ecs/v2/clusters/".concat(a, "/services?region=us-east-1"),
+                            href: "https://us-east-1.console.aws.amazon.com/ecs/v2/clusters/".concat(null === (n = e.cluster) || void 0 === n ? void 0 : n.cluster_name, "/services?region=us-east-1"),
                             style: {
                                 marginLeft: "6pt"
                             }
-                        }), i() ? (0, wo.jsx)(wo.Fragment, {
-                            children: (0, wo.jsx)(Tf, {
+                        }), s() ? (0, wo.jsx)(wo.Fragment, {
+                            children: (0, wo.jsx)(zf, {
                                 cluster: e.cluster,
-                                clusterDisplayName: a,
+                                clusterDisplayName: null === (r = e.cluster) || void 0 === r ? void 0 : r.cluster_name,
                                 keyedState: e.keyedState
                             })
                         }) : (0, wo.jsx)(wo.Fragment, {})]
                     })
                 },
                 zf = function(e) {
+                    var n, r, o, i, a, s, u, c, d, p, f = l(Xa(e.keyedState), 2),
+                        h = f[0],
+                        g = f[1],
+                        y = function() {
+                            return h["show-services"]
+                        },
+                        m = function() {
+                            return g({
+                                "show-services": !y()
+                            })
+                        },
+                        v = Ya("//aws/ecs/clusters/".concat(encodeURIComponent(null === (n = e.cluster) || void 0 === n ? void 0 : n.cluster_name)), {
+                            cache: !0
+                        });
+                    return (0, t.useEffect)((function() {
+                        m()
+                    }), []), (0, wo.jsx)("div", {
+                        className: "box",
+                        style: {
+                            background: "inherit",
+                            marginTop: "2pt",
+                            marginBottom: "3pt",
+                            overflow: "auto"
+                        },
+                        children: (0, wo.jsx)(lf, {
+                            data: v.data,
+                            yaml: !0,
+                            both: !0,
+                            children: (0, wo.jsxs)("small", {
+                                children: [(0, wo.jsx)("b", {
+                                    children: "Cluster ARN"
+                                }), ": ", null === (r = v.data) || void 0 === r ? void 0 : r.cluster_arn, " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("b", {
+                                    children: "Status"
+                                }), ": ", null === (o = v.data) || void 0 === o ? void 0 : o.status, " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("b", {
+                                    children: "Deployed"
+                                }), ": ", ha.Format(null === (i = v.data) || void 0 === i ? void 0 : i.most_recent_deployment_at), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("b", {
+                                    children: "Services"
+                                }), ": ", null === (a = v.data) || void 0 === a || null === (s = a.services) || void 0 === s ? void 0 : s.length, (null === (u = v.data) || void 0 === u || null === (c = u.services) || void 0 === c ? void 0 : c.length) > 0 && (0, wo.jsxs)(wo.Fragment, {
+                                    children: ["\xa0", y() ? (0, wo.jsxs)(wo.Fragment, {
+                                        children: [(0, wo.jsx)("span", {
+                                            onClick: m,
+                                            className: "pointer",
+                                            children: po.DownArrow
+                                        }), (0, wo.jsx)(Of, {
+                                            cluster: null === (d = v.data) || void 0 === d ? void 0 : d.cluster_name,
+                                            services: null === (p = v.data) || void 0 === p ? void 0 : p.services
+                                        })]
+                                    }) : (0, wo.jsx)(wo.Fragment, {
+                                        children: (0, wo.jsx)("span", {
+                                            onClick: m,
+                                            className: "pointer",
+                                            children: po.UpArrow
+                                        })
+                                    })]
+                                })]
+                            })
+                        })
+                    })
+                },
+                Of = function(e) {
+                    var t, n = wt.LongestCommonInitialSubstring(e.services, (function(e) {
+                        return e.service_name
+                    }));
+                    return (0, wo.jsx)("div", {
+                        className: "box bigmargin smallpadding nobackground",
+                        children: (0, wo.jsx)("ul", {
+                            children: null === (t = e.services) || void 0 === t ? void 0 : t.map((function(t, r) {
+                                return (0, wo.jsx)(wo.Fragment, {
+                                    children: (0, wo.jsxs)("li", {
+                                        children: [(0, wo.jsx)("b", {
+                                            children: t.service_name == t.service_display_name ? (0, wo.jsx)(wo.Fragment, {
+                                                children: (0, wo.jsxs)("span", {
+                                                    onClick: function() {
+                                                        fo.CopyText(t.service_name)
+                                                    },
+                                                    style: {
+                                                        cursor: "copy"
+                                                    },
+                                                    children: [(0, wo.jsx)("b", {
+                                                        id: "tooltip-".concat(t.service_name),
+                                                        children: t.service_name.substring(n.length)
+                                                    }), (0, wo.jsx)(oa, {
+                                                        id: "tooltip-".concat(t.service_name),
+                                                        text: t.service_name,
+                                                        position: "right",
+                                                        shape: "squared"
+                                                    })]
+                                                })
+                                            }) : (0, wo.jsx)(wo.Fragment, {
+                                                children: t.service_name
+                                            })
+                                        }), (0, wo.jsx)(la, {
+                                            href: "https://us-east-1.console.aws.amazon.com/ecs/v2/clusters/".concat(e.cluster, "/services/").concat(t.service_name, "/health?region=us-east-1"),
+                                            style: {
+                                                marginLeft: "6pt"
+                                            }
+                                        }), "\xa0|\xa0", (0, wo.jsxs)("small", {
+                                            children: [(0, wo.jsx)("b", {
+                                                children: "Logs"
+                                            }), (0, wo.jsx)(la, {
+                                                href: "https://us-east-1.console.aws.amazon.com/ecs/v2/clusters/".concat(e.cluster, "/services/").concat(t.service_name, "/logs?region=us-east-1"),
+                                                style: {
+                                                    marginLeft: "4pt"
+                                                }
+                                            })]
+                                        }), (0, wo.jsx)("br", {}), (0, wo.jsxs)("small", {
+                                            children: [(0, wo.jsx)("b", {
+                                                children: "Service ARN"
+                                            }), ": ", t.service_arn, " ", (0, wo.jsx)("br", {}), t.service_name == t.service_display_name && (0, wo.jsxs)(wo.Fragment, {
+                                                children: [(0, wo.jsx)("b", {
+                                                    children: "Service Name"
+                                                }), ": Service: ", t.service_display_name, " ", (0, wo.jsx)("br", {})]
+                                            }), (0, wo.jsx)("b", {
+                                                children: "Task Definition"
+                                            }), ": ", t.task_display_name, (0, wo.jsx)(la, {
+                                                href: "https://us-east-1.console.aws.amazon.com/ecs/v2/task-definitions/".concat(t.task_name, "?region=us-east-1"),
+                                                style: {
+                                                    marginLeft: "4pt"
+                                                }
+                                            }), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("b", {
+                                                children: "Task Definition ARN"
+                                            }), ": ", t.task_arn, (0, wo.jsx)(la, {
+                                                href: "https://us-east-1.console.aws.amazon.com/ecs/v2/task-definitions/".concat(t.task_name, "/1/containers?region=us-east-1"),
+                                                style: {
+                                                    marginLeft: "4pt"
+                                                }
+                                            })]
+                                        }), r < e.services.length - 1 && (0, wo.jsxs)(wo.Fragment, {
+                                            children: [(0, wo.jsx)("br", {}), (0, wo.jsx)("br", {})]
+                                        })]
+                                    })
+                                })
+                            }))
+                        })
+                    })
+                },
+                _f = function(e) {
                     var t = e.keyedState,
                         n = e.hide,
-                        r = Ua("//aws/ecs/clusters"),
-                        o = wt.LongestCommonInitialSubstring(r.data);
+                        r = Ya("//aws/ecs/tasks/latest");
                     return (0, wo.jsxs)("div", {
                         style: {
                             marginBottom: "8pt"
                         },
                         children: [(0, wo.jsxs)("div", {
                             children: [(0, wo.jsx)("b", {
-                                children: "AWS ESC Clusters"
+                                children: "AWS ECS Tasks Definitions"
                             }), "\xa0\xa0", !r.loading && (0, wo.jsxs)("small", {
                                 children: ["(", null === r || void 0 === r ? void 0 : r.length, ")"]
                             }), (0, wo.jsx)("b", {
                                 style: {
                                     float: "right",
                                     fontSize: "small",
                                     marginTop: "2pt",
@@ -68494,33 +68667,140 @@
                         }), (0, wo.jsxs)("div", {
                             style: {
                                 width: "100%"
                             },
                             className: "box lighten nomargin",
                             children: [r.loading && (0, wo.jsx)("div", {
                                 children: (0, wo.jsx)(Lo, {
-                                    label: "Loading ECS clusters"
+                                    label: "Loading ECS tasks"
                                 })
                             }), r.map((function(e, n) {
                                 return (0, wo.jsxs)("div", {
-                                    children: [(0, wo.jsx)(Af, {
-                                        cluster: e,
-                                        commonInitialSubstring: o,
-                                        keyedState: null === t || void 0 === t ? void 0 : t.keyed(e)
+                                    children: [(0, wo.jsx)(Uf, {
+                                        task: e,
+                                        keyedState: null === t || void 0 === t ? void 0 : t.keyed(null === e || void 0 === e ? void 0 : e.task_name)
                                     }), n < r.length - 1 && (0, wo.jsx)(aa, {
                                         top: "2pt",
                                         bottom: "2pt",
                                         dotted: !0
                                     })]
-                                }, e)
+                                }, null === e || void 0 === e ? void 0 : e.task_name)
                             }))]
                         })]
                     })
                 },
-                Of = function() {
+                Uf = function(e) {
+                    var t = l(Xa(e.keyedState), 2),
+                        n = t[0],
+                        r = t[1],
+                        o = function() {
+                            return n["detail"]
+                        };
+                    return (0, wo.jsxs)("div", {
+                        children: [(0, wo.jsx)("span", {
+                            onClick: function() {
+                                return r(et({}, e = "detail", !n[e]));
+                                var e
+                            },
+                            className: "pointer",
+                            style: {
+                                fontWeight: o() ? "bold" : "inherit"
+                            },
+                            children: e.task
+                        }), (0, wo.jsx)(la, {
+                            href: "https://us-east-1.console.aws.amazon.com/ecs/v2/task-definitions/".concat(e.task, "?region=us-east-1"),
+                            style: {
+                                marginLeft: "6pt"
+                            }
+                        }), o() && (0, wo.jsx)(wo.Fragment, {
+                            children: (0, wo.jsx)(Pf, {
+                                task: e.task,
+                                keyedState: e.keyedState
+                            })
+                        })]
+                    })
+                },
+                Pf = function(e) {
+                    var n, r, o, i, a, s = l(Xa(e.keyedState), 2),
+                        u = (s[0], s[1], Ya("//aws/ecs/tasks/".concat(encodeURIComponent(e.task)), {
+                            cache: !0
+                        }));
+                    (0, t.useEffect)((function() {}), []);
+                    var c = {
+                            fontSize: "small",
+                            verticalAlign: "top"
+                        },
+                        d = nt(nt({}, c), {}, {
+                            paddingRight: "3pt",
+                            whiteSpace: "nowrap"
+                        }),
+                        p = nt(nt({}, c), {}, {
+                            whiteSpace: "break-spaces",
+                            wordBreak: "break-all"
+                        });
+                    return (0, wo.jsx)("div", {
+                        className: "box",
+                        style: {
+                            background: "inherit",
+                            marginTop: "2pt",
+                            marginBottom: "3pt",
+                            overflow: "auto"
+                        },
+                        children: (0, wo.jsx)(lf, {
+                            data: u.data,
+                            yaml: !0,
+                            both: !0,
+                            children: (0, wo.jsx)("small", {
+                                children: (0, wo.jsx)("table", {
+                                    children: (0, wo.jsxs)("tbody", {
+                                        children: [(0, wo.jsxs)("tr", {
+                                            children: [(0, wo.jsxs)("td", {
+                                                style: d,
+                                                children: [(0, wo.jsx)("b", {
+                                                    children: "Task Definition Name"
+                                                }), ":"]
+                                            }), (0, wo.jsx)("td", {
+                                                style: p,
+                                                children: (0, wo.jsx)("u", {
+                                                    children: null === (n = u.data) || void 0 === n ? void 0 : n.task_display_name
+                                                })
+                                            })]
+                                        }), (0, wo.jsxs)("tr", {
+                                            children: [(0, wo.jsxs)("td", {
+                                                style: d,
+                                                children: [(0, wo.jsx)("b", {
+                                                    children: "Task Definition ARN"
+                                                }), ":"]
+                                            }), (0, wo.jsxs)("td", {
+                                                style: p,
+                                                children: [null === (r = u.data) || void 0 === r ? void 0 : r.task_arn, (0, wo.jsx)(la, {
+                                                    href: "https://us-east-1.console.aws.amazon.com/ecs/v2/task-definitions/".concat(null === (o = u.data) || void 0 === o ? void 0 : o.task_name).concat(null !== (i = u.data) && void 0 !== i && i.task_revision ? "/" + u.data.task_revision : "", "/containers?region=us-east-1"),
+                                                    style: {
+                                                        marginLeft: "6pt"
+                                                    }
+                                                })]
+                                            })]
+                                        }), (0, wo.jsxs)("tr", {
+                                            children: [(0, wo.jsxs)("td", {
+                                                style: d,
+                                                children: [(0, wo.jsx)("b", {
+                                                    children: "Task Definition Revision"
+                                                }), ":"]
+                                            }), (0, wo.jsx)("td", {
+                                                style: p,
+                                                children: null === (a = u.data) || void 0 === a ? void 0 : a.task_revision
+                                            })]
+                                        })]
+                                    })
+                                })
+                            })
+                        })
+                    })
+                },
+                Rf = function() {
                     var e = Xa(),
                         n = $a(),
                         r = [{
                             type: "stack",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
                                 return (0, wo.jsx)(Df, {
@@ -68591,15 +68871,24 @@
                                     hide: n
                                 })
                             }
                         }, {
                             type: "ecs-clusters",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(zf, {
+                                return (0, wo.jsx)(Tf, {
+                                    keyedState: o.keyed(t),
+                                    hide: n
+                                })
+                            }
+                        }, {
+                            type: "ecs-tasks",
+                            create: function(e, t, n, r) {
+                                var o = r.keyedState;
+                                return (0, wo.jsx)(_f, {
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }],
                         o = Za(r),
                         i = Za(r);
@@ -68667,14 +68956,20 @@
                                         }
                                     }), (0, wo.jsx)(hf, {
                                         showEcsClusters: function() {
                                             return o.selected("ecs-clusters")
                                         },
                                         toggleEcsClusters: function() {
                                             return o.toggle("ecs-clusters")
+                                        },
+                                        showEcsTasks: function() {
+                                            return o.selected("ecs-tasks")
+                                        },
+                                        toggleEcsTasks: function() {
+                                            return o.toggle("ecs-tasks")
                                         }
                                     }), (0, wo.jsx)(ts, {
                                         toggleSecrets: function(e) {
                                             return o.toggle("secrets", e) ? n.setList("secrets", e) : n.unsetList("secrets", e)
                                         },
                                         selectedSecrets: function(e) {
                                             return o.selected("secrets", e)
@@ -68712,16 +69007,16 @@
                                         }, t.key)
                                     }))
                                 })]
                             })
                         })
                     })
                 },
-                _f = function(e) {
-                    var t = Fa();
+                Ff = function(e) {
+                    var t = Wa();
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "container",
                             id: "login_container",
                             children: (0, wo.jsxs)("div", {
                                 className: "boxstyle check-warn",
                                 style: {
@@ -68749,88 +69044,88 @@
                                         })
                                     }), " page."]
                                 })]
                             })
                         })
                     })
                 },
-                Uf = function() {
+                Bf = function() {
                     var e = me().state.url;
                     return e.startsWith(window.location.origin) && (e = e.substring(window.location.origin.length)), (0, wo.jsx)(ze, {
                         to: e,
                         replace: !0
                     })
                 },
-                Pf = function(e) {
+                Yf = function(e) {
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "box thickborder",
                             style: {
                                 marginBottom: "6pt"
                             },
-                            children: (0, wo.jsx)(pa, {
+                            children: (0, wo.jsx)(ma, {
                                 certificate: e.certificate
                             })
                         })
                     })
                 },
-                Rf = function(e) {
+                Qf = function(e) {
                     var t, n = l($e(), 1)[0].get("hostname"),
-                        r = Ua("/certificates?hostname=".concat(n));
+                        r = Ya("/certificates?hostname=".concat(n));
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsxs)("div", {
                             className: "container",
                             style: {
                                 width: "800pt"
                             },
                             children: [(0, wo.jsx)("b", {
                                 children: "SSL Certificates"
                             }), null === r || void 0 === r || null === (t = r.data) || void 0 === t ? void 0 : t.map((function(e) {
                                 return (0, wo.jsx)("div", {
-                                    children: (0, wo.jsx)(Pf, {
+                                    children: (0, wo.jsx)(Yf, {
                                         certificate: e
                                     })
                                 }, e.serial_number)
                             }))]
                         })
                     })
                 },
-                Ff = function(e) {
-                    var t = Ua("/portal_access_key");
+                Gf = function(e) {
+                    var t = Ya("/portal_access_key");
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsxs)("div", {
                             className: "container",
                             style: {
                                 width: "800pt"
                             },
                             children: [(0, wo.jsx)("b", {
                                 children: "Portal Access Key"
                             }), (0, wo.jsx)("div", {
                                 className: "box thickborder",
                                 style: {
                                     marginBottom: "6pt"
                                 },
-                                children: (0, wo.jsx)(ca, {
+                                children: (0, wo.jsx)(ga, {
                                     accessKey: t.data
                                 })
                             })]
                         })
                     })
                 },
-                Bf = function() {
-                    var e = Ua("/users/projects", {
+                Wf = function() {
+                    var e = Ya("/users/projects", {
                             cache: !0
                         }),
-                        t = Ua("/users/roles", {
+                        t = Ya("/users/roles", {
                             cache: !0
                         }),
-                        n = Ua("/users/institutions", {
+                        n = Ya("/users/institutions", {
                             cache: !0
                         }),
-                        r = Ua("/users/statuses", {
+                        r = Ya("/users/statuses", {
                             cache: !0
                         }),
                         o = {
                             projectTitle: function(t) {
                                 var n, r;
                                 return (null === (n = e.data) || void 0 === n || null === (r = n.find((function(e) {
                                     return e.id === t
@@ -68878,15 +69173,15 @@
                                 return (null === e || void 0 === e ? void 0 : e.map((function(e) {
                                     return o.title(e)
                                 })).join(", ")) || ""
                             }
                         };
                     return o
                 },
-                Yf = [{
+                Hf = [{
                     name: "email",
                     label: "Email Address",
                     type: "email",
                     focus: !0,
                     required: !0
                 }, {
                     name: "first_name",
@@ -68933,39 +69228,39 @@
                 }, {
                     name: "uuid",
                     label: "UUID",
                     readonly: !0,
                     readonlyOverridableOnCreate: !0,
                     readonlyOverridableOnCreateMessage: "Warning: Only set UUID if you know what you are doing."
                 }],
-                Qf = {
+                Vf = {
                     PrincipalInvestigatorLine: function(e) {
                         var t, n, r = e.institution,
-                            o = Bf();
+                            o = Wf();
                         return (0, wo.jsx)("div", {
                             style: e.style,
                             children: o.principleInvestigator(r) && (0, wo.jsxs)("small", {
                                 children: [(0, wo.jsxs)("b", {
                                     children: ["Principle Investigator ", po.RightArrow]
                                 }), " ", null === (t = o.principleInvestigator(r)) || void 0 === t ? void 0 : t.name, "\xa0", (0, wo.jsx)(la, {
                                     href: $r.Path("/users/".concat(null === (n = o.principleInvestigator(r)) || void 0 === n ? void 0 : n.uuid))
                                 })]
                             })
                         })
                     },
                     useUserInputs: function() {
-                        var e = Fa(),
-                            n = tn.IsFoursightFourfront(e) ? Yf.filter((function(e) {
+                        var e = Wa(),
+                            n = tn.IsFoursightFourfront(e) ? Hf.filter((function(e) {
                                 return "project" !== e.name && "role" !== e.name && "institution" !== e.name
-                            })) : Yf;
+                            })) : Hf;
                         return (0, t.useState)(no.Clone(n))
                     }
                 },
-                Gf = function(e) {
-                    var t = Ua("/users/".concat(e.email, "?raw=true"));
+                Zf = function(e) {
+                    var t = Ya("/users/".concat(e.email, "?raw=true"));
                     return (0, wo.jsxs)("pre", {
                         className: "box",
                         children: [(0, wo.jsx)("span", {
                             style: {
                                 float: "right",
                                 marginTop: "-6pt",
                                 fontSize: "large",
@@ -68974,19 +69269,19 @@
                             onClick: function() {
                                 return t.refresh()
                             },
                             children: po.Refresh
                         }), t.loading ? (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsx)(Lo, {})
                         }) : (0, wo.jsx)(wo.Fragment, {
-                            children: Ia.Format(t.data)
+                            children: Ca.Format(t.data)
                         })]
                     })
                 },
-                Wf = function(e) {
+                qf = function(e) {
                     var n = {
                             color: "var(--box-fg)",
                             fontWeight: "bold",
                             fontSize: "small",
                             paddingTop: "1pt",
                             verticalAlign: "top",
                             width: "5%",
@@ -69095,16 +69390,16 @@
                                         })]
                                     }, o.name)
                                 }))
                             })
                         })
                     })
                 },
-                Hf = function(e) {
-                    var t = Bf(),
+                Jf = function(e) {
+                    var t = Wf(),
                         n = [{
                             label: "Email",
                             name: "email"
                         }, {
                             label: "First Name",
                             name: "first_name"
                         }, {
@@ -69127,61 +69422,61 @@
                             name: "role",
                             map: function(n) {
                                 return t.userRoleTitle(e.user, e.user.project)
                             }
                         }, {
                             label: "Roles",
                             name: "roles",
-                            ui: (0, wo.jsx)(Vf, {
+                            ui: (0, wo.jsx)(Kf, {
                                 user: e.user
                             }),
                             toggle: !0
                         }, {
                             label: "Institution",
                             name: "institution",
                             map: function(e) {
                                 return t.institutionTitle(e)
                             },
                             subComponent: function(e) {
-                                return (0, wo.jsx)(Qf.PrincipalInvestigatorLine, {
+                                return (0, wo.jsx)(Vf.PrincipalInvestigatorLine, {
                                     institution: e
                                 })
                             }
                         }, {
                             label: "Status",
                             name: "status",
                             map: function(e) {
                                 return t.statusTitle(e)
                             }
                         }, {
                             label: "Created",
                             name: "created",
                             map: function(e) {
-                                return Wa.Format(e)
+                                return ha.Format(e)
                             }
                         }, {
                             label: "Updated",
                             name: "updated",
                             map: function(e) {
-                                return Wa.Format(e)
+                                return ha.Format(e)
                             }
                         }, {
                             label: "UUID",
                             name: "uuid"
                         }];
-                    return tn.IsFoursightFourfront(Fa()) && (n = n.filter((function(e) {
+                    return tn.IsFoursightFourfront(Wa()) && (n = n.filter((function(e) {
                         return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
-                    }))), (0, wo.jsx)(Wf, {
+                    }))), (0, wo.jsx)(qf, {
                         keys: n,
                         value: e.user,
                         separators: !0
                     })
                 },
-                Vf = function(e) {
-                    var t = Bf();
+                Kf = function(e) {
+                    var t = Wf();
                     return (0, wo.jsx)("div", {
                         className: "box lighten",
                         style: {
                             marginTop: "2pt",
                             marginBottom: "2pt"
                         },
                         children: (0, wo.jsx)("table", {
@@ -69244,21 +69539,21 @@
                                         })]
                                     }, e.project)
                                 }))]
                             })
                         })
                     })
                 },
-                Zf = function(e) {
+                Xf = function(e) {
                     var n, r, o, i = je().email,
                         a = l((0, t.useState)(!1), 2),
                         s = a[0],
                         u = a[1],
                         c = Me();
-                    var d = Ua({
+                    var d = Ya({
                         url: "/users/".concat(i),
                         onData: function(e) {
                             return Dt.IsObject(e) ? [e] : e
                         },
                         nofetch: !0
                     });
                     return (0, t.useEffect)((function() {
@@ -69368,26 +69663,26 @@
                                                 float: "right",
                                                 fontSize: "small",
                                                 marginTop: "-1pt",
                                                 marginRight: "2pt"
                                             },
                                             children: "Edit"
                                         })]
-                                    }), s ? (0, wo.jsx)(Gf, {
+                                    }), s ? (0, wo.jsx)(Zf, {
                                         email: e.email
-                                    }) : (0, wo.jsx)(Hf, {
+                                    }) : (0, wo.jsx)(Jf, {
                                         user: e
                                     })]
                                 }, e.uuid)
                             }))]
                         })
                     })
                 },
-                qf = function(e) {
-                    var n = Ua(e.url, {
+                $f = function(e) {
+                    var n = Ya(e.url, {
                             nofetch: !0,
                             cache: !0
                         }),
                         r = l((0, t.useState)(e.selected), 2),
                         o = r[0],
                         i = r[1];
                     return (0, t.useEffect)((function() {
@@ -69419,15 +69714,15 @@
                                 }, e.id) : null
                             }))]
                         }), e.subComponent && (0, wo.jsx)(wo.Fragment, {
                             children: e.subComponent(o)
                         })]
                     })
                 },
-                Jf = function(e) {
+                eh = function(e) {
                     var n = e.input,
                         r = e.valueOf,
                         o = e.handleChange,
                         i = e.isDisabled,
                         a = l((0, t.useState)(n.readonly), 2),
                         s = a[0],
                         u = a[1];
@@ -69486,15 +69781,15 @@
                                         children: n.readonlyOverridableOnCreateMessage
                                     })
                                 })]
                             })]
                         })]
                     })
                 },
-                Kf = function(e) {
+                th = function(e) {
                     var n = e.inputs,
                         r = (e.setInputs, e.title, e.loading),
                         o = e.onCreate,
                         i = e.onUpdate,
                         a = e.onDelete,
                         s = e.onCancel,
                         u = e.onRefresh,
@@ -69745,27 +70040,27 @@
                                                             }), (0, wo.jsx)("option", {
                                                                 value: !0,
                                                                 children: "True"
                                                             })]
                                                         })
                                                     }) : (0, wo.jsx)(wo.Fragment, {
                                                         children: "select" === e.type ? (0, wo.jsx)(wo.Fragment, {
-                                                            children: (0, wo.jsx)(qf, {
+                                                            children: (0, wo.jsx)($f, {
                                                                 id: e.name,
                                                                 url: e.url,
                                                                 required: e.required,
                                                                 selected: _(e),
                                                                 onChange: A,
                                                                 disabled: B() || e.readonly,
                                                                 setLoadingCount: L,
                                                                 subComponent: e.subComponent,
                                                                 reset: k
                                                             })
                                                         }) : (0, wo.jsx)(wo.Fragment, {
-                                                            children: (0, wo.jsx)(Jf, {
+                                                            children: (0, wo.jsx)(eh, {
                                                                 input: e,
                                                                 valueOf: _,
                                                                 handleChange: A,
                                                                 isDisabled: B,
                                                                 isCreate: !Dt.IsNull(o)
                                                             })
                                                         })
@@ -69928,28 +70223,28 @@
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                Xf = function() {
-                    var e = Ua(rn.Url("/users"), {
+                nh = function() {
+                    var e = Ya(rn.Url("/users"), {
                             method: "POST",
                             nofetch: !0
                         }),
-                        n = l(Qf.useUserInputs(), 2),
+                        n = l(Vf.useUserInputs(), 2),
                         r = n[0],
                         o = (n[1], Me());
                     return (0, t.useEffect)((function() {
                         var e = r.find((function(e) {
                             return "institution" === e.name
                         }));
                         e && (e.subComponent = function(e) {
-                            return (0, wo.jsx)(Qf.PrincipalInvestigatorLine, {
+                            return (0, wo.jsx)(Vf.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         })
                     }), []), (0, wo.jsx)("center", {
                         children: (0, wo.jsx)("table", {
                             children: (0, wo.jsxs)("tbody", {
                                 children: [(0, wo.jsx)("tr", {
@@ -69976,15 +70271,15 @@
                                                     children: "List"
                                                 })
                                             })
                                         })]
                                     })
                                 }), (0, wo.jsx)("tr", {
                                     children: (0, wo.jsx)("td", {
-                                        children: (0, wo.jsx)(Kf, {
+                                        children: (0, wo.jsx)(th, {
                                             title: "Edit User",
                                             inputs: r,
                                             onCreate: function(t) {
                                                 t.admin ? (delete t.admin, t = nt(nt({}, t), {}, {
                                                     groups: ["admin"]
                                                 })) : (delete t.admin, t = nt(nt({}, t), {}, {
                                                     groups: []
@@ -70004,61 +70299,61 @@
                                         })
                                     })
                                 })]
                             })
                         })
                     })
                 },
-                $f = function() {
+                rh = function() {
                     var e = je().uuid,
-                        n = l(Qf.useUserInputs(), 2),
+                        n = l(Vf.useUserInputs(), 2),
                         r = n[0],
                         o = n[1],
                         i = l((0, t.useState)(!1), 2),
                         a = i[0],
                         s = i[1],
                         u = l(Ls(), 1)[0],
-                        d = Ua({
+                        d = Ya({
                             url: "/users/".concat(e),
                             nofetch: !0,
                             onData: function(e) {
                                 o((function(t) {
                                     var n, r = c(t);
                                     try {
                                         for (r.s(); !(n = r.n()).done;) {
                                             var o, i = n.value;
                                             "email" === i.name ? i.value = e.email : "first_name" === i.name ? i.value = e.first_name : "last_name" === i.name ? i.value = e.last_name : "admin" === i.name ? i.value = !(null === (o = e.groups) || void 0 === o || !o.includes("admin")) : "project" === i.name ? i.value = e.project : "role" === i.name ? i.value = function(t) {
                                                 return void 0 === t || null === t ? "-" : f.userRole(e, t || (null === e || void 0 === e ? void 0 : e.project)) || "-"
-                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = Wa.Format(e.created) : "updated" === i.name ? i.value = Wa.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
+                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = ha.Format(e.created) : "updated" === i.name ? i.value = ha.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
                                         }
                                     } catch (a) {
                                         r.e(a)
                                     } finally {
                                         r.f()
                                     }
                                     return p(t)
                                 }))
                             },
                             onError: function(e) {
                                 404 === e.status && s(!0)
                             }
                         }),
-                        f = Bf(),
+                        f = Wf(),
                         h = Me();
 
                     function g() {
                         h($r.Path("/users/".concat(e)))
                     }
                     return (0, t.useEffect)((function() {
                         d.fetch();
                         var e = r.find((function(e) {
                             return "institution" === e.name
                         }));
                         e && (e.subComponent = function(e) {
-                            return (0, wo.jsx)(Qf.PrincipalInvestigatorLine, {
+                            return (0, wo.jsx)(Vf.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         })
                     }), [e]), (0, wo.jsx)("center", {
                         children: (0, wo.jsx)("table", {
                             children: (0, wo.jsxs)("tbody", {
                                 children: [(0, wo.jsx)("tr", {
@@ -70099,15 +70394,15 @@
                                                 children: ["The specified user was not found: ", e, " ", (0, wo.jsx)("p", {}), (0, wo.jsx)("button", {
                                                     className: "button cancel",
                                                     onClick: g,
                                                     children: "Cancel"
                                                 })]
                                             })
                                         }) : (0, wo.jsx)(wo.Fragment, {
-                                            children: (0, wo.jsx)(Kf, {
+                                            children: (0, wo.jsx)(th, {
                                                 title: "Edit User",
                                                 inputs: r,
                                                 setInputs: o,
                                                 onUpdate: function(t) {
                                                     var n, r = (null === (n = d.get("groups")) || void 0 === n ? void 0 : n.filter((function(e) {
                                                         return "admin" !== e
                                                     }))) || [];
@@ -70142,15 +70437,15 @@
                                         })
                                     })
                                 })]
                             })
                         })
                     })
                 },
-                eh = function(e) {
+                oh = function(e) {
                     var n, r = e.columns,
                         o = e.data,
                         i = e.update,
                         a = e.initialSort,
                         s = e.children,
                         u = l($e(), 2),
                         c = u[0],
@@ -70330,27 +70625,27 @@
                                 }), (0, wo.jsx)("tbody", {
                                     children: s
                                 })]
                             })
                         })]
                     })
                 },
-                th = function() {
+                ih = function() {
                     var e = je().environ,
                         n = l($e(), 2),
                         r = n[0],
                         o = n[1],
-                        i = Ua(),
+                        i = Ya(),
                         a = l((0, t.useState)(r.get("search") || ""), 2),
                         s = a[0],
                         u = a[1],
                         c = l((0, t.useState)(wt.HasValue(s)), 2),
                         d = c[0],
                         p = c[1],
-                        f = Bf();
+                        f = Wf();
 
                     function h(t) {
                         var n = t.limit,
                             o = t.offset,
                             a = t.sort,
                             s = t.search,
                             u = t.onDone;
@@ -70480,15 +70775,15 @@
                                     style: {
                                         height: "1px",
                                         background: ln.GetForegroundColor(),
                                         marginTop: "2pt",
                                         marginBottom: "4pt"
                                     }
                                 })]
-                            }), (0, wo.jsx)(eh, {
+                            }), (0, wo.jsx)(oh, {
                                 columns: [{
                                     label: ""
                                 }, {
                                     label: "User",
                                     key: "email"
                                 }, {
                                     label: "Groups",
@@ -70623,16 +70918,16 @@
                                         })]
                                     }, e.uuid)
                                 }))
                             })]
                         })
                     })
                 },
-                nh = function() {
-                    var e = Fa();
+                ah = function() {
+                    var e = Wa();
 
                     function t() {
                         return "/api/react/".concat(tn.PreferredName(tn.Default(e)), "/login")
                     }
                     return (0, wo.jsx)(He, {
                         children: (0, wo.jsxs)(Pu, {
                             children: [(0, wo.jsx)(Uu, {}), (0, wo.jsx)("div", {
@@ -70661,142 +70956,142 @@
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ",
                                         element: (0, wo.jsx)(ze, {
                                             to: t()
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/accounts",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(vs, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/env",
-                                        element: (0, wo.jsx)(wa.KnownEnvRequired, {
+                                        element: (0, wo.jsx)(La.KnownEnvRequired, {
                                             children: (0, wo.jsx)(Du, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/env",
-                                        element: (0, wo.jsx)(wa.KnownEnvRequired, {
+                                        element: (0, wo.jsx)(La.KnownEnvRequired, {
                                             children: (0, wo.jsx)(Du, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/login",
-                                        element: (0, wo.jsx)(wa.KnownEnvRequired, {
+                                        element: (0, wo.jsx)(La.KnownEnvRequired, {
                                             children: (0, wo.jsx)(af, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/checks",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(cu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/checksnew",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(yu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/checks/:check/history",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(Nu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/home",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(Ru, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/info",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(Yu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(th, {})
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
+                                            children: (0, wo.jsx)(ih, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users/:email",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Zf, {})
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
+                                            children: (0, wo.jsx)(Xf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users/edit/:uuid",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)($f, {})
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
+                                            children: (0, wo.jsx)(rh, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users/create",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Xf, {})
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
+                                            children: (0, wo.jsx)(nh, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/gac/:environCompare",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(sf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/aws/s3",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(Is, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/aws/infrastructure",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Of, {})
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
+                                            children: (0, wo.jsx)(Rf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/certificates",
-                                        element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(Rf, {})
+                                        element: (0, wo.jsx)(La.KnownEnvRequired, {
+                                            children: (0, wo.jsx)(Qf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/portal_access_key",
-                                        element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(Ff, {})
+                                        element: (0, wo.jsx)(La.KnownEnvRequired, {
+                                            children: (0, wo.jsx)(Gf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/apicache",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
                                             children: (0, wo.jsx)(xs, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/forbidden",
                                         element: (0, wo.jsx)(Su, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/error",
-                                        element: (0, wo.jsx)(ma, {})
+                                        element: (0, wo.jsx)(wa, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/error",
-                                        element: (0, wo.jsx)(ma, {})
+                                        element: (0, wo.jsx)(wa, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/redirect",
-                                        element: (0, wo.jsx)(Uf, {})
+                                        element: (0, wo.jsx)(Bf, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "*",
-                                        element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(_f, {})
+                                        element: (0, wo.jsx)(La.AuthorizationRequired, {
+                                            children: (0, wo.jsx)(Ff, {})
                                         })
                                     })]
                                 })
                             }), (0, wo.jsx)(Lu, {})]
                         })
                     })
                 },
-                rh = o.createRoot(document.getElementById("root"));
-            "1" === Bt.Get("test_mode_strict_mode") ? rh.render((0, wo.jsx)(t.StrictMode, {
-                children: (0, wo.jsx)(nh, {})
-            })) : rh.render((0, wo.jsx)("table", {
+                sh = o.createRoot(document.getElementById("root"));
+            "1" === Bt.Get("test_mode_strict_mode") ? sh.render((0, wo.jsx)(t.StrictMode, {
+                children: (0, wo.jsx)(ah, {})
+            })) : sh.render((0, wo.jsx)("table", {
                 style: {
                     width: "100%"
                 },
                 cellPadding: "0",
                 cellSpacing: "0",
                 children: (0, wo.jsx)("tbody", {
                     children: (0, wo.jsx)("tr", {
                         children: (0, wo.jsx)("td", {
-                            children: (0, wo.jsx)(nh, {})
+                            children: (0, wo.jsx)(ah, {})
                         })
                     })
                 })
             }))
         }()
 }();
```

### Comparing `foursight_core-4.3.0.2b6/foursight_core/route_prefixes.py` & `foursight_core-4.4.0/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/routes.py` & `foursight_core-4.4.0/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/run_result.py` & `foursight_core-4.4.0/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/s3_connection.py` & `foursight_core-4.4.0/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/schedule_decorator.py` & `foursight_core-4.4.0/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/sqs_utils.py` & `foursight_core-4.4.0/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/stage.py` & `foursight_core-4.4.0/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/base.html` & `foursight_core-4.4.0/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/header.html` & `foursight_core-4.4.0/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/history.html` & `foursight_core-4.4.0/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/info.html` & `foursight_core-4.4.0/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/unused.html` & `foursight_core-4.4.0/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/user.html` & `foursight_core-4.4.0/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/users.html` & `foursight_core-4.4.0/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/view_checks.html` & `foursight_core-4.4.0/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/foursight_core/templates/view_groups.html` & `foursight_core-4.4.0/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b6/pyproject.toml` & `foursight_core-4.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0.2b6"  # TODO: To become 4.4.0
+version = "4.4.0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.3.0.2b6/PKG-INFO` & `foursight_core-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0.2b6
+Version: 4.4.0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

