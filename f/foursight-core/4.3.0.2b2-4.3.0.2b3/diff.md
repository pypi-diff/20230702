# Comparing `tmp/foursight_core-4.3.0.2b2.tar.gz` & `tmp/foursight_core-4.3.0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.2b2.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.2b3.tar", max compression
```

## Comparing `foursight_core-4.3.0.2b2.tar` & `foursight_core-4.3.0.2b3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-07-02 05:26:54.392623 foursight_core-4.3.0.2b2/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/app.py
--rw-r--r--   0        0        0   103622 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/app_utils.py
--rw-r--r--   0        0        0     1283 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/boto_s3.py
--rw-r--r--   0        0        0     1305 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/boto_sqs.py
--rw-r--r--   0        0        0     2589 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     7293 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/decorators.py
--rw-r--r--   0        0        0    15846 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/deploy.py
--rw-r--r--   0        0        0     8169 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/environment.py
--rw-r--r--   0        0        0    11948 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5597 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3065 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6104 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6213 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     4096 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5216 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    88080 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    35908 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-07-02 05:26:54.400623 foursight_core-4.3.0.2b2/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-07-02 05:26:54.404623 foursight_core-4.3.0.2b2/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-07-02 05:26:54.404623 foursight_core-4.3.0.2b2/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11953 2023-07-02 05:26:54.404623 foursight_core-4.3.0.2b2/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1862144 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/routes.py
--rw-r--r--   0        0        0    22941 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/run_result.py
--rw-r--r--   0        0        0     6380 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     5442 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-07-02 05:26:54.412623 foursight_core-4.3.0.2b2/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1500 2023-07-02 05:26:54.416623 foursight_core-4.3.0.2b2/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-02 10:33:43.538224 foursight_core-4.3.0.2b3/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/app.py
+-rw-r--r--   0        0        0   103622 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/boto_s3.py
+-rw-r--r--   0        0        0     1305 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/boto_sqs.py
+-rw-r--r--   0        0        0     2589 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     7293 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15846 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8169 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/environment.py
+-rw-r--r--   0        0        0    11948 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5597 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3065 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6104 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6213 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     4096 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5216 2023-07-02 10:33:43.546224 foursight_core-4.3.0.2b3/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    88080 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    35908 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11953 2023-07-02 10:33:43.550224 foursight_core-4.3.0.2b3/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1862142 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/routes.py
+-rw-r--r--   0        0        0    22941 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6380 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     5442 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-07-02 10:33:43.558224 foursight_core-4.3.0.2b3/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1500 2023-07-02 10:33:43.562224 foursight_core-4.3.0.2b3/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b3/PKG-INFO
```

### Comparing `foursight_core-4.3.0.2b2/LICENSE.txt` & `foursight_core-4.3.0.2b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/abstract_connection.py` & `foursight_core-4.3.0.2b3/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/app_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/boto_s3.py` & `foursight_core-4.3.0.2b3/foursight_core/boto_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/boto_sqs.py` & `foursight_core-4.3.0.2b3/foursight_core/boto_sqs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/buckets.py` & `foursight_core-4.3.0.2b3/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/check_schema.py` & `foursight_core-4.3.0.2b3/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/check_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0.2b3/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/decorators.py` & `foursight_core-4.3.0.2b3/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/deploy.py` & `foursight_core-4.3.0.2b3/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/environment.py` & `foursight_core-4.3.0.2b3/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/es_connection.py` & `foursight_core-4.3.0.2b3/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/exceptions.py` & `foursight_core-4.3.0.2b3/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/fs_connection.py` & `foursight_core-4.3.0.2b3/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/identity.py` & `foursight_core-4.3.0.2b3/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/mapping.json` & `foursight_core-4.3.0.2b3/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/package.py` & `foursight_core-4.3.0.2b3/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/auth.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/checks.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/envs.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/gac.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/ui/index.html` & `foursight_core-4.3.0.2b3/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0.2b3/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0.2b3/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.276e14ec.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.97f703bf.js.LICENSE.txt */ ! function() {
     var e = {
             3339: function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.RawSha256 = void 0;
                 var r = n(3277),
@@ -50396,14 +50396,17 @@
                                     }), (0, wo.jsx)("br", {})]
                                 })
                             }))]
                         }), (0, wo.jsx)("br", {})]
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
                 Ns = {
+                    Format: uo.FormatDate
+                },
+                Is = {
                     FormatDateTime: function(e) {
                         var n = e.verbose,
                             r = void 0 !== n && n,
                             o = e.timezone,
                             i = void 0 === o || o,
                             a = l((0, t.useState)(new Date), 2),
                             s = a[0],
@@ -50453,36 +50456,36 @@
                                     id: "tooltip-timestamp-".concat(r || i),
                                     text: uo.FormatDateTime(r || i)
                                 })]
                             })
                         })
                     }
                 },
-                Is = Ns,
-                Ds = !1,
-                Ls = !0,
-                Ss = {
+                Ds = Is,
+                Ls = !1,
+                Ss = !0,
+                ks = {
                     Now: function() {
                         return new Date
                     },
                     Format: function(e) {
-                        return uo.FormatDateTime(e, Ds, Ls, true)
+                        return uo.FormatDateTime(e, Ls, Ss, true)
                     },
                     Format24: function(e) {
-                        return uo.FormatDateTime(e, Ds, Ls, true)
+                        return uo.FormatDateTime(e, Ls, Ss, true)
                     },
                     Format12: function(e) {
-                        return uo.FormatDateTime(e, Ds, Ls, false)
+                        return uo.FormatDateTime(e, Ls, Ss, false)
                     },
                     FormatVerbose: function(e) {
-                        return uo.FormatDateTime(e, true, Ls, false)
+                        return uo.FormatDateTime(e, true, Ss, false)
                     },
-                    Live: Is.FormatDateTime
+                    Live: Ds.FormatDateTime
                 },
-                ks = function(e) {
+                Cs = function(e) {
                     var t, n = e.status;
                     return function(e) {
                         return "ok" == e || "done" == e || e.includes("pass") || e.includes("success")
                     }(n = (null === (t = n) || void 0 === t ? void 0 : t.toLowerCase(n).trim()) || "") ? (0, wo.jsx)("b", {
                         style: {
                             color: ln.GetForegroundColor()
                         },
@@ -50511,148 +50514,148 @@
                     }) : (0, wo.jsx)("b", {
                         style: {
                             color: "black"
                         },
                         children: n
                     })
                 },
-                Cs = {
+                Es = {
                     Ago: uo.Ago,
                     Format: uo.FormatDuration,
                     FromNow: uo.FromNow,
-                    Live: Is.FormatDuration
+                    Live: Ds.FormatDuration
                 };
 
-            function Es(e) {
-                e.update()
-            }
-
             function Ts(e) {
                 e.update()
             }
 
             function As(e) {
                 e.update()
             }
 
-            function zs(e, t) {
-                e.__showingResults = !1, Es(t)
+            function zs(e) {
+                e.update()
             }
 
-            function Os(e, t, n) {
-                e.__showingResults = !0, Es(n)
+            function Os(e, t) {
+                e.__showingResults = !1, Ts(t)
             }
 
             function _s(e, t, n) {
-                Ps(e, n) || (n.prepend(e), Es(n))
+                e.__showingResults = !0, Ts(n)
             }
 
             function Us(e, t, n) {
+                Rs(e, n) || (n.prepend(e), Ts(n))
+            }
+
+            function Ps(e, t, n) {
                 e.checks.map((function(e) {
-                    return Bs(e, n)
+                    return Ys(e, n)
                 }));
                 var r = function(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         if (t.get(n).group === e.group) return n
                     }
                     return -1
                 }(e, t);
                 t.remove(r)
             }
 
-            function Ps(e, t) {
+            function Rs(e, t) {
                 for (var n = 0; n < t.length; n++) {
                     if (t.get(n).group === e.group) return !0
                 }
                 return !1
             }
 
-            function Rs(e) {
+            function Fs(e) {
                 return null === e || void 0 === e ? void 0 : e.__showingResults
             }
 
-            function Fs(e) {
+            function Bs(e) {
                 Object.keys(e.kwargs).forEach((function(t) {
                     if (!Dt.IsBoolean(e.kwargs[t]) && !Dt.IsNonEmptyArray(e.kwargs[t])) {
                         var n = "".concat(e.name, ".").concat(t),
                             r = document.getElementById(n),
                             o = null === r || void 0 === r ? void 0 : r.value;
                         e.kwargs[t] = o
                     }
                 }))
             }
 
-            function Bs(e, t) {
+            function Ys(e, t) {
                 if (e.__showingHistory) {
                     e.__showingHistory = !1;
                     var n = function(e, t) {
                         for (var n = 0; n < t.length; n++) {
                             if (t.get(n).name === e.name) return n
                         }
                         return -1
                     }(e, t);
                     t.remove(n)
                 }
             }
 
-            function Ys(e, t, n) {
+            function Qs(e, t, n) {
                 ! function(e, t, n) {
-                    e.__showingHistory ? Bs(e, n) : Qs(e, t, n)
+                    e.__showingHistory ? Ys(e, n) : Gs(e, t, n)
                 }(e, t, n)
             }
 
-            function Qs(e, t, n) {
+            function Gs(e, t, n) {
                 e.__showingHistory || (e.__showingHistory = !0, n.prepend(e))
             }
 
-            function Gs(e, t, n, r, o) {
+            function Ws(e, t, n, r, o) {
                 var i = e.kwargs,
                     a = no.Str(i),
                     s = btoa(a);
-                Hs(e, n), As(n), e.__queueingCheckRun = !0, o({
+                Vs(e, n), zs(n), e.__queueingCheckRun = !0, o({
                         url: rn.Url("/checks/".concat(e.name, "/run?args=").concat(s), t),
                         onData: function(t) {
                             return e.__queueingCheckRun = !1, e.__queuedCheckRun = t.uuid, setTimeout((function() {
                                 ! function(e) {
                                     e.__resultHistory && e.__resultHistory.refresh()
-                                }(e), As(n)
+                                }(e), zs(n)
                             }), 4e3), t.uuid
                         }
                     }), e.__queuedCheckRun = null,
                     function(e, t) {
-                        e.showingCheckRunningBox = !0, As(t)
-                    }(e, n), Qs(e, 0, r)
+                        e.showingCheckRunningBox = !0, zs(t)
+                    }(e, n), Gs(e, 0, r)
             }
 
-            function Ws(e, t, n, r, o) {
+            function Hs(e, t, n, r, o) {
                 var i, a = {
                         check_name: e.name,
                         called_by: null === (i = e.__result) || void 0 === i ? void 0 : i.get("uuid")
                     },
                     s = no.Str(a),
                     u = btoa(s);
-                Vs(e, r), As(r), e.__queueingActionRun = !0, o({
+                Zs(e, r), zs(r), e.__queueingActionRun = !0, o({
                         url: rn.Url("/action/".concat(t, "/run?args=").concat(u), n),
                         onData: function(t) {
                             return e.__queueingActionRun = !1, e.__queuedActionRun = t.uuid, t.uuid
                         }
                     }), e.__queuedActionRun = null,
                     function(e, t) {
-                        e.__showingActionRunningBox = !0, As(t)
+                        e.__showingActionRunningBox = !0, zs(t)
                     }(e, r)
             }
 
-            function Hs(e, t) {
-                e.showingCheckRunningBox = !1, As(t)
+            function Vs(e, t) {
+                e.showingCheckRunningBox = !1, zs(t)
             }
 
-            function Vs(e, t) {
-                e.__showingActionRunningBox = !1, As(t)
+            function Zs(e, t) {
+                e.__showingActionRunningBox = !1, zs(t)
             }
-            var Zs = function(e) {
+            var qs = function(e) {
                     var t = e.groupList,
                         n = e.env,
                         r = e.historyList,
                         o = e.info,
                         i = e.toggleShowingChecksSearch;
                     return t.error ? (0, wo.jsx)(ua, {
                         error: t.error,
@@ -50678,45 +50681,45 @@
                                     id: "tooltip-search",
                                     position: "right",
                                     shape: "squared",
                                     size: "small",
                                     text: "Click to search for checks."
                                 })]
                             }), t.map((function(e, i) {
-                                return (0, wo.jsx)(qs, {
+                                return (0, wo.jsx)(Js, {
                                     group: e,
                                     env: n,
                                     groupList: t,
                                     historyList: r,
                                     info: o,
                                     style: {
                                         paddingBottom: "6pt"
                                     }
                                 }, e.group)
                             }))]
                         }) : (0, wo.jsx)(wo.Fragment, {})
                     })
                 },
-                qs = function(e) {
+                Js = function(e) {
                     var t, n = e.group,
                         r = e.groupList,
                         o = e.historyList,
                         i = e.env,
                         a = e.info,
                         s = e.style,
                         u = void 0 === s ? {} : s;
 
                     function l(e, t) {
                         c(e) ? function(e, t) {
                             e.map((function(e) {
-                                return e.__showingResults && zs(e, t)
+                                return e.__showingResults && Os(e, t)
                             }))
                         }(e, t) : function(e, t, n) {
                             e.map((function(e) {
-                                return !e.__showingResults && Os(e, 0, n)
+                                return !e.__showingResults && _s(e, 0, n)
                             }))
                         }(e, 0, t)
                     }
 
                     function c(e) {
                         for (var t = 0; t < (null === e || void 0 === e ? void 0 : e.length); t++)
                             if (e[t].__showingResults) return !0;
@@ -50750,15 +50753,15 @@
                                     })]
                                 }), (0, wo.jsx)("span", {
                                     style: {
                                         float: "right",
                                         cursor: "pointer"
                                     },
                                     onClick: function() {
-                                        Us(n, r, o)
+                                        Ps(n, r, o)
                                     },
                                     children: (0, wo.jsx)("b", {
                                         children: po.X
                                     })
                                 })]
                             }), (0, wo.jsx)("div", {
                                 style: {
@@ -50768,27 +50771,27 @@
                                 return e.title > t.title ? 1 : e.title < t.title ? -1 : 0
                             })).map((function(e, t) {
                                 return (0, wo.jsxs)("div", {
                                     children: [t > 0 && (0, wo.jsx)("div", {
                                         style: {
                                             marginBottom: "12px"
                                         }
-                                    }), (0, wo.jsx)(Js, {
+                                    }), (0, wo.jsx)(Ks, {
                                         check: e,
                                         env: i,
                                         groupList: r,
                                         historyList: o,
                                         info: a
                                     })]
                                 }, t)
                             }))]
                         })
                     })
                 },
-                Js = function(e) {
+                Ks = function(e) {
                     var n, r = e.check,
                         o = e.env,
                         i = e.groupList,
                         a = e.historyList,
                         s = e.info,
                         u = (0, t.useState)(!1);
 
@@ -50858,19 +50861,19 @@
                                             style: {
                                                 verticalAlign: "top",
                                                 width: "1%",
                                                 cursor: "pointer"
                                             },
                                             onClick: function() {
                                                 ! function(e, t, n) {
-                                                    e.__showingResults ? zs(e, n) : (Os(e, 0, n), f(!0))
+                                                    e.__showingResults ? Os(e, n) : (_s(e, 0, n), f(!0))
                                                 }(r, 0, i)
                                             },
                                             children: (0, wo.jsxs)("b", {
-                                                children: [Rs(r) ? (0, wo.jsx)("small", {
+                                                children: [Fs(r) ? (0, wo.jsx)("small", {
                                                     children: po.DownArrowHollow
                                                 }) : (0, wo.jsx)("small", {
                                                     children: po.RightArrowHollow
                                                 }), "\xa0"]
                                             })
                                         }), (0, wo.jsxs)("td", {
                                             style: {
@@ -50885,15 +50888,15 @@
                                                         id: "tooltip-configure ".concat(r.name),
                                                         className: r.__configuringCheckRun ? "check-config-button" : "check-run-button",
                                                         style: {
                                                             marginTop: "-2pt",
                                                             float: "right"
                                                         },
                                                         onClick: function() {
-                                                            r.__configuringCheckRun ? (Fs(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, As(i), f(!0)
+                                                            r.__configuringCheckRun ? (Bs(r), r.__configuringCheckRun = !1) : r.__configuringCheckRun = !0, zs(i), f(!0)
                                                         },
                                                         children: [(0, wo.jsx)("span", {
                                                             style: {
                                                                 fontSize: "small"
                                                             }
                                                         }), "\xa0Run ..."]
                                                     }), (0, wo.jsx)(oa, {
@@ -50904,15 +50907,15 @@
                                                 })
                                             }) : (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("div", {
                                                     style: {
                                                         marginLeft: "10pt",
                                                         float: "right"
                                                     },
-                                                    children: (0, wo.jsx)(eu, {
+                                                    children: (0, wo.jsx)(tu, {
                                                         check: r,
                                                         env: o,
                                                         groupList: i,
                                                         historyList: a,
                                                         style: {
                                                             marginTop: "-1pt"
                                                         }
@@ -50922,19 +50925,19 @@
                                                 style: {
                                                     whiteSpace: "nowrap"
                                                 },
                                                 children: [(0, wo.jsx)("u", {
                                                     id: "tooltip-check-info ".concat(r.name),
                                                     style: {
                                                         cursor: "pointer",
-                                                        fontWeight: Rs(r) ? "bold" : "normal",
+                                                        fontWeight: Fs(r) ? "bold" : "normal",
                                                         whiteSpace: "break-spaces"
                                                     },
                                                     onClick: function() {
-                                                        Ys(r, o, a)
+                                                        Qs(r, o, a)
                                                     },
                                                     children: (null === (n = r.title) || void 0 === n ? void 0 : n.length) > 70 ? r.title.substring(0, 69) + " ..." : r.title
                                                 }), (0, wo.jsx)(oa, {
                                                     id: "tooltip-check-info ".concat(r.name),
                                                     text: "Check: ".concat(r.name, ". Module: ").concat(r.module, ".")
                                                 }), r.__result.get("action") && (0, wo.jsx)("u", {
                                                     children: u[0] ? (0, wo.jsxs)(wo.Fragment, {
@@ -50992,15 +50995,15 @@
                                                             height: "18"
                                                         })
                                                     }), (0, wo.jsx)(oa, {
                                                         id: "tooltip-view-source ".concat(r.name),
                                                         text: "Click to view source code for this check (in new tab)."
                                                     })]
                                                 })]
-                                            }), (0, wo.jsx)(Ks, {
+                                            }), (0, wo.jsx)(Xs, {
                                                 check: r,
                                                 env: o,
                                                 historyList: a
                                             }), Object.keys(null === r || void 0 === r ? void 0 : r.schedule).map((function(e, t) {
                                                 var n, o;
                                                 return (0, wo.jsx)("div", {
                                                     children: wt.HasValue(null === (n = r.schedule[e]) || void 0 === n ? void 0 : n.cron_description) ? (0, wo.jsxs)("div", {
@@ -51022,42 +51025,42 @@
                                                         })]
                                                     }, t) : (0, wo.jsx)("small", {
                                                         children: (0, wo.jsx)("i", {
                                                             children: "Not scheduled."
                                                         })
                                                     })
                                                 }, e)
-                                            })), (0, wo.jsx)(tu, {
+                                            })), (0, wo.jsx)(nu, {
                                                 check: r,
                                                 env: o,
                                                 groupList: i,
                                                 historyList: a,
                                                 update: function() {
-                                                    return As(i)
+                                                    return zs(i)
                                                 },
                                                 showDependenciesBox: p,
                                                 setShowDependenciesBox: f
-                                            }), (0, wo.jsx)(nu, {
+                                            }), (0, wo.jsx)(ru, {
                                                 check: r,
                                                 groupList: i,
                                                 info: s
-                                            }), (0, wo.jsx)(uu, {
+                                            }), (0, wo.jsx)(lu, {
                                                 check: r,
                                                 env: o,
                                                 groupList: i,
                                                 update: function() {
                                                     return i.update()
                                                 },
                                                 fetchResult: c,
                                                 runActionAllowedState: u
-                                            }), (0, wo.jsx)(ru, {
+                                            }), (0, wo.jsx)(ou, {
                                                 check: r,
                                                 groupList: i,
                                                 info: s
-                                            }), (0, wo.jsx)(Xs, {
+                                            }), (0, wo.jsx)($s, {
                                                 check: r,
                                                 env: o,
                                                 groupList: i,
                                                 fetchResult: c,
                                                 runActionAllowedState: u
                                             })]
                                         })]
@@ -51068,25 +51071,25 @@
                                         children: (0, wo.jsx)("td", {})
                                     })]
                                 })
                             })
                         })
                     })
                 },
-                Ks = function(e) {
+                Xs = function(e) {
                     var t = e.check,
                         n = e.env,
                         r = e.historyList,
                         o = e.style;
                     return (0, wo.jsxs)("span", {
                         style: nt(nt({}, o), {}, {
                             cursor: "pointer"
                         }),
                         onClick: function() {
-                            return Ys(t, n, r)
+                            return Qs(t, n, r)
                         },
                         children: [(0, wo.jsx)("span", {
                             id: "tooltip-recent-history ".concat(t.name),
                             children: (0, wo.jsx)("img", {
                                 alt: "history",
                                 onClick: function(e) {},
                                 src: on.History(),
@@ -51100,15 +51103,15 @@
                             id: "tooltip-recent-history ".concat(t.name),
                             text: "Click to " + (t.__showingHistory ? "hide" : "show") + " recent history of check runs."
                         }), t.__showingHistory ? (0, wo.jsx)("span", {
                             children: po.RightArrow
                         }) : (0, wo.jsx)(wo.Fragment, {})]
                     })
                 },
-                Xs = function(e) {
+                $s = function(e) {
                     var n, r, o, i = e.check,
                         a = e.env,
                         s = e.groupList,
                         u = e.fetchResult,
                         c = (e.runActionAllowedState, l((0, t.useState)(!1), 2)),
                         d = c[0],
                         p = c[1],
@@ -51125,15 +51128,15 @@
                     }
 
                     function v(e, t) {
                         p(!1), g(!0)
                     }
 
                     function M(e, t) {
-                        e.__showingResultDetails = !e.__showingResultDetails, Ts(t)
+                        e.__showingResultDetails = !e.__showingResultDetails, As(t)
                     }
                     var j = function(e) {
                         var t, n = e.check,
                             r = e.env,
                             o = (e.checkUuid, e.groupList);
                         return t = d ? n.__resultByUuid.loading ? "Fetching latest result: ".concat(n.__result.get("uuid")) : "Click to fetch latest result: ".concat(n.__result.get("uuid")) : n.__result.loading ? "Fetching latest result." : "Click to fetch latest result.", (0, wo.jsxs)("span", {
                             style: {
@@ -51217,15 +51220,15 @@
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
                                         children: i.__result.get("timestamp")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result ".concat(i.name),
                                         text: "Click to " + (i.__showingResultDetails ? "hide" : "show") + " latest result."
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
-                                        text: Cs.Format(i.__result.get("timestamp"), new Date, !0, null, null, "ago")
+                                        text: Es.Format(i.__result.get("timestamp"), ks.Now(), !0, null, null, "ago")
                                     })]
                                 }), i.__showingResultDetails && (0, wo.jsx)(wo.Fragment, {
                                     children: i.__result.get("uuid") ? (0, wo.jsx)(wo.Fragment, {
                                         children: d ? (0, wo.jsx)(wo.Fragment, {
                                             children: i.__result.get("action") ? (0, wo.jsxs)(wo.Fragment, {
                                                 children: ["\xa0|\xa0", (0, wo.jsx)("span", {
                                                     id: "tooltip-view-latest-result-summary ".concat(i.name),
@@ -51440,24 +51443,24 @@
                                 })]
                             })
                         }), i.__showingResultDetails && (!i.__result.empty || !i.__resultByUuid.empty || !i.__resultByAction.empty) && (0, wo.jsxs)(wo.Fragment, {
                             children: [(0, wo.jsx)("div", {
                                 style: {
                                     height: "2pt"
                                 }
-                            }), (0, wo.jsx)($s, {
+                            }), (0, wo.jsx)(eu, {
                                 check: i,
                                 groupList: s,
                                 showResultByUuid: d,
                                 showResultByAction: h
                             })]
                         })]
                     })
                 },
-                $s = function(e) {
+                eu = function(e) {
                     var t, n = e.check,
                         r = e.groupList,
                         o = e.showResultByUuid,
                         i = e.showResultByAction;
                     e.style;
                     return n.__showingResults ? o ? (0, wo.jsxs)("pre", {
                         className: "box lighten",
@@ -51498,15 +51501,15 @@
                             }), "\xa0", (0, wo.jsx)("span", {
                                 style: {
                                     fontSize: "large",
                                     cursor: "pointer",
                                     color: "black"
                                 },
                                 onClick: function() {
-                                    n.__showingResultDetails = !1, Ts(r)
+                                    n.__showingResultDetails = !1, As(r)
                                 },
                                 children: "X"
                             })]
                         }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsx)(Lo, {
                                 condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                                 color: ln.GetForegroundColor(),
@@ -51554,15 +51557,15 @@
                             }), "\xa0", (0, wo.jsx)("span", {
                                 style: {
                                     fontSize: "large",
                                     cursor: "pointer",
                                     color: "black"
                                 },
                                 onClick: function() {
-                                    n.__showingResultDetails = !1, Ts(r)
+                                    n.__showingResultDetails = !1, As(r)
                                 },
                                 children: "X"
                             })]
                         }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsx)(Lo, {
                                 condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                                 color: ln.GetForegroundColor(),
@@ -51611,30 +51614,30 @@
                             }), "\xa0", (0, wo.jsx)("span", {
                                 style: {
                                     fontSize: "x-large",
                                     cursor: "pointer",
                                     color: "black"
                                 },
                                 onClick: function() {
-                                    n.showingResultDetailsFull = !n.showingResultDetailsFull, Ts(r)
+                                    n.showingResultDetailsFull = !n.showingResultDetailsFull, As(r)
                                 },
                                 children: n.showingResultDetailsFull ? (0, wo.jsx)("span", {
                                     title: "Show full result output.",
                                     children: po.UpArrow
                                 }) : (0, wo.jsx)("span", {
                                     children: po.DownArrow
                                 })
                             }), "\xa0", (0, wo.jsx)("span", {
                                 style: {
                                     fontSize: "large",
                                     cursor: "pointer",
                                     color: "black"
                                 },
                                 onClick: function() {
-                                    n.__showingResultDetails = !1, Ts(r)
+                                    n.__showingResultDetails = !1, As(r)
                                 },
                                 children: "X"
                             })]
                         }), n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading ? (0, wo.jsx)(Lo, {
                             condition: n.__result.loading || n.__resultByUuid.loading || n.__resultByAction.loading,
                             color: ln.GetForegroundColor(),
                             label: "Loading latest result "
@@ -51642,15 +51645,15 @@
                             style: {
                                 marginTop: "1pt"
                             },
                             children: "No result."
                         }) : Ia.Format(n.showingResultDetailsFull ? n.__result.get("full_output") : n.__result.get())]
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                eu = function(e) {
+                tu = function(e) {
                     var t = e.check,
                         n = e.env,
                         r = e.groupList,
                         o = e.historyList,
                         i = e.style,
                         a = l(ws(), 1)[0],
                         s = hs();
@@ -51678,15 +51681,15 @@
                             className: "check-run-button" + (t.__configuringCheckRun, ""),
                             style: nt(nt({}, i), {}, {
                                 cursor: a && t.__configuringCheckRun ? "not-allowed" : "",
                                 background: a && t.__configuringCheckRun ? "#888888" : "",
                                 color: t.__configuringCheckRun ? "yellow" : ""
                             }),
                             onClick: function(e) {
-                                t.__configuringCheckRun ? a || (Fs(t), Gs(t, n, r, o, s)) : (t.__configuringCheckRun = !0, As(r))
+                                t.__configuringCheckRun ? a || (Bs(t), Ws(t, n, r, o, s)) : (t.__configuringCheckRun = !0, zs(r))
                             },
                             children: (0, wo.jsx)("span", {
                                 children: a ? (0, wo.jsx)(wo.Fragment, {
                                     children: t.__configuringCheckRun ? (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsxs)("span", {
                                             style: {
                                                 fontSize: "",
@@ -51723,15 +51726,15 @@
                                         })
                                     })
                                 })
                             })
                         })]
                     })
                 },
-                tu = function(e) {
+                nu = function(e) {
                     var n = e.check,
                         r = e.env,
                         o = e.groupList,
                         i = e.historyList,
                         a = (e.update, e.showDependenciesBox),
                         s = e.setShowDependenciesBox;
 
@@ -51828,15 +51831,15 @@
                             },
                             children: Dt.IsNonEmptyObject(n.kwargs) ? (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("div", {
                                     style: {
                                         marginTop: "-2pt",
                                         float: "right"
                                     },
-                                    children: (0, wo.jsx)(eu, {
+                                    children: (0, wo.jsx)(tu, {
                                         check: n,
                                         env: r,
                                         groupList: o,
                                         historyList: i,
                                         style: {
                                             float: "right"
                                         }
@@ -51867,15 +51870,15 @@
                                                         defaultValue: n.kwargs[e] ? "true" : "false",
                                                         style: {
                                                             background: "lightyellow",
                                                             border: "1px solid lightgray",
                                                             borderRadius: "4pt"
                                                         },
                                                         onChange: function(t) {
-                                                            n.kwargs[e] = "true" === t.target.value, As(o)
+                                                            n.kwargs[e] = "true" === t.target.value, zs(o)
                                                         },
                                                         children: (n.kwargs[e], (0, wo.jsxs)(wo.Fragment, {
                                                             children: [(0, wo.jsx)("option", {
                                                                 children: "true"
                                                             }), (0, wo.jsx)("option", {
                                                                 children: "false"
                                                             })]
@@ -51883,28 +51886,28 @@
                                                     }), Dt.IsNonEmptyArray(n.kwargs[e]) && (0, wo.jsx)("select", {
                                                         defaultValue: null === (t = n.kwargs[e]) || void 0 === t ? void 0 : t.__selected,
                                                         style: {
                                                             background: "lightyellow",
                                                             border: "1px solid lightgray"
                                                         },
                                                         onChange: function(t) {
-                                                            n.kwargs[e].__selected = t.target.value, As(o)
+                                                            n.kwargs[e].__selected = t.target.value, zs(o)
                                                         },
                                                         children: n.kwargs[e].map((function(e) {
                                                             return (0, wo.jsx)("option", {
                                                                 children: e
                                                             }, Jr()())
                                                         }))
                                                     }, Jr()()), !Dt.IsBoolean(n.kwargs[e]) && !Dt.IsNonEmptyArray(n.kwargs[e]) && (0, wo.jsx)(wo.Fragment, {
                                                         children: (0, wo.jsx)("input", {
                                                             id: "".concat(n.name, ".").concat(e),
                                                             defaultValue: n.kwargs[e],
                                                             placeholder: "Empty",
                                                             onBlur: function() {
-                                                                Fs(n)
+                                                                Bs(n)
                                                             },
                                                             style: {
                                                                 marginLeft: "0pt",
                                                                 height: "14pt",
                                                                 background: "lightyellow",
                                                                 border: "1px solid lightgray",
                                                                 borderRadius: "2pt"
@@ -51918,29 +51921,29 @@
                                 })]
                             }) : (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("div", {
                                     style: {
                                         marginTop: "-3pt",
                                         float: "right"
                                     },
-                                    children: (0, wo.jsx)(eu, {
+                                    children: (0, wo.jsx)(tu, {
                                         check: n,
                                         env: r,
                                         groupList: o,
                                         historyList: i,
                                         style: {
                                             float: "right"
                                         }
                                     })
                                 }), "No arguments."]
                             })
                         })]
                     })
                 },
-                nu = function(e) {
+                ru = function(e) {
                     var n = e.check,
                         r = e.groupList,
                         o = e.info,
                         i = l((0, t.useState)(!1), 2),
                         a = i[0],
                         s = i[1];
                     return n.showingCheckRunningBox && n.__configuringCheckRun ? (0, wo.jsx)("div", {
@@ -51969,15 +51972,15 @@
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: Ss.Format(n.__queuedCheckRun + "+00:00")
+                                        children: ks.Format(n.__queuedCheckRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
@@ -52018,15 +52021,15 @@
                                     }), (0, wo.jsxs)("div", {
                                         style: {
                                             float: "right",
                                             marginTop: "-0pt",
                                             cursor: "pointer"
                                         },
                                         onClick: function() {
-                                            Hs(n, r)
+                                            Vs(n, r)
                                         },
                                         children: ["\xa0", (0, wo.jsx)("b", {
                                             children: po.X
                                         }), "\xa0"]
                                     })]
                                 })
                             }), !n.__queuedCheckRun && (0, wo.jsx)("div", {
@@ -52038,15 +52041,15 @@
                                     label: " Queueing check run",
                                     color: "darkred"
                                 })
                             })]
                         })
                     }) : (0, wo.jsx)("span", {})
                 },
-                ru = function(e) {
+                ou = function(e) {
                     var n = e.check,
                         r = e.groupList,
                         o = e.info,
                         i = l((0, t.useState)(!1), 2),
                         a = i[0],
                         s = i[1];
                     return n.__showingActionRunningBox && n.__configuringCheckRun ? (0, wo.jsx)("div", {
@@ -52076,15 +52079,15 @@
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: Ss.Format(n.__queuedActionRun + "+00:00")
+                                        children: ks.Format(n.__queuedActionRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
@@ -52125,15 +52128,15 @@
                                     }), (0, wo.jsxs)("div", {
                                         style: {
                                             float: "right",
                                             marginTop: "-0pt",
                                             cursor: "pointer"
                                         },
                                         onClick: function() {
-                                            Vs(n, r)
+                                            Zs(n, r)
                                         },
                                         children: ["\xa0", po.X]
                                     })]
                                 })
                             }), !n.__queuedActionRun && (0, wo.jsx)("div", {
                                 style: {
                                     marginTop: "-2pt"
@@ -52143,15 +52146,15 @@
                                     label: " Queueing action run",
                                     color: "darkred"
                                 })
                             })]
                         })
                     }) : (0, wo.jsx)("span", {})
                 },
-                ou = function(e) {
+                iu = function(e) {
                     var t = e.env,
                         n = e.historyList;
                     if (n.error) return (0, wo.jsx)(ua, {
                         error: n.error,
                         message: "Error loading check history from Foursight API"
                     });
                     var r = n.filter((function(e) {
@@ -52164,24 +52167,24 @@
                             },
                             children: "Recent Results"
                         }), null === r || void 0 === r ? void 0 : r.map((function(e, r) {
                             return (0, wo.jsx)("div", {
                                 style: {
                                     marginTop: "3pt"
                                 },
-                                children: (0, wo.jsx)(iu, {
+                                children: (0, wo.jsx)(au, {
                                     check: e,
                                     env: t,
                                     historyList: n
                                 })
                             }, e.name)
                         }))]
                     })
                 },
-                iu = function(e) {
+                au = function(e) {
                     var n, r, o, i = e.check,
                         a = (e.env, e.historyList);
 
                     function s(e, t) {
                         e.__resultShowing = !1, e.__result = null, e.__resultLoading = !1, t.update()
                     }
 
@@ -52317,15 +52320,15 @@
                                 })]
                             }), (0, wo.jsxs)("span", {
                                 style: {
                                     float: "right",
                                     cursor: "pointer"
                                 },
                                 onClick: function() {
-                                    Bs(i, a)
+                                    Ys(i, a)
                                 },
                                 children: ["\xa0\xa0", (0, wo.jsx)("b", {
                                     children: po.X
                                 })]
                             })]
                         }), (0, wo.jsx)("div", {
                             style: {
@@ -52416,15 +52419,15 @@
                                                                 children: (0, wo.jsx)("b", {
                                                                     style: {
                                                                         color: "inherit"
                                                                     },
                                                                     children: "OK"
                                                                 })
                                                             }) : (0, wo.jsx)(wo.Fragment, {
-                                                                children: (0, wo.jsx)(ks, {
+                                                                children: (0, wo.jsx)(Cs, {
                                                                     status: c(e)
                                                                 })
                                                             }), "\xa0\xa0"]
                                                         }), (0, wo.jsxs)("td", {
                                                             style: {
                                                                 textAlign: "right"
                                                             },
@@ -52550,15 +52553,15 @@
                                         })
                                     })
                                 })
                             })
                         })]
                     })
                 },
-                au = function(e) {
+                su = function(e) {
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: ["\xa0", (0, wo.jsxs)("span", {
                             style: {
                                 fontWeight: e.showingChecksSearch ? "bold" : "normal"
                             },
                             onClick: e.toggleShowingChecksSearch,
                             children: [(0, wo.jsx)("span", {
@@ -52576,15 +52579,15 @@
                                 },
                                 src: on.NewIcon(),
                                 height: "42"
                             })]
                         }), " ", (0, wo.jsx)("br", {})]
                     })
                 },
-                su = function(e) {
+                uu = function(e) {
                     var n = l((0, t.useState)(""), 2),
                         r = n[0],
                         o = n[1],
                         i = l((0, t.useState)([]), 2),
                         a = i[0],
                         s = i[1];
 
@@ -52831,15 +52834,15 @@
                                         children: "No results."
                                     })
                                 })]
                             })
                         })]
                     })
                 },
-                uu = function(e) {
+                lu = function(e) {
                     var n, r = e.check,
                         o = e.env,
                         i = e.groupList,
                         a = e.fetchResult,
                         s = e.runActionAllowedState,
                         u = l((0, t.useState)(!1), 2),
                         c = u[0],
@@ -52848,15 +52851,15 @@
                         f = hs();
 
                     function h() {
                         if (c) {
                             var e;
                             d(!1);
                             var t = null === (e = r.__result) || void 0 === e ? void 0 : e.get("action");
-                            t && (Ws(r, t, o, i, f), s[1](!1))
+                            t && (Hs(r, t, o, i, f), s[1](!1))
                         } else d(!0)
                     }
                     return (0, t.useEffect)((function() {
                         d(!1)
                     }), []), (0, wo.jsx)(wo.Fragment, {
                         children: r.__configuringCheckRun && (null === (n = r.__result) || void 0 === n ? void 0 : n.get("action")) && (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsxs)("div", {
@@ -53015,15 +53018,15 @@
                                         position: "top"
                                     })]
                                 })]
                             })
                         })
                     })
                 },
-                lu = function(e) {
+                cu = function(e) {
                     var n = je().environ,
                         r = Ua({
                             initial: []
                         }),
                         o = Ua({
                             initial: []
                         }),
@@ -53034,15 +53037,15 @@
                     var c = Ua({
                             url: rn.Url("/checks/grouped/schedule", n),
                             nofetch: !0,
                             cache: !0,
                             onData: function(e) {
                                 return e.sort((function(e, t) {
                                     return e.group > t.group ? 1 : e.group < t.group ? -1 : 0
-                                })), e.length > 0 && _s(function(e) {
+                                })), e.length > 0 && Us(function(e) {
                                     for (var t = null, n = 0; n < (null === e || void 0 === e ? void 0 : e.length); n++) {
                                         var r, o;
                                         (!t || (null === (r = e[n]) || void 0 === r || null === (o = r.checks) || void 0 === o ? void 0 : o.length) < t.checks.length) && (t = e[n])
                                     }
                                     return t
                                 }(e), 0, o), e
                             }
@@ -53062,15 +53065,15 @@
                     var p = Ua();
 
                     function f() {
                         p.refresh(rn.Url("/checks_status", n))
                     }
 
                     function h(e, t, n, r) {
-                        Ps(e, n) ? Us(e, n, r) : _s(e, 0, n)
+                        Rs(e, n) ? Ps(e, n, r) : Us(e, 0, n)
                     }
 
                     function g() {
                         u(!s), o.update([])
                     }
                     var y = function(e) {
                             e.props;
@@ -53187,15 +53190,15 @@
                                     },
                                     children: c.map((function(e, t) {
                                         var n;
                                         return (0, wo.jsxs)("div", {
                                             children: [(0, wo.jsxs)("span", {
                                                 id: "tooltip-group-count-".concat(t),
                                                 style: {
-                                                    fontWeight: Ps(e, o) ? "bold" : "normal",
+                                                    fontWeight: Rs(e, o) ? "bold" : "normal",
                                                     cursor: "pointer"
                                                 },
                                                 onClick: function() {
                                                     return h(e, 0, o, r)
                                                 },
                                                 children: [e.group.replace(/ checks$/i, ""), " \xa0", (0, wo.jsxs)("small", {
                                                     children: ["(", e.checks.length, ")"]
@@ -53425,15 +53428,15 @@
                                                 children: [(0, wo.jsx)("b", {
                                                     children: "Most Recent"
                                                 }), ":\xa0"]
                                             }) : (0, wo.jsxs)(wo.Fragment, {
                                                 children: [(0, wo.jsx)("b", {
                                                     children: "Top"
                                                 }), ":\xa0"]
-                                            }), (0, wo.jsx)(Cs.Live, {
+                                            }), (0, wo.jsx)(Es.Live, {
                                                 start: null === C || void 0 === C || null === (u = C.data[0]) || void 0 === u ? void 0 : u.timestamp,
                                                 verbose: !0,
                                                 fallback: "just now",
                                                 suffix: "ago",
                                                 tooltip: !0
                                             })]
                                         }), (0, wo.jsx)("b", {
@@ -53530,30 +53533,30 @@
                                                                     children: po.X
                                                                 }), "\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 id: "recent-runs-timestamp ".concat(i),
                                                                 style: {
                                                                     width: "20%"
                                                                 },
-                                                                children: [Date.Format(e.timestamp), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                                                children: [Ns.Format(e.timestamp), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                                     children: uo.Format(e.timestamp)
                                                                 }), (0, wo.jsx)(oa, {
                                                                     id: "recent-runs-timestamp ".concat(i),
-                                                                    text: Cs.Format(e.timestamp, new Date, !0, null, null, "agoy")
+                                                                    text: Es.Format(e.timestamp, ks.Now(), !0, null, null, "agoy")
                                                                 }), "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     width: "45%"
                                                                 },
                                                                 children: [(0, wo.jsx)("b", {
                                                                     style: {
                                                                         cursor: "pointer"
                                                                     },
                                                                     onClick: function() {
-                                                                        return Ys(P(e.check, e.group), n, r)
+                                                                        return Qs(P(e.check, e.group), n, r)
                                                                     },
                                                                     children: e.title
                                                                 }), "\xa0\xa0", (0, wo.jsxs)(qe, {
                                                                     to: $r.Path("/checks/".concat(e.check, "/history")),
                                                                     rel: "noreferrer",
                                                                     target: "_blank",
                                                                     children: [(0, wo.jsx)("small", {
@@ -53580,15 +53583,15 @@
                                                                         children: e.group
                                                                     })
                                                                 }), "\xa0 \xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     width: "10%"
                                                                 },
-                                                                children: ["\xa0", (0, wo.jsx)(ks, {
+                                                                children: ["\xa0", (0, wo.jsx)(Cs, {
                                                                     status: e.status
                                                                 }), "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 align: "right",
                                                                 style: {
                                                                     width: "10%"
                                                                 },
@@ -53911,15 +53914,15 @@
                                                 children: [(0, wo.jsx)("td", {
                                                     style: c,
                                                     children: "Updated:"
                                                 }), (0, wo.jsx)("td", {
                                                     style: l,
                                                     children: (0, wo.jsx)("span", {
                                                         id: "tooltip-lambda-updated-".concat(u.lambda_name),
-                                                        children: Ss.Format(u.lambda_modified)
+                                                        children: ks.Format(u.lambda_modified)
                                                     })
                                                 }), (0, wo.jsx)(oa, {
                                                     id: "tooltip-lambda-updated-".concat(u.lambda_name),
                                                     text: uo.Ago(u.lambda_modified),
                                                     position: "right",
                                                     shape: "squared"
                                                 })]
@@ -54007,15 +54010,15 @@
                                                                                 children: [(0, wo.jsx)("b", {
                                                                                     id: "tooltip-lambda-check-".concat(e.check_name),
                                                                                     style: {
                                                                                         color: ln.GetForegroundColor(),
                                                                                         cursor: "pointer"
                                                                                     },
                                                                                     onClick: function() {
-                                                                                        return Ys(P(e.check_name, e.check_group), n, r)
+                                                                                        return Qs(P(e.check_name, e.check_group), n, r)
                                                                                     },
                                                                                     children: e.check_title
                                                                                 }), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("i", {
                                                                                     id: "tooltip-lambda-check-group-".concat(e.check_name),
                                                                                     style: {
                                                                                         color: ln.GetForegroundColor(),
                                                                                         cursor: "pointer"
@@ -54098,58 +54101,58 @@
                                                 }), (0, wo.jsx)(N, {}), (0, wo.jsx)("div", {
                                                     style: {
                                                         marginTop: "3pt",
                                                         marginBottom: "3pt",
                                                         height: "1px",
                                                         backgroundColor: "var(--box-fg)"
                                                     }
-                                                }), (0, wo.jsx)(au, {
+                                                }), (0, wo.jsx)(su, {
                                                     showingChecksSearch: D,
                                                     toggleShowingChecksSearch: S
                                                 })]
                                             }), (0, wo.jsx)(B, {}), (0, wo.jsx)(H, {})]
                                         }), (0, wo.jsxs)("td", {
                                             style: {
                                                 paddingLeft: "8pt",
                                                 verticalAlign: "top"
                                             },
                                             children: [(0, wo.jsx)(k, {
                                                 info: i
-                                            }), (0, wo.jsx)(Zs, {
+                                            }), (0, wo.jsx)(qs, {
                                                 env: n,
                                                 groupList: o,
                                                 historyList: r,
                                                 info: i,
                                                 toggleShowingChecksSearch: S
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: {
                                                 paddingLeft: (null === o || void 0 === o ? void 0 : o.length) > 0 || o.error || b() ? "8pt" : "0",
                                                 verticalAlign: "top"
                                             },
-                                            children: [(0, wo.jsx)(su, {
+                                            children: [(0, wo.jsx)(uu, {
                                                 checks: c,
                                                 groupList: o,
                                                 environ: n,
                                                 findGroup: U,
                                                 toggleShowGroup: h,
                                                 showingChecksSearch: D,
                                                 toggleShowingChecksSearch: S
-                                            }), (0, wo.jsx)(V, {}), (0, wo.jsx)(F, {}), (0, wo.jsx)(ou, {
+                                            }), (0, wo.jsx)(V, {}), (0, wo.jsx)(F, {}), (0, wo.jsx)(iu, {
                                                 env: n,
                                                 historyList: r
                                             })]
                                         })]
                                     })
                                 })
                             })
                         })]
                     })
                 },
-                cu = function(e) {
+                du = function(e) {
                     var t;
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("b", {
                             children: "Check Groups"
                         }), (0, wo.jsx)("div", {
                             className: "box margin",
                             style: {
@@ -54175,15 +54178,15 @@
                                         })
                                     }), (0, wo.jsx)("br", {})]
                                 }, t.group)
                             }))
                         })]
                     })
                 },
-                du = function(e) {
+                pu = function(e) {
                     var n, r, o = l((0, t.useState)(!0), 2),
                         i = o[0],
                         a = o[1];
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsxs)("div", {
                             className: "pointer",
                             onClick: function() {
@@ -54204,15 +54207,15 @@
                             }))) || void 0 === r ? void 0 : r.map((function(t, n) {
                                 return (0, wo.jsxs)("div", {
                                     children: [(0, wo.jsx)("div", {
                                         className: "box margin",
                                         style: {
                                             maxWidth: "800pt"
                                         },
-                                        children: (0, wo.jsx)(pu, {
+                                        children: (0, wo.jsx)(fu, {
                                             group: t,
                                             update: e.update,
                                             showResult: i
                                         })
                                     }), (0, wo.jsx)("div", {
                                         style: {
                                             height: "6pt"
@@ -54224,15 +54227,15 @@
                             children: (0, wo.jsx)("div", {
                                 className: "box margin",
                                 children: "No check groups selected."
                             })
                         })]
                     })
                 },
-                pu = function(e) {
+                fu = function(e) {
                     var n, r, o = l((0, t.useState)(e.showResult), 2),
                         i = o[0],
                         a = o[1];
                     return (0, t.useEffect)((function() {
                         a(e.showResult)
                     }), [e.showResult]), (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("b", {
@@ -54240,29 +54243,29 @@
                             onClick: function() {
                                 a(!i)
                             },
                             children: e.group.group
                         }), null === (n = e.group) || void 0 === n || null === (r = n.checks) || void 0 === r ? void 0 : r.map((function(t, n) {
                             var r;
                             return (0, wo.jsxs)("div", {
-                                children: [(0, wo.jsx)(fu, {
+                                children: [(0, wo.jsx)(hu, {
                                     check: t,
                                     index: n,
                                     update: e.update,
                                     showResult: i
                                 }), n < (null === (r = e.group.checks) || void 0 === r ? void 0 : r.length) - 1 && (0, wo.jsx)("div", {
                                     style: {
                                         height: "6pt"
                                     }
                                 })]
                             }, t.name)
                         }))]
                     })
                 },
-                fu = function(e) {
+                hu = function(e) {
                     var n, r = l((0, t.useState)(e.showResult), 2),
                         o = r[0],
                         i = r[1];
 
                     function a() {
                         i(!o)
                     }
@@ -54318,27 +54321,27 @@
                                                         })
                                                     }, n) : (0, wo.jsx)("small", {
                                                         children: (0, wo.jsx)("i", {
                                                             children: "Not scheduled."
                                                         })
                                                     })
                                                 }, t)
-                                            })), (0, wo.jsx)(hu, {
+                                            })), (0, wo.jsx)(gu, {
                                                 check: e.check,
                                                 update: e.update,
                                                 showResult: o
                                             })]
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                hu = function(e) {
+                gu = function(e) {
                     var n, r = (n = e.check, Ua({
                             url: rn.Url("/checks/".concat(n.name)),
                             nofetch: !0,
                             cache: !0
                         })),
                         o = l((0, t.useState)(!1), 2),
                         i = o[0],
@@ -54398,15 +54401,15 @@
                                         children: ["Summary: ", r.get("summary") || r.get("description") || "No result summary."]
                                     })]
                                 })
                             })
                         })
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                gu = function(e) {
+                yu = function(e) {
                     var n = Ua(),
                         r = l((0, t.useState)([]), 2),
                         o = r[0],
                         i = r[1];
 
                     function a(e) {
                         return void 0 !== o.find((function(t) {
@@ -54441,15 +54444,15 @@
                                 children: (0, wo.jsx)("tbody", {
                                     children: (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
                                             style: {
                                                 paddingLeft: "10pt",
                                                 verticalAlign: "top"
                                             },
-                                            children: (0, wo.jsx)(cu, {
+                                            children: (0, wo.jsx)(du, {
                                                 groups: n,
                                                 selected: a,
                                                 toggle: function(e) {
                                                     a(e) ? function(e) {
                                                         var t = o.findIndex((function(t) {
                                                             return t.group === e.group
                                                         }));
@@ -54458,31 +54461,31 @@
                                                 }
                                             })
                                         }), (0, wo.jsx)("td", {
                                             style: {
                                                 paddingLeft: "10pt",
                                                 verticalAlign: "top"
                                             },
-                                            children: (0, wo.jsx)(du, {
+                                            children: (0, wo.jsx)(pu, {
                                                 groups: o,
                                                 selected: a,
                                                 update: function(e) {
                                                     u()
                                                 }
                                             })
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                yu = n(8145),
-                mu = n.n(yu),
-                vu = function(e) {
+                mu = n(8145),
+                vu = n.n(mu),
+                Mu = function(e) {
                     var t = e.pages,
                         n = e.page,
                         r = e.onChange,
                         o = e.refresh,
                         i = e.loading,
                         a = e.spinner;
                     return (0, wo.jsx)("table", {
@@ -54497,15 +54500,15 @@
                                             style: {
                                                 pointerEvents: i ? "none" : "",
                                                 opacity: i ? "0.4" : "",
                                                 fontSize: "8pt",
                                                 fontWeight: "bold"
                                             },
                                             className: "pagination-control",
-                                            children: (0, wo.jsx)(mu(), {
+                                            children: (0, wo.jsx)(vu(), {
                                                 nextLabel: "NEXT",
                                                 onPageChange: r,
                                                 pageRangeDisplayed: 2,
                                                 initialPage: n,
                                                 disableInitialCallback: !0,
                                                 marginPagesDisplayed: 2,
                                                 pageCount: t,
@@ -54560,23 +54563,23 @@
                                     })
                                 })]
                             })
                         })
                     })
                 };
 
-            function Mu(e) {
+            function ju(e) {
                 var t;
                 return null === e || void 0 === e || null === (t = e.split("/")) || void 0 === t ? void 0 : t.reverse()[0]
             }
 
-            function ju(e) {
+            function bu(e) {
                 return null === e || void 0 === e ? void 0 : e.substring(0, null === e || void 0 === e ? void 0 : e.lastIndexOf("/"))
             }
-            var bu = function(e) {
+            var wu = function(e) {
                     var t = e.check,
                         n = e.checkInfo;
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "box",
                             children: (0, wo.jsx)("table", {
                                 children: (0, wo.jsxs)("tbody", {
@@ -54691,16 +54694,16 @@
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsxs)("td", {
                                             children: [(0, wo.jsx)("b", {
                                                 children: "Code"
                                             }), ":"]
                                         }), (0, wo.jsxs)("td", {
-                                            children: [Mu(n.get("file")), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
-                                                children: ju(n.get("file"))
+                                            children: [ju(n.get("file")), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                                children: bu(n.get("file"))
                                             })]
                                         })]
                                     }), (0, wo.jsx)("tr", {
                                         children: (0, wo.jsx)("td", {
                                             style: {
                                                 paddingTop: "2px"
                                             }
@@ -54793,15 +54796,15 @@
                                         })]
                                     })]
                                 })
                             })
                         })
                     })
                 },
-                wu = function(e) {
+                xu = function(e) {
                     var n, r = e.check,
                         o = e.checkInfo;
 
                     function i(e) {
                         var t = e.get("schedule");
                         if (t) {
                             var n = Object.values(t);
@@ -55065,16 +55068,16 @@
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsxs)("td", {
                                             children: [(0, wo.jsx)("b", {
                                                 children: "Code"
                                             }), ":"]
                                         }), (0, wo.jsxs)("td", {
-                                            children: [Mu(o.get("registered_file")), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
-                                                children: ju(o.get("registered_file"))
+                                            children: [ju(o.get("registered_file")), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                                children: bu(o.get("registered_file"))
                                             })]
                                         })]
                                     }), (0, wo.jsx)("tr", {
                                         children: (0, wo.jsx)("td", {
                                             style: {
                                                 paddingTop: "3px"
                                             }
@@ -55281,16 +55284,16 @@
                                                 style: {
                                                     paddingRight: "8pt"
                                                 },
                                                 children: [(0, wo.jsx)("b", {
                                                     children: "Code"
                                                 }), ":"]
                                             }), (0, wo.jsxs)("td", {
-                                                children: [Mu(o.get("registered_action.file")), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
-                                                    children: ju(o.get("registered_action.file"))
+                                                children: [ju(o.get("registered_action.file")), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                                    children: bu(o.get("registered_action.file"))
                                                 })]
                                             })]
                                         }), (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "3px"
                                                 }
@@ -55390,15 +55393,15 @@
                                         })]
                                     })
                                 })
                             })]
                         })]
                     })
                 },
-                xu = function(e) {
+                Nu = function(e) {
                     var n, r = je(),
                         o = r.environ,
                         i = r.check,
                         a = l($e(), 2),
                         s = a[0],
                         u = a[1],
                         c = l((0, t.useState)(parseInt(s.get("limit")) || 25), 2),
@@ -55655,15 +55658,15 @@
                                                         children: [a(e), "\xa0\xa0"]
                                                     }), (0, wo.jsxs)("td", {
                                                         id: "tooltip-status-".concat(n),
                                                         style: {
                                                             verticalAlign: "top",
                                                             whiteSpace: "break-spaces"
                                                         },
-                                                        children: [(0, wo.jsx)(ks, {
+                                                        children: [(0, wo.jsx)(Cs, {
                                                             status: s(e)
                                                         }), (0, wo.jsx)(oa, {
                                                             id: "tooltip-status-".concat(n),
                                                             text: s(e),
                                                             position: "right",
                                                             shape: "squared",
                                                             offset: -12
@@ -55793,15 +55796,15 @@
                                             },
                                             children: (0, wo.jsx)("tbody", {
                                                 children: (0, wo.jsxs)("tr", {
                                                     children: [(0, wo.jsx)("td", {
                                                         style: {
                                                             width: "90%"
                                                         },
-                                                        children: (0, wo.jsx)(vu, {
+                                                        children: (0, wo.jsx)(Mu, {
                                                             pages: x,
                                                             onChange: function(e) {
                                                                 var t = e.selected * d % I.get("paging.total");
                                                                 L(d, t, m)
                                                             },
                                                             refresh: function() {
                                                                 return S(d, h, m)
@@ -55917,43 +55920,43 @@
                                         children: (0, wo.jsx)(T, {
                                             history: I
                                         })
                                     }), (0, wo.jsx)("td", {
                                         style: {
                                             verticalAlign: "top"
                                         },
-                                        children: "action" === D.get("type") ? (0, wo.jsx)(bu, {
+                                        children: "action" === D.get("type") ? (0, wo.jsx)(wu, {
                                             check: i,
                                             checkInfo: D
-                                        }) : (0, wo.jsx)(wu, {
+                                        }) : (0, wo.jsx)(xu, {
                                             check: i,
                                             checkInfo: D
                                         })
                                     })]
                                 })]
                             })
                         })
                     })
                 },
-                Nu = function() {
+                Iu = function() {
                     var e = l((0, t.useContext)(Ra), 2),
                         n = (e[0], e[1]),
                         r = Pa();
                     return function(e) {
                         return r.refresh(rn.Url("/header", e), {
                             onData: function(e) {
                                 return n(e)
                             },
                             cache: !0
                         })
                     }
                 },
-                Iu = function(e) {
+                Du = function(e) {
                     var t, n, r = Fa(),
-                        o = Nu(),
+                        o = Iu(),
                         i = Ua(co.IsLoggedIn() ? rn.Url("/info") : null);
                     wa.NoteLastUrl(r);
                     var a = Me();
 
                     function s() {
                         return tn.IsKnown(tn.Current(), r)
                     }
@@ -56288,15 +56291,15 @@
                                 style: {
                                     marginTop: "8pt"
                                 }
                             })]
                         })
                     })
                 },
-                Du = function(e) {
+                Lu = function(e) {
                     var t = Fa();
                     return t.loading ? null : (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("br", {}), (0, wo.jsx)("table", {
                             width: "100%",
                             children: (0, wo.jsxs)("tbody", {
                                 children: [(0, wo.jsx)("tr", {
                                     style: {
@@ -56329,15 +56332,15 @@
                                     },
                                     children: (0, wo.jsx)("td", {})
                                 })]
                             })
                         })]
                     })
                 },
-                Lu = function(e) {
+                Su = function(e) {
                     var t = Fa();
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "container",
                             id: "login_container",
                             children: (0, wo.jsxs)("div", {
                                 className: "boxstyle check-error",
@@ -56376,15 +56379,15 @@
                                         })
                                     }), " page."]
                                 })]
                             })
                         })
                     })
                 },
-                Su = function() {
+                ku = function() {
                     var e = l(ws(), 2),
                         t = e[0],
                         n = e[1];
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("img", {
                             id: "tooltip-readonly",
                             alt: "lock",
@@ -56399,61 +56402,61 @@
                         }), (0, wo.jsx)(oa, {
                             id: "tooltip-readonly",
                             position: "bottom",
                             text: "You are in ".concat(t ? "readonly" : "read/write", " mode. Click to enter ").concat(t ? "read/write" : "readonly", " mode.")
                         })]
                     })
                 },
-                ku = function(e) {
+                Cu = function(e) {
                     var t = e.header;
                     return (0, wo.jsxs)(wo.Fragment, {
-                        children: [(0, wo.jsx)(Cu, {
+                        children: [(0, wo.jsx)(Eu, {
                             header: t
-                        }), (0, wo.jsx)(Eu, {
+                        }), (0, wo.jsx)(Tu, {
                             header: t
                         })]
                     })
                 },
-                Cu = function() {
+                Eu = function() {
                     l($e(), 1)[0];
                     var e = Ua("/certificates");
                     if (e.loading) return (0, wo.jsx)(wo.Fragment, {});
                     var t = e.find((function(e) {
                         return "Portal" === e.name
                     }));
-                    return t && t.expires_soon ? (0, wo.jsxs)(Tu, {
+                    return t && t.expires_soon ? (0, wo.jsxs)(Au, {
                         children: [(0, wo.jsx)("b", {
                             children: "Warning: SSL certificate for associated Portal will expire soon"
                         }), "\xa0", po.RightArrow, "\xa0 ", t.expires_at, " \xa0", po.RightArrow, "\xa0", uo.FromNow(t.expires_at, !0, !1), "\xa0", po.RightArrow, "\xa0", (0, wo.jsx)(qe, {
                             to: $r.Path("/certificates"),
                             style: {
                                 color: "inherit"
                             },
                             children: "View"
                         })]
                     }) : void 0
                 },
-                Eu = function(e) {
+                Tu = function(e) {
                     e.header;
                     var t = Ua("/portal_access_key");
                     if (t.loading) return (0, wo.jsx)(wo.Fragment, {});
                     if (t) {
                         var n, r;
-                        if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, wo.jsxs)(Tu, {
+                        if (null !== t && void 0 !== t && null !== (n = t.data) && void 0 !== n && n.expires_soon) return (0, wo.jsxs)(Au, {
                             children: [(0, wo.jsx)("b", {
                                 children: "Warning: Access key for associated Portal will expire soon"
                             }), "\xa0", po.RightArrow, "\xa0 ", t.data.expires_at, " \xa0", po.RightArrow, "\xa0", uo.FromNow(t.data.expires_at, !0, !1), "\xa0", po.RightArrow, "\xa0", (0, wo.jsx)(qe, {
                                 to: $r.Path("/portal_access_key"),
                                 style: {
                                     color: "inherit"
                                 },
                                 children: "View"
                             })]
                         });
-                        if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, wo.jsxs)(Tu, {
+                        if (null !== (r = t.data) && void 0 !== r && r.invalid) return (0, wo.jsxs)(Au, {
                             children: [(0, wo.jsx)(oa, {
                                 id: "alert-access-key-invalid",
                                 position: "bottom",
                                 text: "Portal access key: ".concat(t.data.key)
                             }), (0, wo.jsxs)("b", {
                                 children: ["Alert: ", (0, wo.jsx)("span", {
                                     id: "alert-access-key-invalid",
@@ -56465,15 +56468,15 @@
                                     color: "inherit"
                                 },
                                 children: "View"
                             })]
                         })
                     }
                 },
-                Tu = function(e) {
+                Au = function(e) {
                     var t = e.children;
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("tr", {
                             children: (0, wo.jsx)("td", {
                                 style: {
                                     background: "black",
                                     height: "2px"
@@ -56498,15 +56501,15 @@
                                     height: "1px"
                                 },
                                 colSpan: "3"
                             })
                         })]
                     })
                 },
-                Au = function(e) {
+                zu = function(e) {
                     var t = e.header,
                         n = ln.LightenDarkenColor(ln.GetBackgroundColor(), -10),
                         r = function(e) {
                             var t = e.path,
                                 n = e.label;
                             return (0, wo.jsx)(wo.Fragment, {
                                 children: $r.CurrentLogicalPath() === t ? (0, wo.jsxs)("span", {
@@ -56580,15 +56583,15 @@
                                     path: "/login",
                                     label: co.IsLoggedIn(t) ? "Session" : "Login"
                                 })]
                             })]
                         })
                     })
                 },
-                zu = function(e) {
+                Ou = function(e) {
                     var t, n, r, o, i = e.header;
 
                     function a(e) {
                         return e ? {
                             textDecoration: "none",
                             color: "black",
                             fontWeight: "bold"
@@ -56664,29 +56667,29 @@
                         }), (0, wo.jsx)(oa, {
                             id: "tooltip-header-aws",
                             position: "bottom",
                             text: "Open AWS console for (".concat(null !== (n = i.app) && void 0 !== n && n.credentials.aws_account_name ? (null === (r = i.app) || void 0 === r ? void 0 : r.credentials.aws_account_name) + "/" : "").concat(null === (o = i.app) || void 0 === o ? void 0 : o.credentials.aws_account_number, ") account (in new tab).")
                         })]
                     })
                 },
-                Ou = function(e) {
+                _u = function(e) {
                     var t = e.header;
                     return (0, wo.jsxs)("span", {
-                        children: [(0, wo.jsx)(Au, {
+                        children: [(0, wo.jsx)(zu, {
                             header: t
                         }), (0, wo.jsx)(wo.Fragment, {
                             children: "\xa0|\xa0"
-                        }), (0, wo.jsx)(zu, {
+                        }), (0, wo.jsx)(Ou, {
                             header: t
                         })]
                     })
                 },
-                _u = function(e) {
+                Uu = function(e) {
                     var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k = Fa(),
-                        C = Nu(),
+                        C = Iu(),
                         E = Me(),
                         T = l(Ba(), 1)[0],
                         A = tn.IsFoursightFourfront(k) ? "#14533C" : "#143C53",
                         z = ln.LightenDarkenColor(ln.GetBackgroundColor(), -10);
                     return (0, wo.jsx)(wo.Fragment, {
                         children: k.loading ? (0, wo.jsxs)("div", {
                             style: {
@@ -56967,15 +56970,15 @@
                                                 style: {
                                                     paddingRight: "10pt",
                                                     whiteSpace: "nowrap",
                                                     color: "#D6EAF8"
                                                 },
                                                 align: "right",
                                                 children: [(0, wo.jsx)("small", {
-                                                    children: (0, wo.jsx)(Ss.Live, {
+                                                    children: (0, wo.jsx)(ks.Live, {
                                                         verbose: !0,
                                                         timezone: !1
                                                     })
                                                 }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, wo.jsxs)(wo.Fragment, {
                                                     children: ["\xa0|\xa0", (0, wo.jsx)(qe, {
                                                         id: "tooltip-header-account",
                                                         to: $r.Path("/login"),
@@ -57033,15 +57036,15 @@
                                                 width: "49%",
                                                 style: {
                                                     paddingLeft: "10pt",
                                                     paddingTop: "3pt",
                                                     paddingBottom: "3pt",
                                                     whiteSpace: "nowrap"
                                                 },
-                                                children: (0, wo.jsx)(Ou, {
+                                                children: (0, wo.jsx)(_u, {
                                                     header: k
                                                 })
                                             }), (0, wo.jsx)("td", {
                                                 width: "2%",
                                                 align: "center",
                                                 style: {
                                                     whiteSpace: "nowrap",
@@ -57363,15 +57366,15 @@
                                                                     })]
                                                                 })
                                                             })]
                                                         })
                                                     })
                                                 })
                                             })]
-                                        }), (0, wo.jsx)(ku, {
+                                        }), (0, wo.jsx)(Cu, {
                                             header: k
                                         }), (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     height: "1px",
                                                     background: "darkblue"
                                                 }
@@ -57389,25 +57392,25 @@
                                     children: (0, wo.jsx)("table", {
                                         children: (0, wo.jsx)("tbody", {
                                             children: (0, wo.jsx)("tr", {
                                                 children: (0, wo.jsx)("td", {
                                                     style: {
                                                         paddingLeft: "10pt"
                                                     },
-                                                    children: (0, wo.jsx)(Su, {})
+                                                    children: (0, wo.jsx)(ku, {})
                                                 })
                                             })
                                         })
                                     })
                                 })]
                             })]
                         })
                     })
                 },
-                Uu = function(e) {
+                Pu = function(e) {
                     var n = e.children,
                         r = l((0, t.useState)({
                             loading: !0
                         }), 2),
                         o = r[0],
                         i = r[1];
                     return Ua("/header", {
@@ -57423,15 +57426,15 @@
                         },
                         cache: !0
                     }), (0, wo.jsx)(Ra.Provider, {
                         value: [o, i],
                         children: n
                     })
                 },
-                Pu = function(e) {
+                Ru = function(e) {
                     var n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w = Fa(),
                         x = (tn.IsFoursightFourfront(w) ? "foursight" : "foursight-cgap") + ": " + (null === w || void 0 === w || null === (n = w.versions) || void 0 === n ? void 0 : n.foursight_core) + " | foursight-core: " + (null === w || void 0 === w || null === (r = w.versions) || void 0 === r ? void 0 : r.foursight) + " | dcicutils: " + (null === w || void 0 === w || null === (o = w.versions) || void 0 === o ? void 0 : o.dcicutils),
                         N = {
                             id: "".concat(null === (i = w.app) || void 0 === i || null === (a = i.credentials) || void 0 === a ? void 0 : a.aws_account_name, ":").concat(null === w || void 0 === w || null === (s = w.app) || void 0 === s ? void 0 : s.stage),
                             name: null === (u = w.app) || void 0 === u || null === (c = u.credentials) || void 0 === c ? void 0 : c.aws_account_name,
                             stage: null === (d = w.app) || void 0 === d ? void 0 : d.stage
                         },
@@ -57705,15 +57708,15 @@
                                         }
                                     })]
                                 })
                             })]
                         })
                     })
                 },
-                Ru = function(e) {
+                Fu = function(e) {
                     var n = e.title,
                         r = e.show,
                         o = void 0 === r || r,
                         i = e.info,
                         a = e.children,
                         s = l((0, t.useState)(o), 2),
                         u = s[0],
@@ -57802,15 +57805,15 @@
                                         children: "show"
                                     }), "."]
                                 })]
                             })
                         })
                     })
                 },
-                Fu = function(e) {
+                Bu = function(e) {
                     var t = e.name,
                         n = e.value,
                         r = e.monospace,
                         o = void 0 !== r && r,
                         i = e.copy,
                         a = void 0 === i || i,
                         s = e.size,
@@ -57998,15 +58001,15 @@
                                         })]
                                     }), O, _]
                                 }))]
                             }) : (0, wo.jsx)("span", {})
                         })
                     })
                 },
-                Bu = function() {
+                Yu = function() {
                     var e, n, r, o, i, a, s, u, c, d, p, f, h, g, y, m, v, M, j, b, w, x, N, I, D, L, S, k, C, E, T, A, z, O, _, U, P, R, F, B, Y, Q, G, W, H, V, Z, q, J, K, X, $, ee = Fa(),
                         te = Ua("/info"),
                         ne = l((0, t.useState)(!1), 2),
                         re = ne[0],
                         oe = ne[1],
                         ie = l((0, t.useState)(!1), 2),
                         ae = ie[0],
@@ -58017,268 +58020,268 @@
                         de = Ua("/portal_access_key"),
                         pe = hs();
                     return te.error ? (0, wo.jsx)(ua, {
                         error: te.error,
                         message: "Error loading info from Foursight API"
                     }) : (0, wo.jsxs)("div", {
                         className: "container",
-                        children: [(0, wo.jsxs)(Ru, {
+                        children: [(0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Versions",
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: null === (e = ee.app) || void 0 === e ? void 0 : e.package,
                                 value: null === (n = ee.versions) || void 0 === n ? void 0 : n.foursight,
                                 monospace: !0,
                                 copy: !0,
                                 pypi: !0,
                                 github: tn.IsFoursightFourfront(ee) ? "4dn-dcic" : "dbmi-bgm",
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "foursight-core",
                                 value: null === (r = ee.versions) || void 0 === r ? void 0 : r.foursight_core,
                                 monospace: !0,
                                 copy: !0,
                                 pypi: !0,
                                 github: "4dn-dcic",
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "dcicutils",
                                 value: null === (o = ee.versions) || void 0 === o ? void 0 : o.dcicutils,
                                 monospace: !0,
                                 copy: !0,
                                 pypi: !0,
                                 github: "4dn-dcic",
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "tibanna",
                                 value: null === (i = ee.versions) || void 0 === i ? void 0 : i.tibanna,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 pypi: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "tibanna-ff",
                                 value: null === (a = ee.versions) || void 0 === a ? void 0 : a.tibanna_ff,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 pypi: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "chalice",
                                 value: null === (s = ee.versions) || void 0 === s ? void 0 : s.chalice,
                                 monospace: !0,
                                 copy: !0,
                                 chalice: !0,
                                 size: "2",
                                 pypi: !0,
                                 github: "aws"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "python",
                                 value: null === (u = ee.versions) || void 0 === u ? void 0 : u.python,
                                 monospace: !0,
                                 copy: !0,
                                 python: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "elasticsearch-server",
                                 value: (null === (c = ee.versions) || void 0 === c ? void 0 : c.elasticsearch_server) || (null === (d = te.data) || void 0 === d || null === (p = d.versions) || void 0 === p ? void 0 : p.elasticsearch_server),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 elasticsearch: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "elasticsearch",
                                 value: null === (f = ee.versions) || void 0 === f ? void 0 : f.elasticsearch,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 pypi: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "elasticsearch-dsl",
                                 value: null === (h = ee.versions) || void 0 === h ? void 0 : h.elasticsearch_dsl,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 pypi: !0
                             }), (null === (g = te.data) || void 0 === g || null === (y = g.versions) || void 0 === y ? void 0 : y.redis_server) && (0, wo.jsxs)(wo.Fragment, {
-                                children: [(0, wo.jsx)(Fu, {
+                                children: [(0, wo.jsx)(Bu, {
                                     name: "redis-server",
                                     value: (null === (m = ee.versions) || void 0 === m ? void 0 : m.redis_server) || (null === (v = te.data) || void 0 === v || null === (M = v.versions) || void 0 === M ? void 0 : M.redis_server),
                                     monospace: !0,
                                     copy: !0,
                                     size: "2",
                                     redis: !0
-                                }), (0, wo.jsx)(Fu, {
+                                }), (0, wo.jsx)(Bu, {
                                     name: "redis",
                                     value: null === (j = ee.versions) || void 0 === j ? void 0 : j.redis,
                                     monospace: !0,
                                     copy: !0,
                                     size: "2",
                                     pypi: !0
                                 })]
                             })]
-                        }), (0, wo.jsxs)(Ru, {
+                        }), (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Credentials Info",
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: "AWS Account Number",
                                 value: te.get("app.credentials.aws_account_number"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "AWS Region Name",
                                 value: te.get("app.credentials.aws_region"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "AWS User ARN",
                                 value: te.get("app.credentials.aws_user_arn"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "AWS Access Key ID",
                                 value: te.get("app.credentials.aws_access_key_id"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), te.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, wo.jsx)(Fu, {
+                            }), te.get("environ.S3_AWS_ACCESS_KEY_ID") && (0, wo.jsx)(Bu, {
                                 name: "AWS S3 Access Key ID",
                                 value: te.get("environ.S3_AWS_ACCESS_KEY_ID"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Portal Access Key",
                                 value: de.get("key"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 portalAccessKey: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Auth0 Client ID",
                                 value: te.get("app.credentials.auth0_client_id"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
                             })]
-                        }), (0, wo.jsxs)(Ru, {
+                        }), (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Resources",
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: "Foursight Server",
                                 value: te.get("server.foursight"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Foursight",
                                 value: null === (b = ee.resources) || void 0 === b ? void 0 : b.foursight,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Portal",
                                 value: null === (w = ee.resources) || void 0 === w ? void 0 : w.portal,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
                                 portalCertificate: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "ElasticSearch",
                                 value: "".concat(null === (x = ee.resources) || void 0 === x ? void 0 : x.es, " (").concat(null === (N = ee.resources) || void 0 === N ? void 0 : N.es_cluster, ")"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "RDS",
                                 value: null === (I = ee.resources) || void 0 === I ? void 0 : I.rds,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "SQS",
                                 value: null === (D = ee.resources) || void 0 === D ? void 0 : D.sqs,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (null === (L = ee.resources) || void 0 === L ? void 0 : L.redis_running) && (0, wo.jsx)(Fu, {
+                            }), (null === (L = ee.resources) || void 0 === L ? void 0 : L.redis_running) && (0, wo.jsx)(Bu, {
                                 name: "Redis",
                                 value: null === (S = ee.resources) || void 0 === S ? void 0 : S.redis,
                                 nocheck: !(null !== (k = ee.resources) && void 0 !== k && k.redis_running),
                                 check: null === (C = ee.resources) || void 0 === C ? void 0 : C.redis_running,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
                             })]
-                        }), (0, wo.jsxs)(Ru, {
+                        }), (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Authentication/Authorization Info",
                             show: !0,
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: "Email",
                                 value: null === (E = co.Token()) || void 0 === E ? void 0 : E.user,
                                 monospace: !0,
                                 copy: !0,
                                 check: null === (T = co.Token()) || void 0 === T ? void 0 : T.user_verified,
                                 link: $r.Path("/users/" + co.LoggedInUser(ee), !0),
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "First Name",
                                 value: null === (A = co.Token()) || void 0 === A ? void 0 : A.first_name,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Last Name",
                                 value: null === (z = co.Token()) || void 0 === z ? void 0 : z.last_name,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environments",
                                 value: null === (O = co.Token()) || void 0 === O ? void 0 : O.allowed_envs.join(", "),
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Audience",
                                 value: null === (_ = co.Token()) || void 0 === _ ? void 0 : _.aud,
                                 monospace: !0,
                                 copy: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Issued At",
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
-                                value: (0, wo.jsx)(Cs.Live, {
+                                value: (0, wo.jsx)(Es.Live, {
                                     start: null === (U = co.Token()) || void 0 === U ? void 0 : U.authenticated_at,
                                     verbose: !0,
                                     fallback: "just now",
                                     suffix: "ago",
                                     tooltip: !0,
                                     prefix: "datetime"
                                 })
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Expires At",
                                 monospace: !0,
                                 copy: !0,
                                 size: "2",
-                                value: (0, wo.jsx)(Cs.Live, {
+                                value: (0, wo.jsx)(Es.Live, {
                                     end: null === (P = co.Token()) || void 0 === P ? void 0 : P.authenticated_until,
                                     verbose: !0,
                                     fallback: "now",
                                     suffix: "from now",
                                     tooltip: !0,
                                     prefix: "datetime"
                                 })
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Using Redis",
                                 monospace: !0,
                                 size: "2",
                                 value: null !== (R = ee.resources) && void 0 !== R && R.redis_running ? "Yes" : "No"
                             }), (0, wo.jsx)("hr", {
                                 style: {
                                     borderTop: "1px solid darkblue",
@@ -58339,77 +58342,77 @@
                                     children: (0, wo.jsxs)("b", {
                                         children: [(0, wo.jsx)("u", {
                                             children: "AuthToken"
                                         }), "\xa0", po.UpArrow]
                                     })
                                 }), (0, wo.jsx)("br", {})]
                             })]
-                        }), (0, wo.jsxs)(Ru, {
+                        }), (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Environment Names",
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: "Environment Name",
                                 value: tn.RegularName(tn.Current(), ee),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environment Name (Full)",
                                 value: tn.FullName(tn.Current(), ee),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environment Name (Short)",
                                 value: tn.ShortName(tn.Current(), ee),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environment Name (Public)",
                                 value: tn.PublicName(tn.Current(), ee),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environment Name (Foursight)",
                                 value: tn.FoursightName(tn.Current(), ee),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environment Name (Preferred)",
                                 value: tn.PreferredName(tn.Current(ee), ee),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
                             })]
-                        }), (0, wo.jsxs)(Ru, {
+                        }), (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Bucket Names",
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: "Global Environment Bucket",
                                 value: te.get("buckets.env"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Foursight Bucket Name",
                                 value: te.get("buckets.foursight"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Foursight Bucket Prefix",
                                 value: te.get("buckets.foursight_prefix"),
                                 monospace: !0,
                                 copy: !0,
                                 size: "3"
                             })]
-                        }), (0, wo.jsx)(Ru, {
+                        }), (0, wo.jsx)(Fu, {
                             info: te,
                             title: "Environment & Bucket Names",
                             children: (0, wo.jsx)("pre", {
                                 className: "box",
                                 style: {
                                     border: "0",
                                     margin: "0",
@@ -58424,15 +58427,15 @@
                                             marginTop: "6px",
                                             marginBottom: "6px",
                                             background: "black"
                                         }
                                     }) : (0, wo.jsx)("span", {})]
                                 }, Jr()())
                             })
-                        }), (0, wo.jsx)(Ru, {
+                        }), (0, wo.jsx)(Fu, {
                             info: te,
                             title: "Ecosystem",
                             show: !1,
                             children: (0, wo.jsx)("pre", {
                                 className: "box",
                                 style: {
                                     border: "0",
@@ -58440,70 +58443,70 @@
                                     paddingTop: "8",
                                     paddingBottom: "8",
                                     marginTop: "0"
                                 },
                                 children: Ia.Format(te.get("buckets.ecosystem"))
                             })
                         }), te.get("environ.AWS_LAMBDA_LOG_GROUP_NAME") && te.get("environ.AWS_LAMBDA_LOG_STREAM_NAME") && (0, wo.jsx)(wo.Fragment, {
-                            children: (0, wo.jsxs)(Ru, {
+                            children: (0, wo.jsxs)(Fu, {
                                 info: te,
                                 title: "Logs",
-                                children: [(0, wo.jsx)(Fu, {
+                                children: [(0, wo.jsx)(Bu, {
                                     name: "Log Group",
                                     value: te.get("environ.AWS_LAMBDA_LOG_GROUP_NAME"),
                                     monospace: !0,
                                     size: "2"
-                                }), (0, wo.jsx)(Fu, {
+                                }), (0, wo.jsx)(Bu, {
                                     name: "Log Stream",
                                     value: te.get("environ.AWS_LAMBDA_LOG_STREAM_NAME"),
                                     monospace: !0,
                                     size: "2"
                                 })]
                             })
-                        }), te.get("app.lambda") && (0, wo.jsxs)(Ru, {
+                        }), te.get("app.lambda") && (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Lambda",
                             show: !1,
-                            children: [(0, wo.jsx)(Fu, {
+                            children: [(0, wo.jsx)(Bu, {
                                 name: "Name",
                                 value: te.get("app.lambda.lambda_name"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Function",
                                 value: te.get("app.lambda.lambda_function_name"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "ARN",
                                 value: te.get("app.lambda.lambda_function_arn"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "S3 Location",
                                 value: te.get("app.lambda.lambda_code_s3_bucket") + "/" + te.get("app.lambda.lambda_code_s3_bucket_key"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Size",
                                 value: te.get("app.lambda.lambda_code_size"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Modified",
-                                value: Ss.Format(te.get("app.lambda.lambda_modified")),
+                                value: ks.Format(te.get("app.lambda.lambda_modified")),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Role",
                                 value: te.get("app.lambda.lambda_role"),
                                 monospace: !0,
                                 size: "2"
                             })]
-                        }), (0, wo.jsxs)(Ru, {
+                        }), (0, wo.jsxs)(Fu, {
                             info: te,
                             title: "Miscellany",
                             children: [le ? (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("div", {
                                     id: "tooltip-info-reloading",
                                     style: {
                                         float: "right"
@@ -58557,109 +58560,109 @@
                                     }
                                 })]
                             }), (0, wo.jsx)(oa, {
                                 id: "tooltip-info-clear",
                                 position: "bottom",
                                 size: "small",
                                 text: "Click to clear any server-side caches."
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "App Deployed At",
-                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Cs.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
+                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
                                 monospace: !0,
                                 copy: !0,
                                 optional: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "App Launched At",
-                                value: (null === (Q = ee.app) || void 0 === Q ? void 0 : Q.launched) + Cs.Format(null === (G = ee.app) || void 0 === G ? void 0 : G.launched, new Date, !0, "just now", "|", "ago"),
+                                value: (null === (Q = ee.app) || void 0 === Q ? void 0 : Q.launched) + Es.Format(null === (G = ee.app) || void 0 === G ? void 0 : G.launched, new Date, !0, "just now", "|", "ago"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Page Loaded At",
-                                value: te.get("page.loaded") + Cs.Format(te.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
+                                value: te.get("page.loaded") + Es.Format(te.get("page.loaded"), new Date, !0, "just now", "|", "ago"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Package",
                                 value: null === (W = ee.app) || void 0 === W ? void 0 : W.package,
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Stage",
                                 value: null === (H = ee.app) || void 0 === H ? void 0 : H.stage,
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Environment",
                                 value: tn.Current(),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Domain",
                                 value: null === (V = ee.app) || void 0 === V ? void 0 : V.domain,
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Context",
                                 value: null === (Z = ee.app) || void 0 === Z ? void 0 : Z.context,
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Path",
                                 value: te.get("page.path"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Endpoint",
                                 value: te.get("page.endpoint"),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Client (React UI)",
                                 value: $r.BaseUrl(),
                                 monospace: !0,
                                 size: "2"
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Server (React API)",
                                 value: rn.BaseUrl(),
                                 monospace: !0,
                                 size: "2",
                                 apiCache: !0
-                            }), (0, wo.jsx)(Fu, {
+                            }), (0, wo.jsx)(Bu, {
                                 name: "Checks File",
                                 value: null === (q = te.data) || void 0 === q || null === (J = q.checks) || void 0 === J ? void 0 : J.file,
                                 monospace: !0,
                                 size: "2"
-                            }), (null === (K = ee.app) || void 0 === K ? void 0 : K.accounts_file) && (0, wo.jsx)(Fu, {
+                            }), (null === (K = ee.app) || void 0 === K ? void 0 : K.accounts_file) && (0, wo.jsx)(Bu, {
                                 name: "Accounts File",
                                 value: null === (X = ee.app) || void 0 === X ? void 0 : X.accounts_file,
                                 monospace: !0,
                                 size: "2"
                             })]
-                        }), (0, wo.jsx)(Ru, {
+                        }), (0, wo.jsx)(Fu, {
                             info: te,
                             title: "GAC: ".concat(te.get("app.identity")),
                             show: !1,
                             children: te.get("gac.values") ? (0, wo.jsx)("span", {
                                 children: Object.keys(te.get("gac.values")).map((function(e) {
-                                    return (0, wo.jsx)(Fu, {
+                                    return (0, wo.jsx)(Bu, {
                                         name: e,
                                         value: te.get("gac.values")[e],
                                         monospace: !0,
                                         copy: !0
                                     }, e)
                                 }))
                             }) : (0, wo.jsx)("span", {})
-                        }), (0, wo.jsx)(Ru, {
+                        }), (0, wo.jsx)(Fu, {
                             info: te,
                             title: "Environment Variables",
                             show: !1,
                             children: te.get("environ") ? (0, wo.jsx)("span", {
                                 children: Object.keys(te.get("environ")).map((function(e) {
-                                    return (0, wo.jsx)(Fu, {
+                                    return (0, wo.jsx)(Bu, {
                                         name: e,
                                         value: te.get("environ")[e],
                                         monospace: !0,
                                         copy: !0
                                     }, e)
                                 }))
                             }) : (0, wo.jsx)("span", {})
@@ -58699,40 +58702,40 @@
                                         children: "show"
                                     }), "."]
                                 })]
                             })
                         })]
                     })
                 },
-                Yu = function(e, t) {
-                    return Yu = Object.setPrototypeOf || {
+                Qu = function(e, t) {
+                    return Qu = Object.setPrototypeOf || {
                         __proto__: []
                     }
                     instanceof Array && function(e, t) {
                         e.__proto__ = t
                     } || function(e, t) {
                         for (var n in t) t.hasOwnProperty(n) && (e[n] = t[n])
-                    }, Yu(e, t)
+                    }, Qu(e, t)
                 };
 
-            function Qu(e, t) {
+            function Gu(e, t) {
                 function n() {
                     this.constructor = e
                 }
-                Yu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+                Qu(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
             }
-            var Gu, Wu, Hu, Vu = function() {
-                return Vu = Object.assign || function(e) {
+            var Wu, Hu, Vu, Zu = function() {
+                return Zu = Object.assign || function(e) {
                     for (var t, n = 1, r = arguments.length; n < r; n++)
                         for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                     return e
-                }, Vu.apply(this, arguments)
+                }, Zu.apply(this, arguments)
             };
 
-            function Zu(e, t, n, r) {
+            function qu(e, t, n, r) {
                 return new(n || (n = Promise))((function(o, i) {
                     function a(e) {
                         try {
                             u(r.next(e))
                         } catch (t) {
                             i(t)
                         }
@@ -58752,15 +58755,15 @@
                             e(t)
                         }))).then(a, s)
                     }
                     u((r = r.apply(e, t || [])).next())
                 }))
             }
 
-            function qu(e, t) {
+            function Ju(e, t) {
                 var n, r, o, i, a = {
                     label: 0,
                     sent: function() {
                         if (1 & o[0]) throw o[1];
                         return o[1]
                     },
                     trys: [],
@@ -58828,15 +58831,15 @@
                                 done: !0
                             }
                         }([i, s])
                     }
                 }
             }
 
-            function Ju(e, t) {
+            function Ku(e, t) {
                 var n = "function" === typeof Symbol && e[Symbol.iterator];
                 if (!n) return e;
                 var r, o, i = n.call(e),
                     a = [];
                 try {
                     for (;
                         (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -58850,47 +58853,47 @@
                     } finally {
                         if (o) throw o.error
                     }
                 }
                 return a
             }
 
-            function Ku(e) {
+            function Xu(e) {
                 return e && !!["provider"].find((function(t) {
                     return e.hasOwnProperty(t)
                 }))
             }
 
-            function Xu(e) {
+            function $u(e) {
                 return void 0 !== e.redirectSignIn
             }! function(e) {
                 e.Cognito = "COGNITO", e.Google = "Google", e.Facebook = "Facebook", e.Amazon = "LoginWithAmazon", e.Apple = "SignInWithApple"
-            }(Gu || (Gu = {})),
+            }(Wu || (Wu = {})),
             function(e) {
                 e.NoConfig = "noConfig", e.MissingAuthConfig = "missingAuthConfig", e.EmptyUsername = "emptyUsername", e.InvalidUsername = "invalidUsername", e.EmptyPassword = "emptyPassword", e.EmptyCode = "emptyCode", e.SignUpError = "signUpError", e.NoMFA = "noMFA", e.InvalidMFA = "invalidMFA", e.EmptyChallengeResponse = "emptyChallengeResponse", e.NoUserSession = "noUserSession", e.Default = "default", e.DeviceConfig = "deviceConfig", e.NetworkError = "networkError", e.AutoSignInError = "autoSignInError"
-            }(Wu || (Wu = {})),
+            }(Hu || (Hu = {})),
             function(e) {
                 e.API_KEY = "API_KEY", e.AWS_IAM = "AWS_IAM", e.OPENID_CONNECT = "OPENID_CONNECT", e.AMAZON_COGNITO_USER_POOLS = "AMAZON_COGNITO_USER_POOLS", e.AWS_LAMBDA = "AWS_LAMBDA"
-            }(Hu || (Hu = {}));
-            var $u, el = function(e) {
+            }(Vu || (Vu = {}));
+            var el, tl = function(e) {
                     var t = "function" === typeof Symbol && Symbol.iterator,
                         n = t && e[t],
                         r = 0;
                     if (n) return n.call(e);
                     if (e && "number" === typeof e.length) return {
                         next: function() {
                             return e && r >= e.length && (e = void 0), {
                                 value: e && e[r++],
                                 done: !e
                             }
                         }
                     };
                     throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
                 },
-                tl = function(e, t) {
+                nl = function(e, t) {
                     var n = "function" === typeof Symbol && e[Symbol.iterator];
                     if (!n) return e;
                     var r, o, i = n.call(e),
                         a = [];
                     try {
                         for (;
                             (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -58903,56 +58906,56 @@
                             r && !r.done && (n = i.return) && n.call(i)
                         } finally {
                             if (o) throw o.error
                         }
                     }
                     return a
                 },
-                nl = function(e, t, n) {
+                rl = function(e, t, n) {
                     if (n || 2 === arguments.length)
                         for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
                     return e.concat(r || Array.prototype.slice.call(t))
                 },
-                rl = {
+                ol = {
                     VERBOSE: 1,
                     DEBUG: 2,
                     INFO: 3,
                     WARN: 4,
                     ERROR: 5
                 };
             ! function(e) {
                 e.DEBUG = "DEBUG", e.ERROR = "ERROR", e.INFO = "INFO", e.WARN = "WARN", e.VERBOSE = "VERBOSE"
-            }($u || ($u = {}));
-            var ol = function() {
+            }(el || (el = {}));
+            var il = function() {
                     function e(e, t) {
-                        void 0 === t && (t = $u.WARN), this.name = e, this.level = t, this._pluggables = []
+                        void 0 === t && (t = el.WARN), this.name = e, this.level = t, this._pluggables = []
                     }
                     return e.prototype._padding = function(e) {
                         return e < 10 ? "0" + e : "" + e
                     }, e.prototype._ts = function() {
                         var e = new Date;
                         return [this._padding(e.getMinutes()), this._padding(e.getSeconds())].join(":") + "." + e.getMilliseconds()
                     }, e.prototype.configure = function(e) {
                         return e ? (this._config = e, this._config) : this._config
                     }, e.prototype._log = function(t) {
                         for (var n, r, o = [], i = 1; i < arguments.length; i++) o[i - 1] = arguments[i];
                         var a = this.level;
-                        if (e.LOG_LEVEL && (a = e.LOG_LEVEL), "undefined" !== typeof window && window.LOG_LEVEL && (a = window.LOG_LEVEL), rl[t] >= rl[a]) {
+                        if (e.LOG_LEVEL && (a = e.LOG_LEVEL), "undefined" !== typeof window && window.LOG_LEVEL && (a = window.LOG_LEVEL), ol[t] >= ol[a]) {
                             var s = console.log.bind(console);
-                            t === $u.ERROR && console.error && (s = console.error.bind(console)), t === $u.WARN && console.warn && (s = console.warn.bind(console));
+                            t === el.ERROR && console.error && (s = console.error.bind(console)), t === el.WARN && console.warn && (s = console.warn.bind(console));
                             var u = "[".concat(t, "] ").concat(this._ts(), " ").concat(this.name),
                                 l = "";
                             if (1 === o.length && "string" === typeof o[0]) s(l = "".concat(u, " - ").concat(o[0]));
                             else if (1 === o.length) l = "".concat(u, " ").concat(o[0]), s(u, o[0]);
                             else if ("string" === typeof o[0]) {
                                 var c = o.slice(1);
                                 1 === c.length && (c = c[0]), l = "".concat(u, " - ").concat(o[0], " ").concat(c), s("".concat(u, " - ").concat(o[0]), c)
                             } else l = "".concat(u, " ").concat(o), s(u, o);
                             try {
-                                for (var d = el(this._pluggables), p = d.next(); !p.done; p = d.next()) {
+                                for (var d = tl(this._pluggables), p = d.next(); !p.done; p = d.next()) {
                                     var f = p.value,
                                         h = {
                                             message: l,
                                             timestamp: Date.now()
                                         };
                                     f.pushLogs([h])
                                 }
@@ -58966,44 +58969,44 @@
                                 } finally {
                                     if (n) throw n.error
                                 }
                             }
                         }
                     }, e.prototype.log = function() {
                         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                        this._log.apply(this, nl([$u.INFO], tl(e), !1))
+                        this._log.apply(this, rl([el.INFO], nl(e), !1))
                     }, e.prototype.info = function() {
                         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                        this._log.apply(this, nl([$u.INFO], tl(e), !1))
+                        this._log.apply(this, rl([el.INFO], nl(e), !1))
                     }, e.prototype.warn = function() {
                         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                        this._log.apply(this, nl([$u.WARN], tl(e), !1))
+                        this._log.apply(this, rl([el.WARN], nl(e), !1))
                     }, e.prototype.error = function() {
                         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                        this._log.apply(this, nl([$u.ERROR], tl(e), !1))
+                        this._log.apply(this, rl([el.ERROR], nl(e), !1))
                     }, e.prototype.debug = function() {
                         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                        this._log.apply(this, nl([$u.DEBUG], tl(e), !1))
+                        this._log.apply(this, rl([el.DEBUG], nl(e), !1))
                     }, e.prototype.verbose = function() {
                         for (var e = [], t = 0; t < arguments.length; t++) e[t] = arguments[t];
-                        this._log.apply(this, nl([$u.VERBOSE], tl(e), !1))
+                        this._log.apply(this, rl([el.VERBOSE], nl(e), !1))
                     }, e.prototype.addPluggable = function(e) {
                         e && "Logging" === e.getCategoryName() && (this._pluggables.push(e), e.configure(this._config))
                     }, e.prototype.listPluggables = function() {
                         return this._pluggables
                     }, e.LOG_LEVEL = null, e
                 }(),
-                il = function() {
-                    return il = Object.assign || function(e) {
+                al = function() {
+                    return al = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, il.apply(this, arguments)
+                    }, al.apply(this, arguments)
                 },
-                al = function(e, t) {
+                sl = function(e, t) {
                     var n = "function" === typeof Symbol && e[Symbol.iterator];
                     if (!n) return e;
                     var r, o, i = n.call(e),
                         a = [];
                     try {
                         for (;
                             (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59016,61 +59019,61 @@
                             r && !r.done && (n = i.return) && n.call(i)
                         } finally {
                             if (o) throw o.error
                         }
                     }
                     return a
                 },
-                sl = function(e, t, n) {
+                ul = function(e, t, n) {
                     if (n || 2 === arguments.length)
                         for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
                     return e.concat(r || Array.prototype.slice.call(t))
                 },
-                ul = new ol("Hub"),
-                ll = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
-            var cl = function() {
+                ll = new il("Hub"),
+                cl = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default";
+            var dl = function() {
                     function e(e) {
                         this.listeners = [], this.patterns = [], this.protectedChannels = ["core", "auth", "api", "analytics", "interactions", "pubsub", "storage", "ui", "xr"], this.name = e
                     }
                     return e.prototype._remove = function(e, t) {
                         if (e instanceof RegExp) {
                             var n = this.patterns.find((function(t) {
                                 return t.pattern.source === e.source
                             }));
-                            if (!n) return void ul.warn("No listeners for ".concat(e));
-                            this.patterns = sl([], al(this.patterns.filter((function(e) {
+                            if (!n) return void ll.warn("No listeners for ".concat(e));
+                            this.patterns = ul([], sl(this.patterns.filter((function(e) {
                                 return e !== n
                             }))), !1)
                         } else {
                             var r = this.listeners[e];
-                            if (!r) return void ul.warn("No listeners for ".concat(e));
-                            this.listeners[e] = sl([], al(r.filter((function(e) {
+                            if (!r) return void ll.warn("No listeners for ".concat(e));
+                            this.listeners[e] = ul([], sl(r.filter((function(e) {
                                 return e.callback !== t
                             }))), !1)
                         }
                     }, e.prototype.remove = function(e, t) {
                         this._remove(e, t)
                     }, e.prototype.dispatch = function(e, t, n, r) {
-                        (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === ll || ul.warn("WARNING: ".concat(e, " is protected and dispatching on it can have unintended consequences")));
+                        (void 0 === n && (n = ""), this.protectedChannels.indexOf(e) > -1) && (r === cl || ll.warn("WARNING: ".concat(e, " is protected and dispatching on it can have unintended consequences")));
                         var o = {
                             channel: e,
-                            payload: il({}, t),
+                            payload: al({}, t),
                             source: n,
                             patternInfo: []
                         };
                         try {
                             this._toListeners(o)
                         } catch (i) {
-                            ul.error(i)
+                            ll.error(i)
                         }
                     }, e.prototype.listen = function(e, t, n) {
                         var r, o = this;
                         if (void 0 === n && (n = "noname"), function(e) {
                                 return void 0 !== e.onHubCapsule
-                            }(t)) ul.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
+                            }(t)) ll.warn("WARNING onHubCapsule is Deprecated. Please pass in a callback."), r = t.onHubCapsule.bind(t);
                         else {
                             if ("function" !== typeof t) throw new Error("No callback supplied to Hub");
                             r = t
                         }
                         if (e instanceof RegExp) this.patterns.push({
                             pattern: e,
                             callback: r
@@ -59086,73 +59089,73 @@
                             o._remove(e, r)
                         }
                     }, e.prototype._toListeners = function(e) {
                         var t = e.channel,
                             n = e.payload,
                             r = this.listeners[t];
                         if (r && r.forEach((function(r) {
-                                ul.debug("Dispatching to ".concat(t, " with "), n);
+                                ll.debug("Dispatching to ".concat(t, " with "), n);
                                 try {
                                     r.callback(e)
                                 } catch (o) {
-                                    ul.error(o)
+                                    ll.error(o)
                                 }
                             })), this.patterns.length > 0) {
-                            if (!n.message) return void ul.warn("Cannot perform pattern matching without a message key");
+                            if (!n.message) return void ll.warn("Cannot perform pattern matching without a message key");
                             var o = n.message;
                             this.patterns.forEach((function(t) {
                                 var n = o.match(t.pattern);
                                 if (n) {
-                                    var r = al(n).slice(1),
-                                        i = il(il({}, e), {
+                                    var r = sl(n).slice(1),
+                                        i = al(al({}, e), {
                                             patternInfo: r
                                         });
                                     try {
                                         t.callback(i)
                                     } catch (a) {
-                                        ul.error(a)
+                                        ll.error(a)
                                     }
                                 }
                             }))
                         }
                     }, e
                 }(),
-                dl = new cl("__default__"),
-                pl = {},
-                fl = function() {
+                pl = new dl("__default__"),
+                fl = {},
+                hl = function() {
                     function e() {}
                     return e.setItem = function(e, t) {
-                        return pl[e] = t, pl[e]
+                        return fl[e] = t, fl[e]
                     }, e.getItem = function(e) {
-                        return Object.prototype.hasOwnProperty.call(pl, e) ? pl[e] : void 0
+                        return Object.prototype.hasOwnProperty.call(fl, e) ? fl[e] : void 0
                     }, e.removeItem = function(e) {
-                        return delete pl[e]
+                        return delete fl[e]
                     }, e.clear = function() {
-                        return pl = {}
+                        return fl = {}
                     }, e
                 }(),
-                hl = function() {
+                gl = function() {
                     function e() {
                         try {
                             this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.amplify.test-ls", 1), this.storageWindow.removeItem("aws.amplify.test-ls")
                         } catch (e) {
-                            this.storageWindow = fl
+                            this.storageWindow = hl
                         }
                     }
                     return e.prototype.getStorage = function() {
                         return this.storageWindow
                     }, e
                 }(),
-                gl = function() {
+                yl = function() {
                     return {
                         isBrowser: "undefined" !== typeof window && "undefined" !== typeof window.document,
                         isNode: "undefined" !== typeof process && null != process.versions && null != process.versions.node
                     }
                 },
-                yl = function() {
+                ml = function() {
                     var e = function(t, n) {
                         return e = Object.setPrototypeOf || {
                             __proto__: []
                         }
                         instanceof Array && function(e, t) {
                             e.__proto__ = t
                         } || function(e, t) {
@@ -59164,15 +59167,15 @@
 
                         function r() {
                             this.constructor = t
                         }
                         e(t, n), t.prototype = null === n ? Object.create(n) : (r.prototype = n.prototype, new r)
                     }
                 }(),
-                ml = function(e, t, n, r) {
+                vl = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -59191,15 +59194,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                vl = function(e, t) {
+                Ml = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -59266,15 +59269,15 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                Ml = function(e, t) {
+                jl = function(e, t) {
                     var n = "function" === typeof Symbol && e[Symbol.iterator];
                     if (!n) return e;
                     var r, o, i = n.call(e),
                         a = [];
                     try {
                         for (;
                             (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59287,65 +59290,65 @@
                             r && !r.done && (n = i.return) && n.call(i)
                         } finally {
                             if (o) throw o.error
                         }
                     }
                     return a
                 },
-                jl = function(e, t, n) {
+                bl = function(e, t, n) {
                     if (n || 2 === arguments.length)
                         for (var r, o = 0, i = t.length; o < i; o++) !r && o in t || (r || (r = Array.prototype.slice.call(t, 0, o)), r[o] = t[o]);
                     return e.concat(r || Array.prototype.slice.call(t))
                 },
-                bl = new ol("Util"),
-                wl = function(e) {
+                wl = new il("Util"),
+                xl = function(e) {
                     function t(t) {
                         var n = e.call(this, t) || this;
                         return n.nonRetryable = !0, n
                     }
-                    return yl(t, e), t
+                    return ml(t, e), t
                 }(Error);
-            var xl = 3e5;
+            var Nl = 3e5;
 
-            function Nl(e) {
-                void 0 === e && (e = xl);
+            function Il(e) {
+                void 0 === e && (e = Nl);
                 return function(t) {
                     var n = 100 * Math.pow(2, t) + 100 * Math.random();
                     return !(n > e) && n
                 }
             }
-            var Il, Dl, Ll, Sl, kl, Cl, El, Tl, Al, zl, Ol, _l, Ul, Pl = function(e, t, n, r) {
-                    return void 0 === n && (n = xl),
+            var Dl, Ll, Sl, kl, Cl, El, Tl, Al, zl, Ol, _l, Ul, Pl, Rl = function(e, t, n, r) {
+                    return void 0 === n && (n = Nl),
                         function(e, t, n, r) {
-                            return ml(this, void 0, void 0, (function() {
+                            return vl(this, void 0, void 0, (function() {
                                 var o = this;
-                                return vl(this, (function(i) {
+                                return Ml(this, (function(i) {
                                     if ("function" !== typeof e) throw Error("functionToRetry must be a function");
                                     return [2, new Promise((function(i, a) {
-                                        return ml(o, void 0, void 0, (function() {
+                                        return vl(o, void 0, void 0, (function() {
                                             var o, s, u, l, c, d, p;
-                                            return vl(this, (function(f) {
+                                            return Ml(this, (function(f) {
                                                 switch (f.label) {
                                                     case 0:
                                                         o = 0, s = !1, l = function() {}, r && r.then((function() {
                                                             s = !0, clearTimeout(u), l()
                                                         })), d = function() {
                                                             var r, d, p, f;
-                                                            return vl(this, (function(h) {
+                                                            return Ml(this, (function(h) {
                                                                 switch (h.label) {
                                                                     case 0:
-                                                                        o++, bl.debug("".concat(e.name, " attempt #").concat(o, " with this vars: ").concat(JSON.stringify(t))), h.label = 1;
+                                                                        o++, wl.debug("".concat(e.name, " attempt #").concat(o, " with this vars: ").concat(JSON.stringify(t))), h.label = 1;
                                                                     case 1:
-                                                                        return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, jl([], Ml(t), !1))];
+                                                                        return h.trys.push([1, 3, , 7]), r = {}, d = i, [4, e.apply(void 0, bl([], jl(t), !1))];
                                                                     case 2:
                                                                         return [2, (r.value = d.apply(void 0, [h.sent()]), r)];
                                                                     case 3:
-                                                                        return p = h.sent(), c = p, bl.debug("error on ".concat(e.name), p), (g = p) && g.nonRetryable ? (bl.debug("".concat(e.name, " non retryable error"), p), [2, {
+                                                                        return p = h.sent(), c = p, wl.debug("error on ".concat(e.name), p), (g = p) && g.nonRetryable ? (wl.debug("".concat(e.name, " non retryable error"), p), [2, {
                                                                             value: a(p)
-                                                                        }]) : (f = n(o, t, p), bl.debug("".concat(e.name, " retrying in ").concat(f, " ms")), !1 === f || s ? [2, {
+                                                                        }]) : (f = n(o, t, p), wl.debug("".concat(e.name, " retrying in ").concat(f, " ms")), !1 === f || s ? [2, {
                                                                             value: a(p)
                                                                         }] : [3, 4]);
                                                                     case 4:
                                                                         return [4, new Promise((function(e) {
                                                                             l = e, u = setTimeout(l, f)
                                                                         }))];
                                                                     case 5:
@@ -59366,17 +59369,17 @@
                                                         return a(c), [2]
                                                 }
                                             }))
                                         }))
                                     }))]
                                 }))
                             }))
-                        }(e, t, Nl(n), r)
+                        }(e, t, Il(n), r)
                 },
-                Rl = function(e, t, n, r) {
+                Fl = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -59395,15 +59398,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                Fl = function(e, t) {
+                Bl = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -59470,60 +59473,60 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                Bl = new ol("CognitoCredentials"),
-                Yl = new Promise((function(e, t) {
-                    return gl().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (Bl.debug("google api already loaded"), e()) : void setTimeout((function() {
+                Yl = new il("CognitoCredentials"),
+                Ql = new Promise((function(e, t) {
+                    return yl().isBrowser ? (window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null) ? (Yl.debug("google api already loaded"), e()) : void setTimeout((function() {
                         return e()
-                    }), 2e3) : (Bl.debug("not in the browser, directly resolved"), e())
+                    }), 2e3) : (Yl.debug("not in the browser, directly resolved"), e())
                 })),
-                Ql = function() {
+                Gl = function() {
                     function e() {
                         this.initialized = !1, this.refreshGoogleToken = this.refreshGoogleToken.bind(this), this._refreshGoogleTokenImpl = this._refreshGoogleTokenImpl.bind(this)
                     }
                     return e.prototype.refreshGoogleToken = function() {
-                        return Rl(this, void 0, void 0, (function() {
-                            return Fl(this, (function(e) {
+                        return Fl(this, void 0, void 0, (function() {
+                            return Bl(this, (function(e) {
                                 switch (e.label) {
                                     case 0:
-                                        return this.initialized ? [3, 2] : (Bl.debug("need to wait for the Google SDK loaded"), [4, Yl]);
+                                        return this.initialized ? [3, 2] : (Yl.debug("need to wait for the Google SDK loaded"), [4, Ql]);
                                     case 1:
-                                        e.sent(), this.initialized = !0, Bl.debug("finish waiting"), e.label = 2;
+                                        e.sent(), this.initialized = !0, Yl.debug("finish waiting"), e.label = 2;
                                     case 2:
                                         return [2, this._refreshGoogleTokenImpl()]
                                 }
                             }))
                         }))
                     }, e.prototype._refreshGoogleTokenImpl = function() {
                         var e = null;
-                        return gl().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
+                        return yl().isBrowser && (e = window.gapi && window.gapi.auth2 ? window.gapi.auth2 : null), e ? new Promise((function(t, n) {
                             e.getAuthInstance().then((function(e) {
-                                e || (Bl.debug("google Auth undefined"), n(new wl("google Auth undefined")));
+                                e || (Yl.debug("google Auth undefined"), n(new xl("google Auth undefined")));
                                 var r = e.currentUser.get();
-                                r.isSignedIn() ? (Bl.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
+                                r.isSignedIn() ? (Yl.debug("refreshing the google access token"), r.reloadAuthResponse().then((function(e) {
                                     var n = e.id_token,
                                         r = e.expires_at;
                                     t({
                                         token: n,
                                         expires_at: r
                                     })
                                 })).catch((function(e) {
-                                    e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new wl("Failed to reload google auth response"))
-                                }))) : n(new wl("User is not signed in with Google"))
+                                    e && "network_error" === e.error ? n("Network error reloading google auth response") : n(new xl("Failed to reload google auth response"))
+                                }))) : n(new xl("User is not signed in with Google"))
                             })).catch((function(e) {
-                                Bl.debug("Failed to refresh google token", e), n(new wl("Failed to refresh google token"))
+                                Yl.debug("Failed to refresh google token", e), n(new xl("Failed to refresh google token"))
                             }))
-                        })) : (Bl.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
+                        })) : (Yl.debug("no gapi auth2 available"), Promise.reject("no gapi auth2 available"))
                     }, e
                 }(),
-                Gl = function(e, t, n, r) {
+                Wl = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -59542,15 +59545,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                Wl = function(e, t) {
+                Hl = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -59617,70 +59620,70 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                Hl = new ol("CognitoCredentials"),
-                Vl = new Promise((function(e, t) {
-                    return gl().isBrowser ? window.FB ? (Hl.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
+                Vl = new il("CognitoCredentials"),
+                Zl = new Promise((function(e, t) {
+                    return yl().isBrowser ? window.FB ? (Vl.debug("FB SDK already loaded"), e()) : void setTimeout((function() {
                         return e()
-                    }), 2e3) : (Hl.debug("not in the browser, directly resolved"), e())
+                    }), 2e3) : (Vl.debug("not in the browser, directly resolved"), e())
                 })),
-                Zl = function() {
+                ql = function() {
                     function e() {
                         this.initialized = !1, this.refreshFacebookToken = this.refreshFacebookToken.bind(this), this._refreshFacebookTokenImpl = this._refreshFacebookTokenImpl.bind(this)
                     }
                     return e.prototype.refreshFacebookToken = function() {
-                        return Gl(this, void 0, void 0, (function() {
-                            return Wl(this, (function(e) {
+                        return Wl(this, void 0, void 0, (function() {
+                            return Hl(this, (function(e) {
                                 switch (e.label) {
                                     case 0:
-                                        return this.initialized ? [3, 2] : (Hl.debug("need to wait for the Facebook SDK loaded"), [4, Vl]);
+                                        return this.initialized ? [3, 2] : (Vl.debug("need to wait for the Facebook SDK loaded"), [4, Zl]);
                                     case 1:
-                                        e.sent(), this.initialized = !0, Hl.debug("finish waiting"), e.label = 2;
+                                        e.sent(), this.initialized = !0, Vl.debug("finish waiting"), e.label = 2;
                                     case 2:
                                         return [2, this._refreshFacebookTokenImpl()]
                                 }
                             }))
                         }))
                     }, e.prototype._refreshFacebookTokenImpl = function() {
                         var e = null;
-                        if (gl().isBrowser && (e = window.FB), !e) {
+                        if (yl().isBrowser && (e = window.FB), !e) {
                             var t = "no fb sdk available";
-                            return Hl.debug(t), Promise.reject(new wl(t))
+                            return Vl.debug(t), Promise.reject(new xl(t))
                         }
                         return new Promise((function(t, n) {
                             e.getLoginStatus((function(e) {
                                 if (e && e.authResponse) {
                                     var r = e.authResponse,
                                         o = r.accessToken,
                                         i = 1e3 * r.expiresIn + (new Date).getTime();
                                     if (!o) {
                                         a = "the jwtToken is undefined";
-                                        Hl.debug(a), n(new wl(a))
+                                        Vl.debug(a), n(new xl(a))
                                     }
                                     t({
                                         token: o,
                                         expires_at: i
                                     })
                                 } else {
                                     var a = "no response from facebook when refreshing the jwt token";
-                                    Hl.debug(a), n(new wl(a))
+                                    Vl.debug(a), n(new xl(a))
                                 }
                             }), {
                                 scope: "public_profile,email"
                             })
                         }))
                     }, e
                 }(),
-                ql = new Ql,
-                Jl = new Zl,
-                Kl = function(e, t) {
+                Jl = new Gl,
+                Kl = new ql,
+                Xl = function(e, t) {
                     var n = "function" === typeof Symbol && e[Symbol.iterator];
                     if (!n) return e;
                     var r, o, i = n.call(e),
                         a = [];
                     try {
                         for (;
                             (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -59693,75 +59696,75 @@
                             r && !r.done && (n = i.return) && n.call(i)
                         } finally {
                             if (o) throw o.error
                         }
                     }
                     return a
                 },
-                Xl = new ol("Amplify"),
-                $l = new(function() {
+                $l = new il("Amplify"),
+                ec = new(function() {
                     function e() {
-                        this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = ol, this.ServiceWorker = null
+                        this._components = [], this._config = {}, this._modules = {}, this.Auth = null, this.Analytics = null, this.API = null, this.Credentials = null, this.Storage = null, this.I18n = null, this.Cache = null, this.PubSub = null, this.Interactions = null, this.Pushnotification = null, this.UI = null, this.XR = null, this.Predictions = null, this.DataStore = null, this.Geo = null, this.Notifications = null, this.Logger = il, this.ServiceWorker = null
                     }
                     return e.prototype.register = function(e) {
-                        Xl.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : Xl.debug("no getModuleName method for component", e), e.configure(this._config)
+                        $l.debug("component registered in amplify", e), this._components.push(e), "function" === typeof e.getModuleName ? (this._modules[e.getModuleName()] = e, this[e.getModuleName()] = e) : $l.debug("no getModuleName method for component", e), e.configure(this._config)
                     }, e.prototype.configure = function(e) {
                         var t = this;
-                        return e ? (this._config = Object.assign(this._config, e), Xl.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
-                            var n = Kl(e, 2),
+                        return e ? (this._config = Object.assign(this._config, e), $l.debug("amplify config", this._config), Object.entries(this._modules).forEach((function(e) {
+                            var n = Xl(e, 2),
                                 r = (n[0], n[1]);
                             Object.keys(r).forEach((function(e) {
                                 t._modules[e] && (r[e] = t._modules[e])
                             }))
                         })), this._components.map((function(e) {
                             e.configure(t._config)
                         })), this._config) : this._config
                     }, e.prototype.addPluggable = function(e) {
                         e && e.getCategory && "function" === typeof e.getCategory && this._components.map((function(t) {
                             t.addPluggable && "function" === typeof t.addPluggable && t.addPluggable(e)
                         }))
                     }, e
                 }()),
-                ec = {
+                tc = {
                     id: "aws",
                     outputs: {
                         dnsSuffix: "amazonaws.com"
                     },
                     regionRegex: "^(us|eu|ap|sa|ca|me|af)\\-\\w+\\-\\d+$",
                     regions: ["aws-global"]
                 },
-                tc = {
-                    partitions: [ec, {
+                nc = {
+                    partitions: [tc, {
                         id: "aws-cn",
                         outputs: {
                             dnsSuffix: "amazonaws.com.cn"
                         },
                         regionRegex: "^cn\\-\\w+\\-\\d+$",
                         regions: ["aws-cn-global"]
                     }]
                 },
-                nc = function(e) {
+                rc = function(e) {
                     var t = "function" === typeof Symbol && Symbol.iterator,
                         n = t && e[t],
                         r = 0;
                     if (n) return n.call(e);
                     if (e && "number" === typeof e.length) return {
                         next: function() {
                             return e && r >= e.length && (e = void 0), {
                                 value: e && e[r++],
                                 done: !e
                             }
                         }
                     };
                     throw new TypeError(t ? "Object is not iterable." : "Symbol.iterator is not defined.")
                 },
-                rc = function(e) {
-                    var t, n, r = tc.partitions;
+                oc = function(e) {
+                    var t, n, r = nc.partitions;
                     try {
-                        for (var o = nc(r), i = o.next(); !i.done; i = o.next()) {
+                        for (var o = rc(r), i = o.next(); !i.done; i = o.next()) {
                             var a = i.value,
                                 s = a.regions,
                                 u = a.outputs,
                                 l = a.regionRegex,
                                 c = new RegExp(l);
                             if (s.includes(e) || c.test(e)) return u.dnsSuffix
                         }
@@ -59772,17 +59775,17 @@
                     } finally {
                         try {
                             i && !i.done && (n = o.return) && n.call(o)
                         } finally {
                             if (t) throw t.error
                         }
                     }
-                    return ec.outputs.dnsSuffix
+                    return tc.outputs.dnsSuffix
                 },
-                oc = function(e, t, n, r) {
+                ic = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -59801,15 +59804,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                ic = function(e, t) {
+                ac = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -59876,32 +59879,32 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                ac = function(e, t) {
+                sc = function(e, t) {
                     if (null === t || void 0 === t ? void 0 : t.aborted) return Promise.resolve();
                     var n, r, o = new Promise((function(t) {
                         r = t, n = setTimeout(t, e)
                     }));
                     return null === t || void 0 === t || t.addEventListener("abort", (function e(o) {
                         clearTimeout(n), null === t || void 0 === t || t.removeEventListener("abort", e), r()
                     })), o
                 },
-                sc = function(e) {
+                uc = function(e) {
                     return "object" === typeof(null === e || void 0 === e ? void 0 : e.$metadata)
                 },
-                uc = function(e, t) {
-                    sc(e) && (e.$metadata.attempts = t), e.$metadata = {
+                lc = function(e, t) {
+                    uc(e) && (e.$metadata.attempts = t), e.$metadata = {
                         attempts: t
                     }
                 },
-                lc = function(e, t, n, r) {
+                cc = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -59920,15 +59923,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                cc = function(e, t) {
+                dc = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -59995,32 +59998,32 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                dc = function(e, t) {
+                pc = function(e, t) {
                     return function(n, r) {
                         for (var o = {}, i = function(t) {
                                 return e(t, r)
                             }, a = t.length - 1; a >= 0; a--) {
                             i = (0, t[a])(r)(i, o)
                         }
                         return i(n)
                     }
                 },
-                pc = (n(8117), function() {
-                    return pc = Object.assign || function(e) {
+                fc = (n(8117), function() {
+                    return fc = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, pc.apply(this, arguments)
+                    }, fc.apply(this, arguments)
                 }),
-                fc = function(e, t, n, r) {
+                hc = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -60039,15 +60042,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                hc = function(e, t) {
+                gc = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -60114,38 +60117,38 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                gc = function(e) {
+                yc = function(e) {
                     return !["HEAD", "GET", "DELETE"].includes(e.toUpperCase())
                 },
-                yc = function(e) {
+                mc = function(e) {
                     var t;
                     return function() {
                         return t || (t = e()), t
                     }
                 },
-                mc = dc((function(e, t) {
+                vc = pc((function(e, t) {
                     var n = e.url,
                         r = e.method,
                         o = e.headers,
                         i = e.body,
                         a = t.abortSignal;
-                    return fc(void 0, void 0, void 0, (function() {
+                    return hc(void 0, void 0, void 0, (function() {
                         var e, t, s, u, l, c, d;
-                        return hc(this, (function(p) {
+                        return gc(this, (function(p) {
                             switch (p.label) {
                                 case 0:
                                     return p.trys.push([0, 2, , 3]), [4, fetch(n, {
                                         method: r,
                                         headers: o,
-                                        body: gc(r) ? i : void 0,
+                                        body: yc(r) ? i : void 0,
                                         signal: a
                                     })];
                                 case 1:
                                     return e = p.sent(), [3, 3];
                                 case 2:
                                     if ((t = p.sent()) instanceof TypeError) throw new Error("Network error");
                                     throw t;
@@ -60153,39 +60156,39 @@
                                     return s = {}, null === (c = e.headers) || void 0 === c || c.forEach((function(e, t) {
                                         s[t.toLowerCase()] = e
                                     })), u = {
                                         statusCode: e.status,
                                         headers: s,
                                         body: null
                                     }, l = Object.assign(null !== (d = e.body) && void 0 !== d ? d : {}, {
-                                        text: yc((function() {
+                                        text: mc((function() {
                                             return e.text()
                                         })),
-                                        blob: yc((function() {
+                                        blob: mc((function() {
                                             return e.blob()
                                         })),
-                                        json: yc((function() {
+                                        json: mc((function() {
                                             return e.json()
                                         }))
-                                    }), [2, pc(pc({}, u), {
+                                    }), [2, fc(fc({}, u), {
                                         body: l
                                     })]
                             }
                         }))
                     }))
                 }), [function(e) {
                     var t = e.userAgentHeader,
                         n = void 0 === t ? "x-amz-user-agent" : t,
                         r = e.userAgentValue,
                         o = void 0 === r ? "" : r;
                     return function(e) {
                         return function(t) {
-                            return lc(this, void 0, void 0, (function() {
+                            return cc(this, void 0, void 0, (function() {
                                 var r;
-                                return cc(this, (function(i) {
+                                return dc(this, (function(i) {
                                     switch (i.label) {
                                         case 0:
                                             return 0 !== o.trim().length ? [3, 2] : [4, e(t)];
                                         case 1:
                                             return [2, i.sent()];
                                         case 2:
                                             return r = n.toLowerCase(), t.headers[r] = t.headers[r] ? "".concat(t.headers[r], " ").concat(o) : o, [4, e(t)];
@@ -60202,17 +60205,17 @@
                         r = e.retryDecider,
                         o = e.computeDelay,
                         i = e.abortSignal;
                     if (n < 1) throw new Error("maxAttempts must be greater than 0");
                     return function(e, t) {
                         return function(a) {
                             var s;
-                            return oc(this, void 0, void 0, (function() {
+                            return ic(this, void 0, void 0, (function() {
                                 var u, l, c, d, p;
-                                return ic(this, (function(f) {
+                                return ac(this, (function(f) {
                                     switch (f.label) {
                                         case 0:
                                             l = null !== (s = t.attemptsCount) && void 0 !== s ? s : 0, f.label = 1;
                                         case 1:
                                             if ((null === i || void 0 === i ? void 0 : i.aborted) || !(l < n)) return [3, 11];
                                             u = void 0, c = void 0, f.label = 2;
                                         case 2:
@@ -60220,50 +60223,50 @@
                                         case 3:
                                             return c = f.sent(), [3, 5];
                                         case 4:
                                             return d = f.sent(), u = d, [3, 5];
                                         case 5:
                                             return l = t.attemptsCount > l ? t.attemptsCount : l + 1, t.attemptsCount = l, [4, r(c, u)];
                                         case 6:
-                                            return f.sent() ? !(null === i || void 0 === i ? void 0 : i.aborted) && l < n ? (p = o(l), [4, ac(p, i)]) : [3, 8] : [3, 9];
+                                            return f.sent() ? !(null === i || void 0 === i ? void 0 : i.aborted) && l < n ? (p = o(l), [4, sc(p, i)]) : [3, 8] : [3, 9];
                                         case 7:
                                             f.sent(), f.label = 8;
                                         case 8:
                                             return [3, 1];
                                         case 9:
-                                            if (c) return uc(c, l), [2, c];
-                                            throw uc(u, l), u;
+                                            if (c) return lc(c, l), [2, c];
+                                            throw lc(u, l), u;
                                         case 10:
                                             return [3, 1];
                                         case 11:
                                             throw (null === i || void 0 === i ? void 0 : i.aborted) ? new Error("Request aborted") : null !== u && void 0 !== u ? u : new Error("Retry attempts exhausted")
                                     }
                                 }))
                             }))
                         }
                     }
                 }]),
-                vc = function() {
-                    return vc = Object.assign || function(e) {
+                Mc = function() {
+                    return Mc = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, vc.apply(this, arguments)
+                    }, Mc.apply(this, arguments)
                 },
-                Mc = function(e) {
+                jc = function(e) {
                     var t, n, r = e.headers,
                         o = e.statusCode;
-                    return vc(vc({}, sc(e) ? e.$metadata : {}), {
+                    return Mc(Mc({}, uc(e) ? e.$metadata : {}), {
                         httpStatusCode: o,
                         requestId: null !== (n = null !== (t = r["x-amzn-requestid"]) && void 0 !== t ? t : r["x-amzn-request-id"]) && void 0 !== n ? n : r["x-amz-request-id"],
                         extendedRequestId: r["x-amz-id-2"],
                         cfId: r["x-amz-cf-id"]
                     })
                 },
-                jc = function(e, t, n, r) {
+                bc = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -60282,15 +60285,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                bc = function(e, t) {
+                wc = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -60357,15 +60360,15 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                wc = function(e, t) {
+                xc = function(e, t) {
                     var n = "function" === typeof Symbol && e[Symbol.iterator];
                     if (!n) return e;
                     var r, o, i = n.call(e),
                         a = [];
                     try {
                         for (;
                             (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60378,54 +60381,54 @@
                             r && !r.done && (n = i.return) && n.call(i)
                         } finally {
                             if (o) throw o.error
                         }
                     }
                     return a
                 },
-                xc = function(e) {
-                    return jc(void 0, void 0, void 0, (function() {
+                Nc = function(e) {
+                    return bc(void 0, void 0, void 0, (function() {
                         var t, n, r, o, i, a, s, u, l;
-                        return bc(this, (function(c) {
+                        return wc(this, (function(c) {
                             switch (c.label) {
                                 case 0:
-                                    return !e || e.statusCode < 300 ? [2] : [4, Nc(e)];
+                                    return !e || e.statusCode < 300 ? [2] : [4, Ic(e)];
                                 case 1:
                                     return t = c.sent(), n = function(e) {
-                                        var t = wc(e.toString().split(/[\,\:]+/), 1)[0];
+                                        var t = xc(e.toString().split(/[\,\:]+/), 1)[0];
                                         return t.includes("#") ? t.split("#")[1] : t
                                     }(null !== (s = null !== (a = null !== (i = e.headers["x-amzn-errortype"]) && void 0 !== i ? i : t.code) && void 0 !== a ? a : t.__type) && void 0 !== s ? s : "UnknownError"), r = null !== (l = null !== (u = t.message) && void 0 !== u ? u : t.Message) && void 0 !== l ? l : "Unknown error", o = new Error(r), [2, Object.assign(o, {
                                         name: n,
-                                        $metadata: Mc(e)
+                                        $metadata: jc(e)
                                     })]
                             }
                         }))
                     }))
                 },
-                Nc = function(e) {
-                    return jc(void 0, void 0, void 0, (function() {
+                Ic = function(e) {
+                    return bc(void 0, void 0, void 0, (function() {
                         var t;
-                        return bc(this, (function(n) {
+                        return wc(this, (function(n) {
                             switch (n.label) {
                                 case 0:
                                     if (!e.body) throw new Error("Missing response payload");
                                     return [4, e.body.json()];
                                 case 1:
                                     return t = n.sent(), [2, Object.assign(t, {
-                                        $metadata: Mc(e)
+                                        $metadata: jc(e)
                                     })]
                             }
                         }))
                     }))
                 },
-                Ic = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch", "BadRequestException"],
-                Dc = function(e) {
-                    return Ic.includes(e)
+                Dc = ["AuthFailure", "InvalidSignatureException", "RequestExpired", "RequestInTheFuture", "RequestTimeTooSkewed", "SignatureDoesNotMatch", "BadRequestException"],
+                Lc = function(e) {
+                    return Dc.includes(e)
                 },
-                Lc = function(e, t, n, r) {
+                Sc = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -60444,15 +60447,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                Sc = function(e, t) {
+                kc = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -60519,214 +60522,214 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                kc = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException"],
-                Cc = ["TimeoutError", "RequestTimeout", "RequestTimeoutException"],
-                Ec = function(e, t) {
-                    return 429 === e || kc.includes(t)
+                Cc = ["BandwidthLimitExceeded", "EC2ThrottledException", "LimitExceededException", "PriorRequestNotComplete", "ProvisionedThroughputExceededException", "RequestLimitExceeded", "RequestThrottled", "RequestThrottledException", "SlowDown", "ThrottledException", "Throttling", "ThrottlingException", "TooManyRequestsException"],
+                Ec = ["TimeoutError", "RequestTimeout", "RequestTimeoutException"],
+                Tc = function(e, t) {
+                    return 429 === e || Cc.includes(t)
                 },
-                Tc = function(e) {
+                Ac = function(e) {
                     return "Network error" === (null === e || void 0 === e ? void 0 : e.name)
                 },
-                Ac = function(e, t) {
-                    return [500, 502, 503, 504].includes(e) || Cc.includes(t)
+                zc = function(e, t) {
+                    return [500, 502, 503, 504].includes(e) || Ec.includes(t)
                 },
-                zc = 3e5;
+                Oc = 3e5;
             ! function(e) {
                 e.WebUnknown = "0", e.React = "1", e.NextJs = "2", e.Angular = "3", e.VueJs = "4", e.Nuxt = "5", e.Svelte = "6", e.ServerSideUnknown = "100", e.ReactSSR = "101", e.NextJsSSR = "102", e.AngularSSR = "103", e.VueJsSSR = "104", e.NuxtSSR = "105", e.SvelteSSR = "106", e.ReactNative = "201", e.Expo = "202"
-            }(Il || (Il = {})),
-            function(e) {
-                e.API = "api", e.Auth = "auth", e.Analytics = "analytics", e.DataStore = "datastore", e.Geo = "geo", e.InAppMessaging = "inappmessaging", e.Interactions = "interactions", e.Predictions = "predictions", e.PubSub = "pubsub", e.PushNotification = "pushnotification", e.Storage = "storage"
             }(Dl || (Dl = {})),
             function(e) {
-                e.Record = "1", e.UpdateEndpoint = "2"
+                e.API = "api", e.Auth = "auth", e.Analytics = "analytics", e.DataStore = "datastore", e.Geo = "geo", e.InAppMessaging = "inappmessaging", e.Interactions = "interactions", e.Predictions = "predictions", e.PubSub = "pubsub", e.PushNotification = "pushnotification", e.Storage = "storage"
             }(Ll || (Ll = {})),
             function(e) {
-                e.GraphQl = "1", e.Get = "2", e.Post = "3", e.Put = "4", e.Patch = "5", e.Del = "6", e.Head = "7"
+                e.Record = "1", e.UpdateEndpoint = "2"
             }(Sl || (Sl = {})),
             function(e) {
-                e.FederatedSignIn = "30"
+                e.GraphQl = "1", e.Get = "2", e.Post = "3", e.Put = "4", e.Patch = "5", e.Del = "6", e.Head = "7"
             }(kl || (kl = {})),
             function(e) {
-                e.Subscribe = "1", e.GraphQl = "2"
+                e.FederatedSignIn = "30"
             }(Cl || (Cl = {})),
             function(e) {
-                e.None = "0"
+                e.Subscribe = "1", e.GraphQl = "2"
             }(El || (El = {})),
             function(e) {
                 e.None = "0"
             }(Tl || (Tl = {})),
             function(e) {
                 e.None = "0"
             }(Al || (Al = {})),
             function(e) {
-                e.Convert = "1", e.Identify = "2", e.Interpret = "3"
+                e.None = "0"
             }(zl || (zl = {})),
             function(e) {
-                e.Subscribe = "1"
+                e.Convert = "1", e.Identify = "2", e.Interpret = "3"
             }(Ol || (Ol = {})),
             function(e) {
-                e.None = "0"
+                e.Subscribe = "1"
             }(_l || (_l = {})),
             function(e) {
+                e.None = "0"
+            }(Ul || (Ul = {})),
+            function(e) {
                 e.Put = "1", e.Get = "2", e.List = "3", e.Copy = "4", e.Remove = "5", e.GetProperties = "6"
-            }(Ul || (Ul = {}));
-            var Oc = "5.3.3",
-                _c = function() {
+            }(Pl || (Pl = {}));
+            var _c = "5.3.3",
+                Uc = function() {
                     return "undefined" !== typeof n.g
                 },
-                Uc = function() {
+                Pc = function() {
                     return "undefined" !== typeof window
                 },
-                Pc = function() {
+                Rc = function() {
                     return "undefined" !== typeof document
                 },
-                Rc = function() {
+                Fc = function() {
                     return "undefined" !== typeof process
                 },
-                Fc = function(e, t) {
+                Bc = function(e, t) {
                     return !!Object.keys(e).find((function(e) {
                         return e.startsWith(t)
                     }))
                 };
-            var Bc, Yc = [{
-                platform: Il.Expo,
+            var Yc, Qc = [{
+                platform: Dl.Expo,
                 detectionMethod: function() {
-                    return _c() && "undefined" !== typeof n.g.expo
+                    return Uc() && "undefined" !== typeof n.g.expo
                 }
             }, {
-                platform: Il.ReactNative,
+                platform: Dl.ReactNative,
                 detectionMethod: function() {
                     return "undefined" !== typeof navigator && "undefined" !== typeof navigator.product && "ReactNative" === navigator.product
                 }
             }, {
-                platform: Il.NextJs,
+                platform: Dl.NextJs,
                 detectionMethod: function() {
-                    return Uc() && window.next && "object" === typeof window.next
+                    return Pc() && window.next && "object" === typeof window.next
                 }
             }, {
-                platform: Il.Nuxt,
+                platform: Dl.Nuxt,
                 detectionMethod: function() {
-                    return Uc() && (void 0 !== window.__NUXT__ || void 0 !== window.$nuxt)
+                    return Pc() && (void 0 !== window.__NUXT__ || void 0 !== window.$nuxt)
                 }
             }, {
-                platform: Il.Angular,
+                platform: Dl.Angular,
                 detectionMethod: function() {
-                    var e = Boolean(Pc() && document.querySelector("[ng-version]")),
-                        t = Boolean(Uc() && "undefined" !== typeof window.ng);
+                    var e = Boolean(Rc() && document.querySelector("[ng-version]")),
+                        t = Boolean(Pc() && "undefined" !== typeof window.ng);
                     return e || t
                 }
             }, {
-                platform: Il.React,
+                platform: Dl.React,
                 detectionMethod: function() {
                     var e = function(e) {
                         return e.startsWith("_react") || e.startsWith("__react")
                     };
-                    return Pc() && Array.from(document.querySelectorAll("[id]")).some((function(t) {
+                    return Rc() && Array.from(document.querySelectorAll("[id]")).some((function(t) {
                         return Object.keys(t).find(e)
                     }))
                 }
             }, {
-                platform: Il.VueJs,
+                platform: Dl.VueJs,
                 detectionMethod: function() {
-                    return Uc() && Fc(window, "__VUE")
+                    return Pc() && Bc(window, "__VUE")
                 }
             }, {
-                platform: Il.Svelte,
+                platform: Dl.Svelte,
                 detectionMethod: function() {
-                    return Uc() && Fc(window, "__SVELTE")
+                    return Pc() && Bc(window, "__SVELTE")
                 }
             }, {
-                platform: Il.WebUnknown,
+                platform: Dl.WebUnknown,
                 detectionMethod: function() {
-                    return Uc()
+                    return Pc()
                 }
             }, {
-                platform: Il.NextJsSSR,
+                platform: Dl.NextJsSSR,
                 detectionMethod: function() {
-                    return _c() && (Fc(n.g, "__next") || Fc(n.g, "__NEXT"))
+                    return Uc() && (Bc(n.g, "__next") || Bc(n.g, "__NEXT"))
                 }
             }, {
-                platform: Il.NuxtSSR,
+                platform: Dl.NuxtSSR,
                 detectionMethod: function() {
-                    return _c() && "undefined" !== typeof n.g.__NUXT_PATHS__
+                    return Uc() && "undefined" !== typeof n.g.__NUXT_PATHS__
                 }
             }, {
-                platform: Il.ReactSSR,
+                platform: Dl.ReactSSR,
                 detectionMethod: function() {
-                    return Rc() && !!Object.keys({
+                    return Fc() && !!Object.keys({
                         NODE_ENV: "production",
                         PUBLIC_URL: "/api/react",
                         WDS_SOCKET_HOST: void 0,
                         WDS_SOCKET_PATH: void 0,
                         WDS_SOCKET_PORT: void 0,
                         FAST_REFRESH: !0
                     }).find((function(e) {
                         return e.includes("react")
                     }))
                 }
             }, {
-                platform: Il.VueJsSSR,
+                platform: Dl.VueJsSSR,
                 detectionMethod: function() {
-                    return _c() && Fc(n.g, "__VUE")
+                    return Uc() && Bc(n.g, "__VUE")
                 }
             }, {
-                platform: Il.AngularSSR,
+                platform: Dl.AngularSSR,
                 detectionMethod: function() {
                     var e;
-                    return Rc() && (null === (e = {
+                    return Fc() && (null === (e = {
                         NODE_ENV: "production",
                         PUBLIC_URL: "/api/react",
                         WDS_SOCKET_HOST: void 0,
                         WDS_SOCKET_PATH: void 0,
                         WDS_SOCKET_PORT: void 0,
                         FAST_REFRESH: !0
                     }.npm_lifecycle_script) || void 0 === e ? void 0 : e.startsWith("ng ")) || !1
                 }
             }, {
-                platform: Il.SvelteSSR,
+                platform: Dl.SvelteSSR,
                 detectionMethod: function() {
-                    return Rc() && !!Object.keys({
+                    return Fc() && !!Object.keys({
                         NODE_ENV: "production",
                         PUBLIC_URL: "/api/react",
                         WDS_SOCKET_HOST: void 0,
                         WDS_SOCKET_PATH: void 0,
                         WDS_SOCKET_PORT: void 0,
                         FAST_REFRESH: !0
                     }).find((function(e) {
                         return e.includes("svelte")
                     }))
                 }
             }];
-            var Qc = [],
-                Gc = !1,
-                Wc = function() {
-                    return Bc || (Bc = function() {
+            var Gc = [],
+                Wc = !1,
+                Hc = function() {
+                    return Yc || (Yc = function() {
                         var e;
-                        return (null === (e = Yc.find((function(e) {
+                        return (null === (e = Qc.find((function(e) {
                             return e.detectionMethod()
-                        }))) || void 0 === e ? void 0 : e.platform) || Il.ServerSideUnknown
-                    }(), Qc.forEach((function(e) {
+                        }))) || void 0 === e ? void 0 : e.platform) || Dl.ServerSideUnknown
+                    }(), Gc.forEach((function(e) {
                         return e()
-                    })), Vc(Il.ServerSideUnknown, 10), Vc(Il.WebUnknown, 10)), Bc
+                    })), Zc(Dl.ServerSideUnknown, 10), Zc(Dl.WebUnknown, 10)), Yc
                 },
-                Hc = function(e) {
-                    Qc.push(e)
+                Vc = function(e) {
+                    Gc.push(e)
                 };
 
-            function Vc(e, t) {
-                Bc !== e || Gc || setTimeout((function() {
-                    Bc = void 0, Gc = !0, setTimeout(Wc, 1e3)
+            function Zc(e, t) {
+                Yc !== e || Wc || setTimeout((function() {
+                    Yc = void 0, Wc = !0, setTimeout(Hc, 1e3)
                 }), t)
             }
-            var Zc, qc = function(e, t) {
+            var qc, Jc = function(e, t) {
                     var n = "function" === typeof Symbol && e[Symbol.iterator];
                     if (!n) return e;
                     var r, o, i = n.call(e),
                         a = [];
                     try {
                         for (;
                             (void 0 === t || t-- > 0) && !(r = i.next()).done;) a.push(r.value)
@@ -60739,52 +60742,52 @@
                             r && !r.done && (n = i.return) && n.call(i)
                         } finally {
                             if (o) throw o.error
                         }
                     }
                     return a
                 },
-                Jc = "aws-amplify",
-                Kc = new(function() {
+                Kc = "aws-amplify",
+                Xc = new(function() {
                     function e() {
-                        this.userAgent = "".concat(Jc, "/").concat(Oc)
+                        this.userAgent = "".concat(Kc, "/").concat(_c)
                     }
                     return Object.defineProperty(e.prototype, "framework", {
                         get: function() {
-                            return Wc()
+                            return Hc()
                         },
                         enumerable: !1,
                         configurable: !0
                     }), Object.defineProperty(e.prototype, "isReactNative", {
                         get: function() {
-                            return this.framework === Il.ReactNative || this.framework === Il.Expo
+                            return this.framework === Dl.ReactNative || this.framework === Dl.Expo
                         },
                         enumerable: !1,
                         configurable: !0
                     }), e.prototype.observeFrameworkChanges = function(e) {
-                        Hc(e)
+                        Vc(e)
                     }, e
                 }()),
-                Xc = function(e) {
+                $c = function(e) {
                     return function(e) {
                         var t = void 0 === e ? {} : e,
                             n = t.category,
                             r = t.action,
                             o = (t.framework, [
-                                [Jc, Oc]
+                                [Kc, _c]
                             ]);
-                        return n && o.push([n, r]), o.push(["framework", Wc()]), o
+                        return n && o.push([n, r]), o.push(["framework", Hc()]), o
                     }(e).map((function(e) {
-                        var t = qc(e, 2),
+                        var t = Jc(e, 2),
                             n = t[0],
                             r = t[1];
                         return "".concat(n, "/").concat(r)
                     })).join(" ")
                 },
-                $c = function(e, t, n, r) {
+                ed = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -60803,15 +60806,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                ed = function(e, t) {
+                td = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -60878,81 +60881,81 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                td = dc(mc, [function() {
+                nd = pc(vc, [function() {
                     return function(e, t) {
                         return function(t) {
-                            return $c(this, void 0, void 0, (function() {
-                                return ed(this, (function(n) {
+                            return ed(this, void 0, void 0, (function() {
+                                return td(this, (function(n) {
                                     return t.headers["cache-control"] = "no-store", [2, e(t)]
                                 }))
                             }))
                         }
                     }
                 }]),
-                nd = {
+                rd = {
                     service: "cognito-identity",
                     endpointResolver: function(e) {
                         var t = e.region;
                         return {
-                            url: new URL("https://cognito-identity.".concat(t, ".").concat(rc(t)))
+                            url: new URL("https://cognito-identity.".concat(t, ".").concat(oc(t)))
                         }
                     },
-                    retryDecider: (Zc = xc, function(e, t) {
-                        return Lc(void 0, void 0, void 0, (function() {
+                    retryDecider: (qc = Nc, function(e, t) {
+                        return Sc(void 0, void 0, void 0, (function() {
                             var n, r, o, i;
-                            return Sc(this, (function(a) {
+                            return kc(this, (function(a) {
                                 switch (a.label) {
                                     case 0:
                                         return null === t || void 0 === t ? [3, 1] : (r = t, [3, 3]);
                                     case 1:
-                                        return [4, Zc(e)];
+                                        return [4, qc(e)];
                                     case 2:
                                         r = a.sent(), a.label = 3;
                                     case 3:
-                                        return n = (null !== (i = r) && void 0 !== i ? i : {}).name, o = null === e || void 0 === e ? void 0 : e.statusCode, [2, Tc(t) || Ec(o, n) || Dc(n) || Ac(o, n)]
+                                        return n = (null !== (i = r) && void 0 !== i ? i : {}).name, o = null === e || void 0 === e ? void 0 : e.statusCode, [2, Ac(t) || Tc(o, n) || Lc(n) || zc(o, n)]
                                 }
                             }))
                         }))
                     }),
                     computeDelay: function(e) {
-                        var t = Nl(zc)(e);
-                        return !1 === t ? zc : t
+                        var t = Il(Oc)(e);
+                        return !1 === t ? Oc : t
                     },
-                    userAgentValue: Xc()
+                    userAgentValue: $c()
                 };
-            Hc((function() {
-                nd.userAgentValue = Xc()
+            Vc((function() {
+                rd.userAgentValue = $c()
             }));
-            var rd = function(e) {
+            var od = function(e) {
                     return {
                         "content-type": "application/x-amz-json-1.1",
                         "x-amz-target": "AWSCognitoIdentityService.".concat(e)
                     }
                 },
-                od = function(e, t, n) {
+                id = function(e, t, n) {
                     return {
                         headers: t,
                         url: e.url,
                         body: n,
                         method: "POST"
                     }
                 },
-                id = function() {
-                    return id = Object.assign || function(e) {
+                ad = function() {
+                    return ad = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, id.apply(this, arguments)
+                    }, ad.apply(this, arguments)
                 },
-                ad = function(e, t, n, r) {
+                sd = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -60971,15 +60974,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                sd = function(e, t) {
+                ud = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -61046,36 +61049,36 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                ud = function(e, t, n, r) {
+                ld = function(e, t, n, r) {
                     return function(o, i) {
-                        return ad(void 0, void 0, void 0, (function() {
+                        return sd(void 0, void 0, void 0, (function() {
                             var a, s, u, l;
-                            return sd(this, (function(c) {
+                            return ud(this, (function(c) {
                                 switch (c.label) {
                                     case 0:
-                                        return [4, (a = id(id({}, r), o)).endpointResolver({
+                                        return [4, (a = ad(ad({}, r), o)).endpointResolver({
                                             region: a.region
                                         })];
                                     case 1:
-                                        return s = c.sent(), u = t(i, s), [4, e(u, id({}, a))];
+                                        return s = c.sent(), u = t(i, s), [4, e(u, ad({}, a))];
                                     case 2:
                                         return l = c.sent(), [4, n(l)];
                                     case 3:
                                         return [2, c.sent()]
                                 }
                             }))
                         }))
                     }
                 },
-                ld = function(e, t, n, r) {
+                cd = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -61094,15 +61097,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                cd = function(e, t) {
+                dd = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -61169,38 +61172,38 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                dd = ud(td, (function(e, t) {
-                    var n = rd("GetId"),
+                pd = ld(nd, (function(e, t) {
+                    var n = od("GetId"),
                         r = JSON.stringify(e);
-                    return od(t, n, r)
+                    return id(t, n, r)
                 }), (function(e) {
-                    return ld(void 0, void 0, void 0, (function() {
-                        return cd(this, (function(t) {
+                    return cd(void 0, void 0, void 0, (function() {
+                        return dd(this, (function(t) {
                             switch (t.label) {
                                 case 0:
-                                    return e.statusCode >= 300 ? [4, xc(e)] : [3, 2];
+                                    return e.statusCode >= 300 ? [4, Nc(e)] : [3, 2];
                                 case 1:
                                     throw t.sent();
                                 case 2:
-                                    return [4, Nc(e)];
+                                    return [4, Ic(e)];
                                 case 3:
                                     return [2, {
                                         IdentityId: t.sent().IdentityId,
-                                        $metadata: Mc(e)
+                                        $metadata: jc(e)
                                     }]
                             }
                         }))
                     }))
-                }), nd),
-                pd = function(e, t, n, r) {
+                }), rd),
+                fd = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -61219,15 +61222,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                fd = function(e, t) {
+                hd = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -61294,56 +61297,56 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                hd = function(e) {
+                gd = function(e) {
                     return void 0 === e && (e = {}), {
                         AccessKeyId: e.AccessKeyId,
                         SecretKey: e.SecretKey,
                         SessionToken: e.SessionToken,
                         Expiration: new Date(1e3 * e.Expiration)
                     }
                 },
-                gd = ud(td, (function(e, t) {
-                    var n = rd("GetCredentialsForIdentity"),
+                yd = ld(nd, (function(e, t) {
+                    var n = od("GetCredentialsForIdentity"),
                         r = JSON.stringify(e);
-                    return od(t, n, r)
+                    return id(t, n, r)
                 }), (function(e) {
-                    return pd(void 0, void 0, void 0, (function() {
+                    return fd(void 0, void 0, void 0, (function() {
                         var t;
-                        return fd(this, (function(n) {
+                        return hd(this, (function(n) {
                             switch (n.label) {
                                 case 0:
-                                    return e.statusCode >= 300 ? [4, xc(e)] : [3, 2];
+                                    return e.statusCode >= 300 ? [4, Nc(e)] : [3, 2];
                                 case 1:
                                     throw n.sent();
                                 case 2:
-                                    return [4, Nc(e)];
+                                    return [4, Ic(e)];
                                 case 3:
                                     return [2, {
                                         IdentityId: (t = n.sent()).IdentityId,
-                                        Credentials: hd(t.Credentials),
-                                        $metadata: Mc(e)
+                                        Credentials: gd(t.Credentials),
+                                        $metadata: jc(e)
                                     }]
                             }
                         }))
                     }))
-                }), nd),
-                yd = function() {
-                    return yd = Object.assign || function(e) {
+                }), rd),
+                md = function() {
+                    return md = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, yd.apply(this, arguments)
+                    }, md.apply(this, arguments)
                 },
-                md = new ol("Parser"),
-                vd = function(e) {
+                vd = new il("Parser"),
+                Md = function(e) {
                     var t, n = {};
                     if (e.aws_mobile_analytics_app_id) {
                         var r = {
                             AWSPinpoint: {
                                 appId: e.aws_mobile_analytics_app_id,
                                 region: e.aws_mobile_analytics_app_region
                             }
@@ -61360,28 +61363,28 @@
                         signUpVerificationMethod: e.aws_cognito_sign_up_verification_method || "code"
                     }), t = e.aws_user_files_s3_bucket ? {
                         AWSS3: {
                             bucket: e.aws_user_files_s3_bucket,
                             region: e.aws_user_files_s3_bucket_region,
                             dangerouslyConnectToHttpEndpointForTesting: e.aws_user_files_s3_dangerously_connect_to_http_endpoint_for_testing
                         }
-                    } : e ? e.Storage || e : {}, e.Logging && (n.Logging = yd(yd({}, e.Logging), {
+                    } : e ? e.Storage || e : {}, e.Logging && (n.Logging = md(md({}, e.Logging), {
                         region: e.aws_project_region
                     })), e.geo && (n.Geo = Object.assign({}, e.geo), e.geo.amazon_location_service && (n.Geo = {
                         AmazonLocationService: e.geo.amazon_location_service
-                    })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), md.debug("parse config", e, "to amplifyconfig", n), n
+                    })), n.Analytics = Object.assign({}, n.Analytics, e.Analytics), n.Auth = Object.assign({}, n.Auth, e.Auth), n.Storage = Object.assign({}, t), n.Logging = Object.assign({}, n.Logging, e.Logging), vd.debug("parse config", e, "to amplifyconfig", n), n
                 },
-                Md = function() {
-                    return Md = Object.assign || function(e) {
+                jd = function() {
+                    return jd = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, Md.apply(this, arguments)
+                    }, jd.apply(this, arguments)
                 },
-                jd = function(e, t, n, r) {
+                bd = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(o, i) {
                         function a(e) {
                             try {
                                 u(r.next(e))
                             } catch (t) {
                                 i(t)
                             }
@@ -61400,15 +61403,15 @@
                             e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                 e(t)
                             }))).then(a, s)
                         }
                         u((r = r.apply(e, t || [])).next())
                     }))
                 },
-                bd = function(e, t) {
+                wd = function(e, t) {
                     var n, r, o, i, a = {
                         label: 0,
                         sent: function() {
                             if (1 & o[0]) throw o[1];
                             return o[1]
                         },
                         trys: [],
@@ -61475,39 +61478,39 @@
                                     value: s[0] ? s[1] : void 0,
                                     done: !0
                                 }
                             }([s, u])
                         }
                     }
                 },
-                wd = new ol("Credentials"),
-                xd = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-                Nd = function() {
+                xd = new il("Credentials"),
+                Nd = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+                Id = function() {
                     function e(e) {
-                        this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = ql.refreshGoogleToken, this._refreshHandlers.facebook = Jl.refreshFacebookToken
+                        this._gettingCredPromise = null, this._refreshHandlers = {}, this.Auth = void 0, this.configure(e), this._refreshHandlers.google = Jl.refreshGoogleToken, this._refreshHandlers.facebook = Kl.refreshFacebookToken
                     }
                     return e.prototype.getModuleName = function() {
                         return "Credentials"
                     }, e.prototype.getCredSource = function() {
                         return this._credentials_source
                     }, e.prototype.configure = function(e) {
                         if (!e) return this._config || {};
                         this._config = Object.assign({}, this._config, e);
                         var t, n, r, o = this._config.refreshHandlers;
-                        return o && (this._refreshHandlers = Md(Md({}, this._refreshHandlers), o)), this._storage = this._config.storage, this._storage || (this._storage = (new hl).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), t = "credentials_configured", n = null, r = "Credentials has been configured successfully", dl.dispatch("core", {
+                        return o && (this._refreshHandlers = jd(jd({}, this._refreshHandlers), o)), this._storage = this._config.storage, this._storage || (this._storage = (new gl).getStorage()), this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), t = "credentials_configured", n = null, r = "Credentials has been configured successfully", pl.dispatch("core", {
                             event: t,
                             data: n,
                             message: r
-                        }, "Credentials", xd), this._config
+                        }, "Credentials", Nd), this._config
                     }, e.prototype.get = function() {
-                        return wd.debug("getting credentials"), this._pickupCredentials()
+                        return xd.debug("getting credentials"), this._pickupCredentials()
                     }, e.prototype._getCognitoIdentityIdStorageKey = function(e) {
                         return "".concat("CognitoIdentityId-").concat(e)
                     }, e.prototype._pickupCredentials = function() {
-                        return wd.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? wd.debug("getting old cred promise") : (wd.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
+                        return xd.debug("picking up credentials"), this._gettingCredPromise && this._gettingCredPromise.isPending() ? xd.debug("getting old cred promise") : (xd.debug("getting new cred promise"), this._gettingCredPromise = function(e) {
                             if (e.isResolved) return e;
                             var t = !0,
                                 n = !1,
                                 r = !1,
                                 o = e.then((function(e) {
                                     return r = !0, t = !1, e
                                 }), (function(e) {
@@ -61518,165 +61521,165 @@
                             }, o.isPending = function() {
                                 return t
                             }, o.isRejected = function() {
                                 return n
                             }, o
                         }(this._keepAlive())), this._gettingCredPromise
                     }, e.prototype._keepAlive = function() {
-                        return jd(this, void 0, void 0, (function() {
+                        return bd(this, void 0, void 0, (function() {
                             var e, t, n, r, o, i, a;
-                            return bd(this, (function(s) {
+                            return wd(this, (function(s) {
                                 switch (s.label) {
                                     case 0:
-                                        if (wd.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return wd.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
-                                        if (wd.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? $l.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
+                                        if (xd.debug("checking if credentials exists and not expired"), (e = this._credentials) && !this._isExpired(e) && !this._isPastTTL()) return xd.debug("credentials not changed and not expired, directly return"), [2, Promise.resolve(e)];
+                                        if (xd.debug("need to get a new credential or refresh the existing one"), t = this.Auth, !(n = void 0 === t ? ec.Auth : t) || "function" !== typeof n.currentUserCredentials) return [2, this._setCredentialsForGuest()];
                                         if (this._isExpired(e) || !this._isPastTTL()) return [3, 6];
-                                        wd.debug("ttl has passed but token is not yet expired"), s.label = 1;
+                                        xd.debug("ttl has passed but token is not yet expired"), s.label = 1;
                                     case 1:
                                         return s.trys.push([1, 5, , 6]), [4, n.currentUserPoolUser()];
                                     case 2:
                                         return r = s.sent(), [4, n.currentSession()];
                                     case 3:
                                         return o = s.sent(), i = o.refreshToken, [4, new Promise((function(e, t) {
                                             r.refreshSession(i, (function(n, r) {
                                                 return n ? t(n) : e(r)
                                             }))
                                         }))];
                                     case 4:
                                         return s.sent(), [3, 6];
                                     case 5:
-                                        return a = s.sent(), wd.debug("Error attempting to refreshing the session", a), [3, 6];
+                                        return a = s.sent(), xd.debug("Error attempting to refreshing the session", a), [3, 6];
                                     case 6:
                                         return [2, n.currentUserCredentials()]
                                 }
                             }))
                         }))
                     }, e.prototype.refreshFederatedToken = function(e) {
-                        wd.debug("Getting federated credentials");
+                        xd.debug("Getting federated credentials");
                         var t = e.provider,
                             n = e.user,
                             r = e.token,
                             o = e.identity_id,
                             i = e.expires_at;
                         i = 1970 === new Date(i).getFullYear() ? 1e3 * i : i;
                         var a = this;
-                        return wd.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (wd.debug("token not expired"), this._setCredentialsFromFederation({
+                        return xd.debug("checking if federated jwt token expired"), i > (new Date).getTime() ? (xd.debug("token not expired"), this._setCredentialsFromFederation({
                             provider: t,
                             token: r,
                             user: n,
                             identity_id: o,
                             expires_at: i
-                        })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (wd.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
+                        })) : a._refreshHandlers[t] && "function" === typeof a._refreshHandlers[t] ? (xd.debug("getting refreshed jwt token from federation provider"), this._providerRefreshWithRetry({
                             refreshHandler: a._refreshHandlers[t],
                             provider: t,
                             user: n
-                        })) : (wd.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
+                        })) : (xd.debug("no refresh handler for provider:", t), this.clear(), Promise.reject("no refresh handler for provider"))
                     }, e.prototype._providerRefreshWithRetry = function(e) {
                         var t = this,
                             n = e.refreshHandler,
                             r = e.provider,
                             o = e.user;
-                        return Pl(n, [], 1e4).then((function(e) {
-                            return wd.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
+                        return Rl(n, [], 1e4).then((function(e) {
+                            return xd.debug("refresh federated token sucessfully", e), t._setCredentialsFromFederation({
                                 provider: r,
                                 token: e.token,
                                 user: o,
                                 identity_id: e.identity_id,
                                 expires_at: e.expires_at
                             })
                         })).catch((function(e) {
-                            return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), wd.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
+                            return "string" === typeof e && 0 === e.toLowerCase().lastIndexOf("network error", e.length) || t.clear(), xd.debug("refresh federated token failed", e), Promise.reject("refreshing federation token failed: " + e)
                         }))
                     }, e.prototype._isExpired = function(e) {
-                        if (!e) return wd.debug("no credentials for expiration check"), !0;
-                        wd.debug("are these credentials expired?", e);
+                        if (!e) return xd.debug("no credentials for expiration check"), !0;
+                        xd.debug("are these credentials expired?", e);
                         var t = Date.now();
                         return e.expiration.getTime() <= t
                     }, e.prototype._isPastTTL = function() {
                         return this._nextCredentialsRefresh <= Date.now()
                     }, e.prototype._setCredentialsForGuest = function() {
                         var e;
-                        return jd(this, void 0, void 0, (function() {
+                        return bd(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s, u, l, c, d = this;
-                            return bd(this, (function(p) {
+                            return wd(this, (function(p) {
                                 switch (p.label) {
                                     case 0:
-                                        return wd.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, vd(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (wd.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (wd.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
+                                        return xd.debug("setting credentials for guest"), (null === (e = this._config) || void 0 === e ? void 0 : e.identityPoolId) || (this._config = Object.assign({}, this._config, Md(this._config || {}).Auth)), t = this._config, n = t.identityPoolId, r = t.region, o = t.mandatorySignIn, i = t.identityPoolRegion, o ? [2, Promise.reject("cannot get guest credentials when mandatory signin enabled")] : n ? i || r ? (s = this, [4, this._getGuestIdentityId()]) : (xd.debug("region is not configured for getting the credentials"), [2, Promise.reject("region is not configured for getting the credentials")]) : (xd.debug("No Cognito Identity pool provided for unauthenticated access"), [2, Promise.reject("No Cognito Identity pool provided for unauthenticated access")]);
                                     case 1:
                                         return a = s._identityId = p.sent(), u = {
                                             region: null !== i && void 0 !== i ? i : r
                                         }, l = function() {
-                                            return jd(d, void 0, void 0, (function() {
+                                            return bd(d, void 0, void 0, (function() {
                                                 var e, t;
-                                                return bd(this, (function(r) {
+                                                return wd(this, (function(r) {
                                                     switch (r.label) {
                                                         case 0:
-                                                            return a ? [3, 2] : [4, dd(u, {
+                                                            return a ? [3, 2] : [4, pd(u, {
                                                                 IdentityPoolId: n
                                                             })];
                                                         case 1:
                                                             e = r.sent().IdentityId, this._identityId = e, r.label = 2;
                                                         case 2:
-                                                            return [4, gd(u, {
+                                                            return [4, yd(u, {
                                                                 IdentityId: this._identityId
                                                             })];
                                                         case 3:
                                                             return t = r.sent().Credentials, [2, {
                                                                 identityId: this._identityId,
                                                                 accessKeyId: t.AccessKeyId,
                                                                 secretAccessKey: t.SecretKey,
                                                                 sessionToken: t.SessionToken,
                                                                 expiration: t.Expiration
                                                             }]
                                                     }
                                                 }))
                                             }))
                                         }, c = l().catch((function(e) {
-                                            return jd(d, void 0, void 0, (function() {
-                                                return bd(this, (function(t) {
+                                            return bd(d, void 0, void 0, (function() {
+                                                return wd(this, (function(t) {
                                                     throw e
                                                 }))
                                             }))
                                         })), [2, this._loadCredentials(c, "guest", !1, null).then((function(e) {
                                             return e
                                         })).catch((function(e) {
-                                            return jd(d, void 0, void 0, (function() {
+                                            return bd(d, void 0, void 0, (function() {
                                                 var t, r = this;
-                                                return bd(this, (function(o) {
+                                                return wd(this, (function(o) {
                                                     switch (o.label) {
                                                         case 0:
-                                                            return "ResourceNotFoundException" !== e.name || e.message !== "Identity '".concat(a, "' not found.") ? [3, 2] : (wd.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
+                                                            return "ResourceNotFoundException" !== e.name || e.message !== "Identity '".concat(a, "' not found.") ? [3, 2] : (xd.debug("Failed to load guest credentials"), [4, this._removeGuestIdentityId()]);
                                                         case 1:
                                                             return o.sent(), t = function() {
-                                                                return jd(r, void 0, void 0, (function() {
+                                                                return bd(r, void 0, void 0, (function() {
                                                                     var e, t;
-                                                                    return bd(this, (function(r) {
+                                                                    return wd(this, (function(r) {
                                                                         switch (r.label) {
                                                                             case 0:
-                                                                                return [4, dd(u, {
+                                                                                return [4, pd(u, {
                                                                                     IdentityPoolId: n
                                                                                 })];
                                                                             case 1:
-                                                                                return e = r.sent().IdentityId, this._identityId = e, [4, gd(u, {
+                                                                                return e = r.sent().IdentityId, this._identityId = e, [4, yd(u, {
                                                                                     IdentityId: e
                                                                                 })];
                                                                             case 2:
                                                                                 return t = r.sent().Credentials, [2, {
                                                                                     identityId: e,
                                                                                     accessKeyId: t.AccessKeyId,
                                                                                     secretAccessKey: t.SecretKey,
                                                                                     sessionToken: t.SessionToken,
                                                                                     expiration: t.Expiration
                                                                                 }]
                                                                         }
                                                                     }))
                                                                 }))
                                                             }, c = t().catch((function(e) {
-                                                                return jd(r, void 0, void 0, (function() {
-                                                                    return bd(this, (function(t) {
+                                                                return bd(r, void 0, void 0, (function() {
+                                                                    return wd(this, (function(t) {
                                                                         throw e
                                                                     }))
                                                                 }))
                                                             })), [2, this._loadCredentials(c, "guest", !1, null)];
                                                         case 2:
                                                             return [2, e]
                                                     }
@@ -61700,221 +61703,221 @@
                         if (!i) return Promise.reject("You must specify a federated provider");
                         var a = {};
                         a[i] = r;
                         var s = this._config,
                             u = s.identityPoolId,
                             l = s.region,
                             c = s.identityPoolRegion;
-                        if (!u) return wd.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                        if (!c && !l) return wd.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                        if (!u) return xd.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                        if (!c && !l) return xd.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
                         var d = {
                                 region: null !== c && void 0 !== c ? c : l
                             },
-                            p = jd(t, void 0, void 0, (function() {
+                            p = bd(t, void 0, void 0, (function() {
                                 var e, t;
-                                return bd(this, (function(n) {
+                                return wd(this, (function(n) {
                                     switch (n.label) {
                                         case 0:
-                                            return o ? [3, 2] : [4, dd(d, {
+                                            return o ? [3, 2] : [4, pd(d, {
                                                 IdentityPoolId: u,
                                                 Logins: a
                                             })];
                                         case 1:
                                             e = n.sent().IdentityId, o = e, n.label = 2;
                                         case 2:
-                                            return [4, gd(d, {
+                                            return [4, yd(d, {
                                                 IdentityId: o,
                                                 Logins: a
                                             })];
                                         case 3:
                                             return t = n.sent().Credentials, [2, {
                                                 identityId: o,
                                                 accessKeyId: t.AccessKeyId,
                                                 secretAccessKey: t.SecretKey,
                                                 sessionToken: t.SessionToken,
                                                 expiration: t.Expiration
                                             }]
                                     }
                                 }))
                             })).catch((function(e) {
-                                return jd(t, void 0, void 0, (function() {
-                                    return bd(this, (function(t) {
+                                return bd(t, void 0, void 0, (function() {
+                                    return wd(this, (function(t) {
                                         throw e
                                     }))
                                 }))
                             }));
                         return this._loadCredentials(p, "federated", !0, e)
                     }, e.prototype._setCredentialsFromSession = function(e) {
                         var t = this;
-                        wd.debug("set credentials from session");
+                        xd.debug("set credentials from session");
                         var n = e.getIdToken().getJwtToken(),
                             r = this._config,
                             o = r.region,
                             i = r.userPoolId,
                             a = r.identityPoolId,
                             s = r.identityPoolRegion;
-                        if (!a) return wd.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
-                        if (!s && !o) return wd.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
+                        if (!a) return xd.debug("No Cognito Federated Identity pool provided"), Promise.reject("No Cognito Federated Identity pool provided");
+                        if (!s && !o) return xd.debug("region is not configured for getting the credentials"), Promise.reject("region is not configured for getting the credentials");
                         var u = {};
                         u["cognito-idp." + o + ".amazonaws.com/" + i] = n;
                         var l = {
                                 region: null !== s && void 0 !== s ? s : o
                             },
-                            c = jd(t, void 0, void 0, (function() {
+                            c = bd(t, void 0, void 0, (function() {
                                 var e, t, n, r, o, i, s, c, d, p;
-                                return bd(this, (function(f) {
+                                return wd(this, (function(f) {
                                     switch (f.label) {
                                         case 0:
                                             return [4, this._getGuestIdentityId()];
                                         case 1:
-                                            return (e = f.sent()) ? [3, 3] : [4, dd(l, {
+                                            return (e = f.sent()) ? [3, 3] : [4, pd(l, {
                                                 IdentityPoolId: a,
                                                 Logins: u
                                             })];
                                         case 2:
                                             n = f.sent().IdentityId, t = n, f.label = 3;
                                         case 3:
-                                            return [4, gd(l, {
+                                            return [4, yd(l, {
                                                 IdentityId: e || t,
                                                 Logins: u
                                             })];
                                         case 4:
-                                            return r = f.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, p = r.IdentityId, this._identityId = p, e ? (wd.debug("The guest identity ".concat(e, " has been successfully linked to the logins")), e === p && wd.debug("The guest identity ".concat(e, " has become the primary identity")), [4, this._removeGuestIdentityId()]) : [3, 6];
+                                            return r = f.sent(), o = r.Credentials, i = o.AccessKeyId, s = o.Expiration, c = o.SecretKey, d = o.SessionToken, p = r.IdentityId, this._identityId = p, e ? (xd.debug("The guest identity ".concat(e, " has been successfully linked to the logins")), e === p && xd.debug("The guest identity ".concat(e, " has become the primary identity")), [4, this._removeGuestIdentityId()]) : [3, 6];
                                         case 5:
                                             f.sent(), f.label = 6;
                                         case 6:
                                             return [2, {
                                                 accessKeyId: i,
                                                 secretAccessKey: c,
                                                 sessionToken: d,
                                                 expiration: s,
                                                 identityId: p
                                             }]
                                     }
                                 }))
                             })).catch((function(e) {
-                                return jd(t, void 0, void 0, (function() {
-                                    return bd(this, (function(t) {
+                                return bd(t, void 0, void 0, (function() {
+                                    return wd(this, (function(t) {
                                         throw e
                                     }))
                                 }))
                             }));
                         return this._loadCredentials(c, "userPool", !0, null)
                     }, e.prototype._loadCredentials = function(e, t, n, r) {
                         var o = this,
                             i = this;
                         return new Promise((function(a, s) {
                             e.then((function(e) {
-                                return jd(o, void 0, void 0, (function() {
+                                return bd(o, void 0, void 0, (function() {
                                     var o, s, u, l, c;
-                                    return bd(this, (function(d) {
+                                    return wd(this, (function(d) {
                                         switch (d.label) {
                                             case 0:
-                                                if (wd.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
+                                                if (xd.debug("Load credentials successfully", e), this._identityId && !e.identityId && (e.identityId = this._identityId), i._credentials = e, i._credentials.authenticated = n, i._credentials_source = t, i._nextCredentialsRefresh = (new Date).getTime() + 3e6, "federated" === t) {
                                                     o = Object.assign({
                                                         id: this._credentials.identityId
                                                     }, r.user), s = r.provider, u = r.token, l = r.expires_at, c = r.identity_id;
                                                     try {
                                                         this._storage.setItem("aws-amplify-federatedInfo", JSON.stringify({
                                                             provider: s,
                                                             token: u,
                                                             user: o,
                                                             expires_at: l,
                                                             identity_id: c
                                                         }))
                                                     } catch (p) {
-                                                        wd.debug("Failed to put federated info into auth storage", p)
+                                                        xd.debug("Failed to put federated info into auth storage", p)
                                                     }
                                                 }
                                                 return "guest" !== t ? [3, 2] : [4, this._setGuestIdentityId(e.identityId)];
                                             case 1:
                                                 d.sent(), d.label = 2;
                                             case 2:
                                                 return a(i._credentials), [2]
                                         }
                                     }))
                                 }))
                             })).catch((function(t) {
-                                if (t) return wd.debug("Failed to load credentials", e), wd.debug("Error loading credentials", t), void s(t)
+                                if (t) return xd.debug("Failed to load credentials", e), xd.debug("Error loading credentials", t), void s(t)
                             }))
                         }))
                     }, e.prototype.set = function(e, t) {
-                        return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (wd.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
+                        return "session" === t ? this._setCredentialsFromSession(e) : "federation" === t ? this._setCredentialsFromFederation(e) : "guest" === t ? this._setCredentialsForGuest() : (xd.debug("no source specified for setting credentials"), Promise.reject("invalid source"))
                     }, e.prototype.clear = function() {
-                        return jd(this, void 0, void 0, (function() {
-                            return bd(this, (function(e) {
-                                return this._credentials = null, this._credentials_source = null, wd.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
+                        return bd(this, void 0, void 0, (function() {
+                            return wd(this, (function(e) {
+                                return this._credentials = null, this._credentials_source = null, xd.debug("removing aws-amplify-federatedInfo from storage"), this._storage.removeItem("aws-amplify-federatedInfo"), [2]
                             }))
                         }))
                     }, e.prototype._getGuestIdentityId = function() {
-                        return jd(this, void 0, void 0, (function() {
+                        return bd(this, void 0, void 0, (function() {
                             var e, t;
-                            return bd(this, (function(n) {
+                            return wd(this, (function(n) {
                                 switch (n.label) {
                                     case 0:
                                         e = this._config.identityPoolId, n.label = 1;
                                     case 1:
                                         return n.trys.push([1, 3, , 4]), [4, this._storageSync];
                                     case 2:
                                         return n.sent(), [2, this._storage.getItem(this._getCognitoIdentityIdStorageKey(e))];
                                     case 3:
-                                        return t = n.sent(), wd.debug("Failed to get the cached guest identityId", t), [3, 4];
+                                        return t = n.sent(), xd.debug("Failed to get the cached guest identityId", t), [3, 4];
                                     case 4:
                                         return [2]
                                 }
                             }))
                         }))
                     }, e.prototype._setGuestIdentityId = function(e) {
-                        return jd(this, void 0, void 0, (function() {
+                        return bd(this, void 0, void 0, (function() {
                             var t, n;
-                            return bd(this, (function(r) {
+                            return wd(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
                                         t = this._config.identityPoolId, r.label = 1;
                                     case 1:
                                         return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                     case 2:
                                         return r.sent(), this._storage.setItem(this._getCognitoIdentityIdStorageKey(t), e), [3, 4];
                                     case 3:
-                                        return n = r.sent(), wd.debug("Failed to cache guest identityId", n), [3, 4];
+                                        return n = r.sent(), xd.debug("Failed to cache guest identityId", n), [3, 4];
                                     case 4:
                                         return [2]
                                 }
                             }))
                         }))
                     }, e.prototype._removeGuestIdentityId = function() {
-                        return jd(this, void 0, void 0, (function() {
+                        return bd(this, void 0, void 0, (function() {
                             var e;
-                            return bd(this, (function(t) {
-                                return e = this._config.identityPoolId, wd.debug("removing ".concat(this._getCognitoIdentityIdStorageKey(e), " from storage")), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
+                            return wd(this, (function(t) {
+                                return e = this._config.identityPoolId, xd.debug("removing ".concat(this._getCognitoIdentityIdStorageKey(e), " from storage")), this._storage.removeItem(this._getCognitoIdentityIdStorageKey(e)), [2]
                             }))
                         }))
                     }, e.prototype.shear = function(e) {
                         return {
                             accessKeyId: e.accessKeyId,
                             sessionToken: e.sessionToken,
                             secretAccessKey: e.secretAccessKey,
                             identityId: e.identityId,
                             authenticated: e.authenticated
                         }
                     }, e
                 }(),
-                Id = new Nd(null);
-            $l.register(Id);
-            var Dd = function() {
-                    return Dd = Object.assign || function(e) {
+                Dd = new Id(null);
+            ec.register(Dd);
+            var Ld = function() {
+                    return Ld = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
                         return e
-                    }, Dd.apply(this, arguments)
+                    }, Ld.apply(this, arguments)
                 },
-                Ld = gl().isBrowser,
-                Sd = function() {
+                Sd = yl().isBrowser,
+                kd = function() {
                     function e(e) {
-                        void 0 === e && (e = {}), this.cookies = new vt, this.store = Ld ? window.localStorage : Object.create(null), this.cookies = e.req ? new vt(e.req.headers.cookie) : new vt, Object.assign(this.store, this.cookies.getAll())
+                        void 0 === e && (e = {}), this.cookies = new vt, this.store = Sd ? window.localStorage : Object.create(null), this.cookies = e.req ? new vt(e.req.headers.cookie) : new vt, Object.assign(this.store, this.cookies.getAll())
                     }
                     return Object.defineProperty(e.prototype, "length", {
                         get: function() {
                             return Object.entries(this.store).length
                         },
                         enumerable: !1,
                         configurable: !0
@@ -61946,22 +61949,22 @@
                         var n = e.split(".").pop();
                         ["LastAuthUser", "accessToken", "refreshToken", "idToken"].includes(null !== n && void 0 !== n ? n : "") && this.setUniversalItem(e, t, {
                             expires: new Date(Date.now() + 31536e6)
                         })
                     }, e.prototype.setLocalItem = function(e, t) {
                         this.store[e] = t
                     }, e.prototype.setUniversalItem = function(e, t, n) {
-                        void 0 === n && (n = {}), this.cookies.set(e, t, Dd(Dd({}, n), {
+                        void 0 === n && (n = {}), this.cookies.set(e, t, Ld(Ld({}, n), {
                             path: "/",
                             sameSite: !0,
-                            secure: !Ld || "localhost" !== window.location.hostname
+                            secure: !Sd || "localhost" !== window.location.hostname
                         }))
                     }, e
                 }();
-            var kd, Cd = function() {
+            var Cd, Ed = function() {
                     function e(e) {
                         var t = e || {},
                             n = t.ValidationData,
                             r = t.Username,
                             o = t.Password,
                             i = t.AuthParameters,
                             a = t.ClientMetadata;
@@ -61976,254 +61979,254 @@
                         return this.validationData
                     }, t.getAuthParameters = function() {
                         return this.authParameters
                     }, t.getClientMetadata = function() {
                         return this.clientMetadata
                     }, e
                 }(),
-                Ed = n(2890);
+                Td = n(2890);
 
-            function Td() {
-                if (kd) {
-                    if ("function" === typeof kd.getRandomValues) try {
-                        return kd.getRandomValues(new Uint32Array(1))[0]
+            function Ad() {
+                if (Cd) {
+                    if ("function" === typeof Cd.getRandomValues) try {
+                        return Cd.getRandomValues(new Uint32Array(1))[0]
                     } catch (e) {}
-                    if ("function" === typeof kd.randomBytes) try {
-                        return kd.randomBytes(4).readInt32LE()
+                    if ("function" === typeof Cd.randomBytes) try {
+                        return Cd.randomBytes(4).readInt32LE()
                     } catch (e) {}
                 }
                 throw new Error("Native crypto module could not be used to get secure random number.")
             }
-            "undefined" !== typeof window && window.crypto && (kd = window.crypto), !kd && "undefined" !== typeof window && window.msCrypto && (kd = window.msCrypto);
-            var Ad, zd = function() {
+            "undefined" !== typeof window && window.crypto && (Cd = window.crypto), !Cd && "undefined" !== typeof window && window.msCrypto && (Cd = window.msCrypto);
+            var zd, Od = function() {
                     function e(e, t) {
                         e = this.words = e || [], this.sigBytes = void 0 != t ? t : 4 * e.length
                     }
                     var t = e.prototype;
                     return t.random = function(t) {
-                        for (var n = [], r = 0; r < t; r += 4) n.push(Td());
+                        for (var n = [], r = 0; r < t; r += 4) n.push(Ad());
                         return new e(n, t)
                     }, t.toString = function() {
                         return function(e) {
                             for (var t = e.words, n = e.sigBytes, r = [], o = 0; o < n; o++) {
                                 var i = t[o >>> 2] >>> 24 - o % 4 * 8 & 255;
                                 r.push((i >>> 4).toString(16)), r.push((15 & i).toString(16))
                             }
                             return r.join("")
                         }(this)
                     }, e
                 }(),
-                Od = n(6915),
-                _d = Ud;
+                _d = n(6915),
+                Ud = Pd;
 
-            function Ud(e, t) {
+            function Pd(e, t) {
                 null != e && this.fromString(e, t)
             }
 
-            function Pd() {
-                return new Ud(null)
+            function Rd() {
+                return new Pd(null)
             }
-            var Rd = "undefined" !== typeof navigator;
-            Rd && "Microsoft Internet Explorer" == navigator.appName ? (Ud.prototype.am = function(e, t, n, r, o, i) {
+            var Fd = "undefined" !== typeof navigator;
+            Fd && "Microsoft Internet Explorer" == navigator.appName ? (Pd.prototype.am = function(e, t, n, r, o, i) {
                 for (var a = 32767 & t, s = t >> 15; --i >= 0;) {
                     var u = 32767 & this[e],
                         l = this[e++] >> 15,
                         c = s * u + l * a;
                     o = ((u = a * u + ((32767 & c) << 15) + n[r] + (1073741823 & o)) >>> 30) + (c >>> 15) + s * l + (o >>> 30), n[r++] = 1073741823 & u
                 }
                 return o
-            }, Ad = 30) : Rd && "Netscape" != navigator.appName ? (Ud.prototype.am = function(e, t, n, r, o, i) {
+            }, zd = 30) : Fd && "Netscape" != navigator.appName ? (Pd.prototype.am = function(e, t, n, r, o, i) {
                 for (; --i >= 0;) {
                     var a = t * this[e++] + n[r] + o;
                     o = Math.floor(a / 67108864), n[r++] = 67108863 & a
                 }
                 return o
-            }, Ad = 26) : (Ud.prototype.am = function(e, t, n, r, o, i) {
+            }, zd = 26) : (Pd.prototype.am = function(e, t, n, r, o, i) {
                 for (var a = 16383 & t, s = t >> 14; --i >= 0;) {
                     var u = 16383 & this[e],
                         l = this[e++] >> 14,
                         c = s * u + l * a;
                     o = ((u = a * u + ((16383 & c) << 14) + n[r] + o) >> 28) + (c >> 14) + s * l, n[r++] = 268435455 & u
                 }
                 return o
-            }, Ad = 28), Ud.prototype.DB = Ad, Ud.prototype.DM = (1 << Ad) - 1, Ud.prototype.DV = 1 << Ad;
-            Ud.prototype.FV = Math.pow(2, 52), Ud.prototype.F1 = 52 - Ad, Ud.prototype.F2 = 2 * Ad - 52;
-            var Fd, Bd, Yd = "0123456789abcdefghijklmnopqrstuvwxyz",
-                Qd = new Array;
-            for (Fd = "0".charCodeAt(0), Bd = 0; Bd <= 9; ++Bd) Qd[Fd++] = Bd;
-            for (Fd = "a".charCodeAt(0), Bd = 10; Bd < 36; ++Bd) Qd[Fd++] = Bd;
-            for (Fd = "A".charCodeAt(0), Bd = 10; Bd < 36; ++Bd) Qd[Fd++] = Bd;
+            }, zd = 28), Pd.prototype.DB = zd, Pd.prototype.DM = (1 << zd) - 1, Pd.prototype.DV = 1 << zd;
+            Pd.prototype.FV = Math.pow(2, 52), Pd.prototype.F1 = 52 - zd, Pd.prototype.F2 = 2 * zd - 52;
+            var Bd, Yd, Qd = "0123456789abcdefghijklmnopqrstuvwxyz",
+                Gd = new Array;
+            for (Bd = "0".charCodeAt(0), Yd = 0; Yd <= 9; ++Yd) Gd[Bd++] = Yd;
+            for (Bd = "a".charCodeAt(0), Yd = 10; Yd < 36; ++Yd) Gd[Bd++] = Yd;
+            for (Bd = "A".charCodeAt(0), Yd = 10; Yd < 36; ++Yd) Gd[Bd++] = Yd;
 
-            function Gd(e) {
-                return Yd.charAt(e)
+            function Wd(e) {
+                return Qd.charAt(e)
             }
 
-            function Wd(e, t) {
-                var n = Qd[e.charCodeAt(t)];
+            function Hd(e, t) {
+                var n = Gd[e.charCodeAt(t)];
                 return null == n ? -1 : n
             }
 
-            function Hd(e) {
-                var t = Pd();
+            function Vd(e) {
+                var t = Rd();
                 return t.fromInt(e), t
             }
 
-            function Vd(e) {
+            function Zd(e) {
                 var t, n = 1;
                 return 0 != (t = e >>> 16) && (e = t, n += 16), 0 != (t = e >> 8) && (e = t, n += 8), 0 != (t = e >> 4) && (e = t, n += 4), 0 != (t = e >> 2) && (e = t, n += 2), 0 != (t = e >> 1) && (e = t, n += 1), n
             }
 
-            function Zd(e) {
+            function qd(e) {
                 this.m = e, this.mp = e.invDigit(), this.mpl = 32767 & this.mp, this.mph = this.mp >> 15, this.um = (1 << e.DB - 15) - 1, this.mt2 = 2 * e.t
             }
 
-            function qd(e) {
-                return Ed.lW.from((new zd).random(e).toString(), "hex")
+            function Jd(e) {
+                return Td.lW.from((new Od).random(e).toString(), "hex")
             }
-            Zd.prototype.convert = function(e) {
-                var t = Pd();
-                return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(Ud.ZERO) > 0 && this.m.subTo(t, t), t
-            }, Zd.prototype.revert = function(e) {
-                var t = Pd();
+            qd.prototype.convert = function(e) {
+                var t = Rd();
+                return e.abs().dlShiftTo(this.m.t, t), t.divRemTo(this.m, null, t), e.s < 0 && t.compareTo(Pd.ZERO) > 0 && this.m.subTo(t, t), t
+            }, qd.prototype.revert = function(e) {
+                var t = Rd();
                 return e.copyTo(t), this.reduce(t), t
-            }, Zd.prototype.reduce = function(e) {
+            }, qd.prototype.reduce = function(e) {
                 for (; e.t <= this.mt2;) e[e.t++] = 0;
                 for (var t = 0; t < this.m.t; ++t) {
                     var n = 32767 & e[t],
                         r = n * this.mpl + ((n * this.mph + (e[t] >> 15) * this.mpl & this.um) << 15) & e.DM;
                     for (e[n = t + this.m.t] += this.m.am(0, r, e, t, 0, this.m.t); e[n] >= e.DV;) e[n] -= e.DV, e[++n]++
                 }
                 e.clamp(), e.drShiftTo(this.m.t, e), e.compareTo(this.m) >= 0 && e.subTo(this.m, e)
-            }, Zd.prototype.mulTo = function(e, t, n) {
+            }, qd.prototype.mulTo = function(e, t, n) {
                 e.multiplyTo(t, n), this.reduce(n)
-            }, Zd.prototype.sqrTo = function(e, t) {
+            }, qd.prototype.sqrTo = function(e, t) {
                 e.squareTo(t), this.reduce(t)
-            }, Ud.prototype.copyTo = function(e) {
+            }, Pd.prototype.copyTo = function(e) {
                 for (var t = this.t - 1; t >= 0; --t) e[t] = this[t];
                 e.t = this.t, e.s = this.s
-            }, Ud.prototype.fromInt = function(e) {
+            }, Pd.prototype.fromInt = function(e) {
                 this.t = 1, this.s = e < 0 ? -1 : 0, e > 0 ? this[0] = e : e < -1 ? this[0] = e + this.DV : this.t = 0
-            }, Ud.prototype.fromString = function(e, t) {
+            }, Pd.prototype.fromString = function(e, t) {
                 var n;
                 if (16 == t) n = 4;
                 else if (8 == t) n = 3;
                 else if (2 == t) n = 1;
                 else if (32 == t) n = 5;
                 else {
                     if (4 != t) throw new Error("Only radix 2, 4, 8, 16, 32 are supported");
                     n = 2
                 }
                 this.t = 0, this.s = 0;
                 for (var r = e.length, o = !1, i = 0; --r >= 0;) {
-                    var a = Wd(e, r);
+                    var a = Hd(e, r);
                     a < 0 ? "-" == e.charAt(r) && (o = !0) : (o = !1, 0 == i ? this[this.t++] = a : i + n > this.DB ? (this[this.t - 1] |= (a & (1 << this.DB - i) - 1) << i, this[this.t++] = a >> this.DB - i) : this[this.t - 1] |= a << i, (i += n) >= this.DB && (i -= this.DB))
                 }
-                this.clamp(), o && Ud.ZERO.subTo(this, this)
-            }, Ud.prototype.clamp = function() {
+                this.clamp(), o && Pd.ZERO.subTo(this, this)
+            }, Pd.prototype.clamp = function() {
                 for (var e = this.s & this.DM; this.t > 0 && this[this.t - 1] == e;) --this.t
-            }, Ud.prototype.dlShiftTo = function(e, t) {
+            }, Pd.prototype.dlShiftTo = function(e, t) {
                 var n;
                 for (n = this.t - 1; n >= 0; --n) t[n + e] = this[n];
                 for (n = e - 1; n >= 0; --n) t[n] = 0;
                 t.t = this.t + e, t.s = this.s
-            }, Ud.prototype.drShiftTo = function(e, t) {
+            }, Pd.prototype.drShiftTo = function(e, t) {
                 for (var n = e; n < this.t; ++n) t[n - e] = this[n];
                 t.t = Math.max(this.t - e, 0), t.s = this.s
-            }, Ud.prototype.lShiftTo = function(e, t) {
+            }, Pd.prototype.lShiftTo = function(e, t) {
                 var n, r = e % this.DB,
                     o = this.DB - r,
                     i = (1 << o) - 1,
                     a = Math.floor(e / this.DB),
                     s = this.s << r & this.DM;
                 for (n = this.t - 1; n >= 0; --n) t[n + a + 1] = this[n] >> o | s, s = (this[n] & i) << r;
                 for (n = a - 1; n >= 0; --n) t[n] = 0;
                 t[a] = s, t.t = this.t + a + 1, t.s = this.s, t.clamp()
-            }, Ud.prototype.rShiftTo = function(e, t) {
+            }, Pd.prototype.rShiftTo = function(e, t) {
                 t.s = this.s;
                 var n = Math.floor(e / this.DB);
                 if (n >= this.t) t.t = 0;
                 else {
                     var r = e % this.DB,
                         o = this.DB - r,
                         i = (1 << r) - 1;
                     t[0] = this[n] >> r;
                     for (var a = n + 1; a < this.t; ++a) t[a - n - 1] |= (this[a] & i) << o, t[a - n] = this[a] >> r;
                     r > 0 && (t[this.t - n - 1] |= (this.s & i) << o), t.t = this.t - n, t.clamp()
                 }
-            }, Ud.prototype.subTo = function(e, t) {
+            }, Pd.prototype.subTo = function(e, t) {
                 for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] - e[n], t[n++] = r & this.DM, r >>= this.DB;
                 if (e.t < this.t) {
                     for (r -= e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                     r += this.s
                 } else {
                     for (r += this.s; n < e.t;) r -= e[n], t[n++] = r & this.DM, r >>= this.DB;
                     r -= e.s
                 }
                 t.s = r < 0 ? -1 : 0, r < -1 ? t[n++] = this.DV + r : r > 0 && (t[n++] = r), t.t = n, t.clamp()
-            }, Ud.prototype.multiplyTo = function(e, t) {
+            }, Pd.prototype.multiplyTo = function(e, t) {
                 var n = this.abs(),
                     r = e.abs(),
                     o = n.t;
                 for (t.t = o + r.t; --o >= 0;) t[o] = 0;
                 for (o = 0; o < r.t; ++o) t[o + n.t] = n.am(0, r[o], t, o, 0, n.t);
-                t.s = 0, t.clamp(), this.s != e.s && Ud.ZERO.subTo(t, t)
-            }, Ud.prototype.squareTo = function(e) {
+                t.s = 0, t.clamp(), this.s != e.s && Pd.ZERO.subTo(t, t)
+            }, Pd.prototype.squareTo = function(e) {
                 for (var t = this.abs(), n = e.t = 2 * t.t; --n >= 0;) e[n] = 0;
                 for (n = 0; n < t.t - 1; ++n) {
                     var r = t.am(n, t[n], e, 2 * n, 0, 1);
                     (e[n + t.t] += t.am(n + 1, 2 * t[n], e, 2 * n + 1, r, t.t - n - 1)) >= t.DV && (e[n + t.t] -= t.DV, e[n + t.t + 1] = 1)
                 }
                 e.t > 0 && (e[e.t - 1] += t.am(n, t[n], e, 2 * n, 0, 1)), e.s = 0, e.clamp()
-            }, Ud.prototype.divRemTo = function(e, t, n) {
+            }, Pd.prototype.divRemTo = function(e, t, n) {
                 var r = e.abs();
                 if (!(r.t <= 0)) {
                     var o = this.abs();
                     if (o.t < r.t) return null != t && t.fromInt(0), void(null != n && this.copyTo(n));
-                    null == n && (n = Pd());
-                    var i = Pd(),
+                    null == n && (n = Rd());
+                    var i = Rd(),
                         a = this.s,
                         s = e.s,
-                        u = this.DB - Vd(r[r.t - 1]);
+                        u = this.DB - Zd(r[r.t - 1]);
                     u > 0 ? (r.lShiftTo(u, i), o.lShiftTo(u, n)) : (r.copyTo(i), o.copyTo(n));
                     var l = i.t,
                         c = i[l - 1];
                     if (0 != c) {
                         var d = c * (1 << this.F1) + (l > 1 ? i[l - 2] >> this.F2 : 0),
                             p = this.FV / d,
                             f = (1 << this.F1) / d,
                             h = 1 << this.F2,
                             g = n.t,
                             y = g - l,
-                            m = null == t ? Pd() : t;
-                        for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), Ud.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
+                            m = null == t ? Rd() : t;
+                        for (i.dlShiftTo(y, m), n.compareTo(m) >= 0 && (n[n.t++] = 1, n.subTo(m, n)), Pd.ONE.dlShiftTo(l, m), m.subTo(i, i); i.t < l;) i[i.t++] = 0;
                         for (; --y >= 0;) {
                             var v = n[--g] == c ? this.DM : Math.floor(n[g] * p + (n[g - 1] + h) * f);
                             if ((n[g] += i.am(0, v, n, y, 0, l)) < v)
                                 for (i.dlShiftTo(y, m), n.subTo(m, n); n[g] < --v;) n.subTo(m, n)
                         }
-                        null != t && (n.drShiftTo(l, t), a != s && Ud.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && Ud.ZERO.subTo(n, n)
+                        null != t && (n.drShiftTo(l, t), a != s && Pd.ZERO.subTo(t, t)), n.t = l, n.clamp(), u > 0 && n.rShiftTo(u, n), a < 0 && Pd.ZERO.subTo(n, n)
                     }
                 }
-            }, Ud.prototype.invDigit = function() {
+            }, Pd.prototype.invDigit = function() {
                 if (this.t < 1) return 0;
                 var e = this[0];
                 if (0 == (1 & e)) return 0;
                 var t = 3 & e;
                 return (t = (t = (t = (t = t * (2 - (15 & e) * t) & 15) * (2 - (255 & e) * t) & 255) * (2 - ((65535 & e) * t & 65535)) & 65535) * (2 - e * t % this.DV) % this.DV) > 0 ? this.DV - t : -t
-            }, Ud.prototype.addTo = function(e, t) {
+            }, Pd.prototype.addTo = function(e, t) {
                 for (var n = 0, r = 0, o = Math.min(e.t, this.t); n < o;) r += this[n] + e[n], t[n++] = r & this.DM, r >>= this.DB;
                 if (e.t < this.t) {
                     for (r += e.s; n < this.t;) r += this[n], t[n++] = r & this.DM, r >>= this.DB;
                     r += this.s
                 } else {
                     for (r += this.s; n < e.t;) r += e[n], t[n++] = r & this.DM, r >>= this.DB;
                     r += e.s
                 }
                 t.s = r < 0 ? -1 : 0, r > 0 ? t[n++] = r : r < -1 && (t[n++] = this.DV + r), t.t = n, t.clamp()
-            }, Ud.prototype.toString = function(e) {
+            }, Pd.prototype.toString = function(e) {
                 if (this.s < 0) return "-" + this.negate().toString(e);
                 var t;
                 if (16 == e) t = 4;
                 else if (8 == e) t = 3;
                 else if (2 == e) t = 1;
                 else if (32 == e) t = 5;
                 else {
@@ -62232,231 +62235,231 @@
                 }
                 var n, r = (1 << t) - 1,
                     o = !1,
                     i = "",
                     a = this.t,
                     s = this.DB - a * this.DB % t;
                 if (a-- > 0)
-                    for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Gd(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Gd(n));
+                    for (s < this.DB && (n = this[a] >> s) > 0 && (o = !0, i = Wd(n)); a >= 0;) s < t ? (n = (this[a] & (1 << s) - 1) << t - s, n |= this[--a] >> (s += this.DB - t)) : (n = this[a] >> (s -= t) & r, s <= 0 && (s += this.DB, --a)), n > 0 && (o = !0), o && (i += Wd(n));
                 return o ? i : "0"
-            }, Ud.prototype.negate = function() {
-                var e = Pd();
-                return Ud.ZERO.subTo(this, e), e
-            }, Ud.prototype.abs = function() {
+            }, Pd.prototype.negate = function() {
+                var e = Rd();
+                return Pd.ZERO.subTo(this, e), e
+            }, Pd.prototype.abs = function() {
                 return this.s < 0 ? this.negate() : this
-            }, Ud.prototype.compareTo = function(e) {
+            }, Pd.prototype.compareTo = function(e) {
                 var t = this.s - e.s;
                 if (0 != t) return t;
                 var n = this.t;
                 if (0 != (t = n - e.t)) return this.s < 0 ? -t : t;
                 for (; --n >= 0;)
                     if (0 != (t = this[n] - e[n])) return t;
                 return 0
-            }, Ud.prototype.bitLength = function() {
-                return this.t <= 0 ? 0 : this.DB * (this.t - 1) + Vd(this[this.t - 1] ^ this.s & this.DM)
-            }, Ud.prototype.mod = function(e) {
-                var t = Pd();
-                return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(Ud.ZERO) > 0 && e.subTo(t, t), t
-            }, Ud.prototype.equals = function(e) {
+            }, Pd.prototype.bitLength = function() {
+                return this.t <= 0 ? 0 : this.DB * (this.t - 1) + Zd(this[this.t - 1] ^ this.s & this.DM)
+            }, Pd.prototype.mod = function(e) {
+                var t = Rd();
+                return this.abs().divRemTo(e, null, t), this.s < 0 && t.compareTo(Pd.ZERO) > 0 && e.subTo(t, t), t
+            }, Pd.prototype.equals = function(e) {
                 return 0 == this.compareTo(e)
-            }, Ud.prototype.add = function(e) {
-                var t = Pd();
+            }, Pd.prototype.add = function(e) {
+                var t = Rd();
                 return this.addTo(e, t), t
-            }, Ud.prototype.subtract = function(e) {
-                var t = Pd();
+            }, Pd.prototype.subtract = function(e) {
+                var t = Rd();
                 return this.subTo(e, t), t
-            }, Ud.prototype.multiply = function(e) {
-                var t = Pd();
+            }, Pd.prototype.multiply = function(e) {
+                var t = Rd();
                 return this.multiplyTo(e, t), t
-            }, Ud.prototype.divide = function(e) {
-                var t = Pd();
+            }, Pd.prototype.divide = function(e) {
+                var t = Rd();
                 return this.divRemTo(e, t, null), t
-            }, Ud.prototype.modPow = function(e, t, n) {
+            }, Pd.prototype.modPow = function(e, t, n) {
                 var r, o = e.bitLength(),
-                    i = Hd(1),
-                    a = new Zd(t);
+                    i = Vd(1),
+                    a = new qd(t);
                 if (o <= 0) return i;
                 r = o < 18 ? 1 : o < 48 ? 3 : o < 144 ? 4 : o < 768 ? 5 : 6;
                 var s = new Array,
                     u = 3,
                     l = r - 1,
                     c = (1 << r) - 1;
                 if (s[1] = a.convert(this), r > 1) {
-                    var d = Pd();
-                    for (a.sqrTo(s[1], d); u <= c;) s[u] = Pd(), a.mulTo(d, s[u - 2], s[u]), u += 2
+                    var d = Rd();
+                    for (a.sqrTo(s[1], d); u <= c;) s[u] = Rd(), a.mulTo(d, s[u - 2], s[u]), u += 2
                 }
                 var p, f, h = e.t - 1,
                     g = !0,
-                    y = Pd();
-                for (o = Vd(e[h]) - 1; h >= 0;) {
+                    y = Rd();
+                for (o = Zd(e[h]) - 1; h >= 0;) {
                     for (o >= l ? p = e[h] >> o - l & c : (p = (e[h] & (1 << o + 1) - 1) << l - o, h > 0 && (p |= e[h - 1] >> this.DB + o - l)), u = r; 0 == (1 & p);) p >>= 1, --u;
                     if ((o -= u) < 0 && (o += this.DB, --h), g) s[p].copyTo(i), g = !1;
                     else {
                         for (; u > 1;) a.sqrTo(i, y), a.sqrTo(y, i), u -= 2;
                         u > 0 ? a.sqrTo(i, y) : (f = i, i = y, y = f), a.mulTo(y, s[p], i)
                     }
                     for (; h >= 0 && 0 == (e[h] & 1 << o);) a.sqrTo(i, y), f = i, i = y, y = f, --o < 0 && (o = this.DB - 1, --h)
                 }
                 var m = a.revert(i);
                 return n(null, m), m
-            }, Ud.ZERO = Hd(0), Ud.ONE = Hd(1);
-            var Jd = /^[89a-f]/i,
-                Kd = function() {
+            }, Pd.ZERO = Vd(0), Pd.ONE = Vd(1);
+            var Kd = /^[89a-f]/i,
+                Xd = function() {
                     function e(e) {
-                        this.N = new _d("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new _d("2", 16), this.k = new _d(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = Ed.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
+                        this.N = new Ud("FFFFFFFFFFFFFFFFC90FDAA22168C234C4C6628B80DC1CD129024E088A67CC74020BBEA63B139B22514A08798E3404DDEF9519B3CD3A431B302B0A6DF25F14374FE1356D6D51C245E485B576625E7EC6F44C42E9A637ED6B0BFF5CB6F406B7EDEE386BFB5A899FA5AE9F24117C4B1FE649286651ECE45B3DC2007CB8A163BF0598DA48361C55D39A69163FA8FD24CF5F83655D23DCA3AD961C62F356208552BB9ED529077096966D670C354E4ABC9804F1746C08CA18217C32905E462E36CE3BE39E772C180E86039B2783A2EC07A28FB5C55DF06F4C52C9DE2BCBF6955817183995497CEA956AE515D2261898FA051015728E5A8AAAC42DAD33170D04507A33A85521ABDF1CBA64ECFB850458DBEF0A8AEA71575D060C7DB3970F85A6E1E4C7ABF5AE8CDB0933D71E8C94E04A25619DCEE3D2261AD2EE6BF12FFA06D98A0864D87602733EC86A64521F2B18177B200CBBE117577A615D6C770988C0BAD946E208E24FA074E5AB3143DB5BFCE0FD108E4B82D120A93AD2CAFFFFFFFFFFFFFFFF", 16), this.g = new Ud("2", 16), this.k = new Ud(this.hexHash("" + this.padHex(this.N) + this.padHex(this.g)), 16), this.smallAValue = this.generateRandomSmallA(), this.getLargeAValue((function() {})), this.infoBits = Td.lW.from("Caldera Derived Key", "utf8"), this.poolName = e
                     }
                     var t = e.prototype;
                     return t.getSmallAValue = function() {
                         return this.smallAValue
                     }, t.getLargeAValue = function(e) {
                         var t = this;
                         this.largeAValue ? e(null, this.largeAValue) : this.calculateA(this.smallAValue, (function(n, r) {
                             n && e(n, null), t.largeAValue = r, e(null, t.largeAValue)
                         }))
                     }, t.generateRandomSmallA = function() {
-                        var e = qd(128).toString("hex");
-                        return new _d(e, 16)
+                        var e = Jd(128).toString("hex");
+                        return new Ud(e, 16)
                     }, t.generateRandomString = function() {
-                        return qd(40).toString("base64")
+                        return Jd(40).toString("base64")
                     }, t.getRandomPassword = function() {
                         return this.randomPassword
                     }, t.getSaltDevices = function() {
                         return this.SaltToHashDevices
                     }, t.getVerifierDevices = function() {
                         return this.verifierDevices
                     }, t.generateHashDevice = function(e, t, n) {
                         var r = this;
                         this.randomPassword = this.generateRandomString();
                         var o = "" + e + t + ":" + this.randomPassword,
                             i = this.hash(o),
-                            a = qd(16).toString("hex");
-                        this.SaltToHashDevices = this.padHex(new _d(a, 16)), this.g.modPow(new _d(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
+                            a = Jd(16).toString("hex");
+                        this.SaltToHashDevices = this.padHex(new Ud(a, 16)), this.g.modPow(new Ud(this.hexHash(this.SaltToHashDevices + i), 16), this.N, (function(e, t) {
                             e && n(e, null), r.verifierDevices = r.padHex(t), n(null, null)
                         }))
                     }, t.calculateA = function(e, t) {
                         var n = this;
                         this.g.modPow(e, this.N, (function(e, r) {
-                            e && t(e, null), r.mod(n.N).equals(_d.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
+                            e && t(e, null), r.mod(n.N).equals(Ud.ZERO) && t(new Error("Illegal paramater. A mod N cannot be 0."), null), t(null, r)
                         }))
                     }, t.calculateU = function(e, t) {
-                        return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new _d(this.UHexHash, 16)
+                        return this.UHexHash = this.hexHash(this.padHex(e) + this.padHex(t)), new Ud(this.UHexHash, 16)
                     }, t.hash = function(e) {
-                        var t = new Od.Sha256;
+                        var t = new _d.Sha256;
                         t.update(e);
                         var n = t.digestSync(),
-                            r = Ed.lW.from(n).toString("hex");
+                            r = Td.lW.from(n).toString("hex");
                         return new Array(64 - r.length).join("0") + r
                     }, t.hexHash = function(e) {
-                        return this.hash(Ed.lW.from(e, "hex"))
+                        return this.hash(Td.lW.from(e, "hex"))
                     }, t.computehkdf = function(e, t) {
-                        var n = Ed.lW.concat([this.infoBits, Ed.lW.from(String.fromCharCode(1), "utf8")]),
-                            r = new Od.Sha256(t);
+                        var n = Td.lW.concat([this.infoBits, Td.lW.from(String.fromCharCode(1), "utf8")]),
+                            r = new _d.Sha256(t);
                         r.update(e);
                         var o = r.digestSync(),
-                            i = new Od.Sha256(o);
+                            i = new _d.Sha256(o);
                         return i.update(n), i.digestSync().slice(0, 16)
                     }, t.getPasswordAuthenticationKey = function(e, t, n, r, o) {
                         var i = this;
-                        if (n.mod(this.N).equals(_d.ZERO)) throw new Error("B cannot be zero.");
-                        if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(_d.ZERO)) throw new Error("U cannot be zero.");
+                        if (n.mod(this.N).equals(Ud.ZERO)) throw new Error("B cannot be zero.");
+                        if (this.UValue = this.calculateU(this.largeAValue, n), this.UValue.equals(Ud.ZERO)) throw new Error("U cannot be zero.");
                         var a = "" + this.poolName + e + ":" + t,
                             s = this.hash(a),
-                            u = new _d(this.hexHash(this.padHex(r) + s), 16);
+                            u = new Ud(this.hexHash(this.padHex(r) + s), 16);
                         this.calculateS(u, n, (function(e, t) {
                             e && o(e, null);
-                            var n = i.computehkdf(Ed.lW.from(i.padHex(t), "hex"), Ed.lW.from(i.padHex(i.UValue), "hex"));
+                            var n = i.computehkdf(Td.lW.from(i.padHex(t), "hex"), Td.lW.from(i.padHex(i.UValue), "hex"));
                             o(null, n)
                         }))
                     }, t.calculateS = function(e, t, n) {
                         var r = this;
                         this.g.modPow(e, this.N, (function(o, i) {
                             o && n(o, null), t.subtract(r.k.multiply(i)).modPow(r.smallAValue.add(r.UValue.multiply(e)), r.N, (function(e, t) {
                                 e && n(e, null), n(null, t.mod(r.N))
                             }))
                         }))
                     }, t.getNewPasswordRequiredChallengeUserAttributePrefix = function() {
                         return "userAttributes."
                     }, t.padHex = function(e) {
-                        if (!(e instanceof _d)) throw new Error("Not a BigInteger");
-                        var t = e.compareTo(_d.ZERO) < 0,
+                        if (!(e instanceof Ud)) throw new Error("Not a BigInteger");
+                        var t = e.compareTo(Ud.ZERO) < 0,
                             n = e.abs().toString(16);
-                        if (n = n.length % 2 !== 0 ? "0" + n : n, n = Jd.test(n) ? "00" + n : n, t) {
+                        if (n = n.length % 2 !== 0 ? "0" + n : n, n = Kd.test(n) ? "00" + n : n, t) {
                             var r = n.split("").map((function(e) {
                                 var t = 15 & ~parseInt(e, 16);
                                 return "0123456789ABCDEF".charAt(t)
                             })).join("");
-                            (n = new _d(r, 16).add(_d.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
+                            (n = new Ud(r, 16).add(Ud.ONE).toString(16)).toUpperCase().startsWith("FF8") && (n = n.substring(2))
                         }
                         return n
                     }, e
                 }(),
-                Xd = function() {
+                $d = function() {
                     function e(e) {
                         this.jwtToken = e || "", this.payload = this.decodePayload()
                     }
                     var t = e.prototype;
                     return t.getJwtToken = function() {
                         return this.jwtToken
                     }, t.getExpiration = function() {
                         return this.payload.exp
                     }, t.getIssuedAt = function() {
                         return this.payload.iat
                     }, t.decodePayload = function() {
                         var e = this.jwtToken.split(".")[1];
                         try {
-                            return JSON.parse(Ed.lW.from(e, "base64").toString("utf8"))
+                            return JSON.parse(Td.lW.from(e, "base64").toString("utf8"))
                         } catch (t) {
                             return {}
                         }
                     }, e
                 }();
 
-            function $d(e, t) {
-                return $d = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+            function ep(e, t) {
+                return ep = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                     return e.__proto__ = t, e
-                }, $d(e, t)
+                }, ep(e, t)
             }
-            var ep = function(e) {
+            var tp = function(e) {
                 var t, n;
 
                 function r(t) {
                     var n = (void 0 === t ? {} : t).AccessToken;
                     return e.call(this, n || "") || this
                 }
-                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, $d(t, n), r
-            }(Xd);
+                return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, ep(t, n), r
+            }($d);
 
-            function tp(e, t) {
-                return tp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+            function np(e, t) {
+                return np = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                     return e.__proto__ = t, e
-                }, tp(e, t)
+                }, np(e, t)
             }
-            var np = function(e) {
+            var rp = function(e) {
                     var t, n;
 
                     function r(t) {
                         var n = (void 0 === t ? {} : t).IdToken;
                         return e.call(this, n || "") || this
                     }
-                    return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, tp(t, n), r
-                }(Xd),
-                rp = function() {
+                    return n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, np(t, n), r
+                }($d),
+                op = function() {
                     function e(e) {
                         var t = (void 0 === e ? {} : e).RefreshToken;
                         this.token = t || ""
                     }
                     return e.prototype.getToken = function() {
                         return this.token
                     }, e
                 }(),
-                op = {
+                ip = {
                     userAgent: "aws-amplify/5.0.4",
                     isReactNative: "undefined" !== typeof navigator && "ReactNative" === navigator.product
                 },
-                ip = function() {
+                ap = function() {
                     function e(e) {
                         var t = void 0 === e ? {} : e,
                             n = t.IdToken,
                             r = t.RefreshToken,
                             o = t.AccessToken,
                             i = t.ClockDrift;
                         if (null == o || null == n) throw new Error("Id token and Access Token must be present.");
@@ -62474,32 +62477,32 @@
                     }, t.calculateClockDrift = function() {
                         return Math.floor(new Date / 1e3) - Math.min(this.accessToken.getIssuedAt(), this.idToken.getIssuedAt())
                     }, t.isValid = function() {
                         var e = Math.floor(new Date / 1e3) - this.clockDrift;
                         return e < this.accessToken.getExpiration() && e < this.idToken.getExpiration()
                     }, e
                 }(),
-                ap = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
-                sp = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
-                up = function() {
+                sp = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
+                up = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"],
+                lp = function() {
                     function e() {}
                     return e.prototype.getNowString = function() {
                         var e = new Date,
-                            t = sp[e.getUTCDay()],
-                            n = ap[e.getUTCMonth()],
+                            t = up[e.getUTCDay()],
+                            n = sp[e.getUTCMonth()],
                             r = e.getUTCDate(),
                             o = e.getUTCHours();
                         o < 10 && (o = "0" + o);
                         var i = e.getUTCMinutes();
                         i < 10 && (i = "0" + i);
                         var a = e.getUTCSeconds();
                         return a < 10 && (a = "0" + a), t + " " + n + " " + r + " " + o + ":" + i + ":" + a + " UTC " + e.getUTCFullYear()
                     }, e
                 }(),
-                lp = function() {
+                cp = function() {
                     function e(e) {
                         var t = void 0 === e ? {} : e,
                             n = t.Name,
                             r = t.Value;
                         this.Name = n || "", this.Value = r || ""
                     }
                     var t = e.prototype;
@@ -62516,44 +62519,44 @@
                     }, t.toJSON = function() {
                         return {
                             Name: this.Name,
                             Value: this.Value
                         }
                     }, e
                 }(),
-                cp = {},
-                dp = function() {
+                dp = {},
+                pp = function() {
                     function e() {}
                     return e.setItem = function(e, t) {
-                        return cp[e] = t, cp[e]
+                        return dp[e] = t, dp[e]
                     }, e.getItem = function(e) {
-                        return Object.prototype.hasOwnProperty.call(cp, e) ? cp[e] : void 0
+                        return Object.prototype.hasOwnProperty.call(dp, e) ? dp[e] : void 0
                     }, e.removeItem = function(e) {
-                        return delete cp[e]
+                        return delete dp[e]
                     }, e.clear = function() {
-                        return cp = {}
+                        return dp = {}
                     }, e
                 }(),
-                pp = function() {
+                fp = function() {
                     function e() {
                         try {
                             this.storageWindow = window.localStorage, this.storageWindow.setItem("aws.cognito.test-ls", 1), this.storageWindow.removeItem("aws.cognito.test-ls")
                         } catch (e) {
-                            this.storageWindow = dp
+                            this.storageWindow = pp
                         }
                     }
                     return e.prototype.getStorage = function() {
                         return this.storageWindow
                     }, e
                 }(),
-                fp = "undefined" !== typeof navigator ? op.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
-                hp = function() {
+                hp = "undefined" !== typeof navigator ? ip.isReactNative ? "react-native" : navigator.userAgent : "nodejs",
+                gp = function() {
                     function e(e) {
                         if (null == e || null == e.Username || null == e.Pool) throw new Error("Username and Pool information are required.");
-                        this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new pp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
+                        this.username = e.Username || "", this.pool = e.Pool, this.Session = null, this.client = e.Pool.client, this.signInUserSession = null, this.authenticationFlowType = "USER_SRP_AUTH", this.storage = e.Storage || (new fp).getStorage(), this.keyPrefix = "CognitoIdentityServiceProvider." + this.pool.getClientId(), this.userDataKey = this.keyPrefix + "." + this.username + ".userData"
                     }
                     var t = e.prototype;
                     return t.setSignInUserSession = function(e) {
                         this.clearCachedUserData(), this.signInUserSession = e, this.cacheTokens()
                     }, t.getSignInUserSession = function() {
                         return this.signInUserSession
                     }, t.getUsername = function() {
@@ -62579,37 +62582,37 @@
                                 i = r.ChallengeParameters;
                             return "CUSTOM_CHALLENGE" === o ? (n.Session = r.Session, t.customChallenge(i)) : (n.signInUserSession = n.getCognitoUserSession(r.AuthenticationResult), n.cacheTokens(), t.onSuccess(n.signInUserSession))
                         }))
                     }, t.authenticateUser = function(e, t) {
                         return "USER_PASSWORD_AUTH" === this.authenticationFlowType ? this.authenticateUserPlainUsernamePassword(e, t) : "USER_SRP_AUTH" === this.authenticationFlowType || "CUSTOM_AUTH" === this.authenticationFlowType ? this.authenticateUserDefaultAuth(e, t) : t.onFailure(new Error("Authentication flow type is invalid."))
                     }, t.authenticateUserDefaultAuth = function(e, t) {
                         var n, r, o = this,
-                            i = new Kd(this.pool.getUserPoolName()),
-                            a = new up,
+                            i = new Xd(this.pool.getUserPoolName()),
+                            a = new lp,
                             s = {};
                         null != this.deviceKey && (s.DEVICE_KEY = this.deviceKey), s.USERNAME = this.username, i.getLargeAValue((function(u, l) {
                             u && t.onFailure(u), s.SRP_A = l.toString(16), "CUSTOM_AUTH" === o.authenticationFlowType && (s.CHALLENGE_NAME = "SRP_A");
                             var c = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                                 d = {
                                     AuthFlow: o.authenticationFlowType,
                                     ClientId: o.pool.getClientId(),
                                     AuthParameters: s,
                                     ClientMetadata: c
                                 };
                             o.getUserContextData(o.username) && (d.UserContextData = o.getUserContextData(o.username)), o.client.request("InitiateAuth", d, (function(s, u) {
                                 if (s) return t.onFailure(s);
                                 var l = u.ChallengeParameters;
-                                o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new _d(l.SRP_B, 16), r = new _d(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
+                                o.username = l.USER_ID_FOR_SRP, o.userDataKey = o.keyPrefix + "." + o.username + ".userData", n = new Ud(l.SRP_B, 16), r = new Ud(l.SALT, 16), o.getCachedDeviceKeyAndPassword(), i.getPasswordAuthenticationKey(o.username, e.getPassword(), n, r, (function(e, n) {
                                     e && t.onFailure(e);
                                     var r = a.getNowString(),
-                                        s = Ed.lW.concat([Ed.lW.from(o.pool.getUserPoolName(), "utf8"), Ed.lW.from(o.username, "utf8"), Ed.lW.from(l.SECRET_BLOCK, "base64"), Ed.lW.from(r, "utf8")]),
-                                        d = new Od.Sha256(n);
+                                        s = Td.lW.concat([Td.lW.from(o.pool.getUserPoolName(), "utf8"), Td.lW.from(o.username, "utf8"), Td.lW.from(l.SECRET_BLOCK, "base64"), Td.lW.from(r, "utf8")]),
+                                        d = new _d.Sha256(n);
                                     d.update(s);
                                     var p = d.digestSync(),
-                                        f = Ed.lW.from(p).toString("base64"),
+                                        f = Td.lW.from(p).toString("base64"),
                                         h = {};
                                     h.USERNAME = o.username, h.PASSWORD_CLAIM_SECRET_BLOCK = l.SECRET_BLOCK, h.TIMESTAMP = r, h.PASSWORD_CLAIM_SIGNATURE = f, null != o.deviceKey && (h.DEVICE_KEY = o.deviceKey);
                                     var g = {
                                         ChallengeName: "PASSWORD_VERIFIER",
                                         ClientId: o.pool.getClientId(),
                                         ChallengeResponses: h,
                                         Session: u.Session,
@@ -62626,15 +62629,15 @@
                                 }))
                             }))
                         }))
                     }, t.authenticateUserPlainUsernamePassword = function(e, t) {
                         var n = this,
                             r = {};
                         if (r.USERNAME = this.username, r.PASSWORD = e.getPassword(), r.PASSWORD) {
-                            var o = new Kd(this.pool.getUserPoolName());
+                            var o = new Xd(this.pool.getUserPoolName());
                             this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (r.DEVICE_KEY = this.deviceKey);
                             var i = 0 !== Object.keys(e.getValidationData()).length ? e.getValidationData() : e.getClientMetadata(),
                                 a = {
                                     AuthFlow: "USER_PASSWORD_AUTH",
                                     ClientId: this.pool.getClientId(),
                                     AuthParameters: r,
                                     ClientMetadata: i
@@ -62665,30 +62668,30 @@
                         if ("DEVICE_SRP_AUTH" === o) return this.Session = e.Session, void this.getDeviceResponse(n);
                         this.signInUserSession = this.getCognitoUserSession(e.AuthenticationResult), this.challengeName = o, this.cacheTokens();
                         var d = e.AuthenticationResult.NewDeviceMetadata;
                         if (null == d) return n.onSuccess(this.signInUserSession);
                         t.generateHashDevice(e.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, e.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(o) {
                             if (o) return n.onFailure(o);
                             var i = {
-                                Salt: Ed.lW.from(t.getSaltDevices(), "hex").toString("base64"),
-                                PasswordVerifier: Ed.lW.from(t.getVerifierDevices(), "hex").toString("base64")
+                                Salt: Td.lW.from(t.getSaltDevices(), "hex").toString("base64"),
+                                PasswordVerifier: Td.lW.from(t.getVerifierDevices(), "hex").toString("base64")
                             };
                             r.verifierDevices = i.PasswordVerifier, r.deviceGroupKey = d.DeviceGroupKey, r.randomPassword = t.getRandomPassword(), r.client.request("ConfirmDevice", {
                                 DeviceKey: d.DeviceKey,
                                 AccessToken: r.signInUserSession.getAccessToken().getJwtToken(),
                                 DeviceSecretVerifierConfig: i,
-                                DeviceName: fp
+                                DeviceName: hp
                             }, (function(t, o) {
                                 return t ? n.onFailure(t) : (r.deviceKey = e.AuthenticationResult.NewDeviceMetadata.DeviceKey, r.cacheDeviceKeyAndPassword(), !0 === o.UserConfirmationNecessary ? n.onSuccess(r.signInUserSession, o.UserConfirmationNecessary) : n.onSuccess(r.signInUserSession))
                             }))
                         }))
                     }, t.completeNewPasswordChallenge = function(e, t, n, r) {
                         var o = this;
                         if (!e) return n.onFailure(new Error("New password is required."));
-                        var i = new Kd(this.pool.getUserPoolName()),
+                        var i = new Xd(this.pool.getUserPoolName()),
                             a = i.getNewPasswordRequiredChallengeUserAttributePrefix(),
                             s = {};
                         t && Object.keys(t).forEach((function(e) {
                             s[a + e] = t[e]
                         })), s.NEW_PASSWORD = e, s.USERNAME = this.username;
                         var u = {
                             ChallengeName: "NEW_PASSWORD_REQUIRED",
@@ -62698,39 +62701,39 @@
                             ClientMetadata: r
                         };
                         this.getUserContextData() && (u.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", u, (function(e, t) {
                             return e ? n.onFailure(e) : o.authenticateUserInternal(t, i, n)
                         }))
                     }, t.getDeviceResponse = function(e, t) {
                         var n = this,
-                            r = new Kd(this.deviceGroupKey),
-                            o = new up,
+                            r = new Xd(this.deviceGroupKey),
+                            o = new lp,
                             i = {};
                         i.USERNAME = this.username, i.DEVICE_KEY = this.deviceKey, r.getLargeAValue((function(a, s) {
                             a && e.onFailure(a), i.SRP_A = s.toString(16);
                             var u = {
                                 ChallengeName: "DEVICE_SRP_AUTH",
                                 ClientId: n.pool.getClientId(),
                                 ChallengeResponses: i,
                                 ClientMetadata: t,
                                 Session: n.Session
                             };
                             n.getUserContextData() && (u.UserContextData = n.getUserContextData()), n.client.request("RespondToAuthChallenge", u, (function(t, i) {
                                 if (t) return e.onFailure(t);
                                 var a = i.ChallengeParameters,
-                                    s = new _d(a.SRP_B, 16),
-                                    u = new _d(a.SALT, 16);
+                                    s = new Ud(a.SRP_B, 16),
+                                    u = new Ud(a.SALT, 16);
                                 r.getPasswordAuthenticationKey(n.deviceKey, n.randomPassword, s, u, (function(t, r) {
                                     if (t) return e.onFailure(t);
                                     var s = o.getNowString(),
-                                        u = Ed.lW.concat([Ed.lW.from(n.deviceGroupKey, "utf8"), Ed.lW.from(n.deviceKey, "utf8"), Ed.lW.from(a.SECRET_BLOCK, "base64"), Ed.lW.from(s, "utf8")]),
-                                        l = new Od.Sha256(r);
+                                        u = Td.lW.concat([Td.lW.from(n.deviceGroupKey, "utf8"), Td.lW.from(n.deviceKey, "utf8"), Td.lW.from(a.SECRET_BLOCK, "base64"), Td.lW.from(s, "utf8")]),
+                                        l = new _d.Sha256(r);
                                     l.update(u);
                                     var c = l.digestSync(),
-                                        d = Ed.lW.from(c).toString("base64"),
+                                        d = Td.lW.from(c).toString("base64"),
                                         p = {};
                                     p.USERNAME = n.username, p.PASSWORD_CLAIM_SECRET_BLOCK = a.SECRET_BLOCK, p.TIMESTAMP = s, p.PASSWORD_CLAIM_SIGNATURE = d, p.DEVICE_KEY = n.deviceKey;
                                     var f = {
                                         ChallengeName: "DEVICE_PASSWORD_VERIFIER",
                                         ClientId: n.pool.getClientId(),
                                         ChallengeResponses: p,
                                         Session: i.Session
@@ -62752,15 +62755,15 @@
                         this.getUserContextData() && (o.UserContextData = this.getUserContextData()), this.client.request("ConfirmSignUp", o, (function(e) {
                             return e ? n(e, null) : n(null, "SUCCESS")
                         }))
                     }, t.sendCustomChallengeAnswer = function(e, t, n) {
                         var r = this,
                             o = {};
                         o.USERNAME = this.username, o.ANSWER = e;
-                        var i = new Kd(this.pool.getUserPoolName());
+                        var i = new Xd(this.pool.getUserPoolName());
                         this.getCachedDeviceKeyAndPassword(), null != this.deviceKey && (o.DEVICE_KEY = this.deviceKey);
                         var a = {
                             ChallengeName: "CUSTOM_CHALLENGE",
                             ChallengeResponses: o,
                             ClientId: this.pool.getClientId(),
                             Session: this.Session,
                             ClientMetadata: n
@@ -62781,26 +62784,26 @@
                             Session: this.Session,
                             ClientMetadata: r
                         };
                         this.getUserContextData() && (s.UserContextData = this.getUserContextData()), this.client.request("RespondToAuthChallenge", s, (function(e, n) {
                             if (e) return t.onFailure(e);
                             if ("DEVICE_SRP_AUTH" !== n.ChallengeName) {
                                 if (o.signInUserSession = o.getCognitoUserSession(n.AuthenticationResult), o.cacheTokens(), null == n.AuthenticationResult.NewDeviceMetadata) return t.onSuccess(o.signInUserSession);
-                                var r = new Kd(o.pool.getUserPoolName());
+                                var r = new Xd(o.pool.getUserPoolName());
                                 r.generateHashDevice(n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, n.AuthenticationResult.NewDeviceMetadata.DeviceKey, (function(e) {
                                     if (e) return t.onFailure(e);
                                     var i = {
-                                        Salt: Ed.lW.from(r.getSaltDevices(), "hex").toString("base64"),
-                                        PasswordVerifier: Ed.lW.from(r.getVerifierDevices(), "hex").toString("base64")
+                                        Salt: Td.lW.from(r.getSaltDevices(), "hex").toString("base64"),
+                                        PasswordVerifier: Td.lW.from(r.getVerifierDevices(), "hex").toString("base64")
                                     };
                                     o.verifierDevices = i.PasswordVerifier, o.deviceGroupKey = n.AuthenticationResult.NewDeviceMetadata.DeviceGroupKey, o.randomPassword = r.getRandomPassword(), o.client.request("ConfirmDevice", {
                                         DeviceKey: n.AuthenticationResult.NewDeviceMetadata.DeviceKey,
                                         AccessToken: o.signInUserSession.getAccessToken().getJwtToken(),
                                         DeviceSecretVerifierConfig: i,
-                                        DeviceName: fp
+                                        DeviceName: hp
                                     }, (function(e, r) {
                                         return e ? t.onFailure(e) : (o.deviceKey = n.AuthenticationResult.NewDeviceMetadata.DeviceKey, o.cacheDeviceKeyAndPassword(), !0 === r.UserConfirmationNecessary ? t.onSuccess(o.signInUserSession, r.UserConfirmationNecessary) : t.onSuccess(o.signInUserSession))
                                     }))
                                 }))
                             } else o.getDeviceResponse(t)
                         }))
                     }, t.changePassword = function(e, t, n, r) {
@@ -62872,15 +62875,15 @@
                         }, (function(t, n) {
                             if (t) return e(t, null);
                             for (var r = [], o = 0; o < n.UserAttributes.length; o++) {
                                 var i = {
                                         Name: n.UserAttributes[o].Name,
                                         Value: n.UserAttributes[o].Value
                                     },
-                                    a = new lp(i);
+                                    a = new cp(i);
                                 r.push(a)
                             }
                             return e(null, r)
                         }))
                     }, t.getMFAOptions = function(e) {
                         if (null == this.signInUserSession || !this.signInUserSession.isValid()) return e(new Error("User is not authenticated"), null);
                         this.client.request("GetUser", {
@@ -62954,25 +62957,25 @@
                         if (null != this.signInUserSession && this.signInUserSession.isValid()) return e(null, this.signInUserSession);
                         var n = "CognitoIdentityServiceProvider." + this.pool.getClientId() + "." + this.username,
                             r = n + ".idToken",
                             o = n + ".accessToken",
                             i = n + ".refreshToken",
                             a = n + ".clockDrift";
                         if (this.storage.getItem(r)) {
-                            var s = new np({
+                            var s = new rp({
                                     IdToken: this.storage.getItem(r)
                                 }),
-                                u = new ep({
+                                u = new tp({
                                     AccessToken: this.storage.getItem(o)
                                 }),
-                                l = new rp({
+                                l = new op({
                                     RefreshToken: this.storage.getItem(i)
                                 }),
                                 c = parseInt(this.storage.getItem(a), 0) || 0,
-                                d = new ip({
+                                d = new ap({
                                     IdToken: s,
                                     AccessToken: u,
                                     RefreshToken: l,
                                     ClockDrift: c
                                 });
                             if (d.isValid()) return this.signInUserSession = d, e(null, this.signInUserSession);
                             if (!l.getToken()) return e(new Error("Cannot retrieve a new session. Please authenticate."), null);
@@ -63040,18 +63043,18 @@
                             t = e + "." + this.username + ".idToken",
                             n = e + "." + this.username + ".accessToken",
                             r = e + "." + this.username + ".refreshToken",
                             o = e + ".LastAuthUser",
                             i = e + "." + this.username + ".clockDrift";
                         this.storage.removeItem(t), this.storage.removeItem(n), this.storage.removeItem(r), this.storage.removeItem(o), this.storage.removeItem(i)
                     }, t.getCognitoUserSession = function(e) {
-                        var t = new np(e),
-                            n = new ep(e),
-                            r = new rp(e);
-                        return new ip({
+                        var t = new rp(e),
+                            n = new tp(e),
+                            r = new op(e);
+                        return new ap({
                             IdToken: t,
                             AccessToken: n,
                             RefreshToken: r
                         })
                     }, t.forgotPassword = function(e, t) {
                         var n = {
                             ClientId: this.pool.getClientId(),
@@ -63237,111 +63240,111 @@
                             r.getUserContextData() && (i.UserContextData = r.getUserContextData()), r.client.request("RespondToAuthChallenge", i, (function(e, t) {
                                 return e ? n.onFailure(e) : (r.signInUserSession = r.getCognitoUserSession(t.AuthenticationResult), r.cacheTokens(), n.onSuccess(r.signInUserSession))
                             }))
                         }))
                     }, e
                 }();
 
-            function gp() {}
-            gp.prototype.userAgent = op.userAgent;
-            var yp = function(e) {
-                    gp.framework = e
+            function yp() {}
+            yp.prototype.userAgent = ip.userAgent;
+            var mp = function(e) {
+                    yp.framework = e
                 },
-                mp = function(e) {
-                    var t = gp.category ? " " + gp.category : "",
-                        n = gp.framework ? " framework/" + gp.framework : "";
-                    return "" + gp.prototype.userAgent + t + n
+                vp = function(e) {
+                    var t = yp.category ? " " + yp.category : "",
+                        n = yp.framework ? " framework/" + yp.framework : "";
+                    return "" + yp.prototype.userAgent + t + n
                 };
 
-            function vp(e, t) {
-                e.prototype = Object.create(t.prototype), e.prototype.constructor = e, bp(e, t)
+            function Mp(e, t) {
+                e.prototype = Object.create(t.prototype), e.prototype.constructor = e, wp(e, t)
             }
 
-            function Mp(e) {
+            function jp(e) {
                 var t = "function" === typeof Map ? new Map : void 0;
-                return Mp = function(e) {
+                return jp = function(e) {
                     if (null === e || (n = e, -1 === Function.toString.call(n).indexOf("[native code]"))) return e;
                     var n;
                     if ("function" !== typeof e) throw new TypeError("Super expression must either be null or a function");
                     if ("undefined" !== typeof t) {
                         if (t.has(e)) return t.get(e);
                         t.set(e, r)
                     }
 
                     function r() {
-                        return jp(e, arguments, wp(this).constructor)
+                        return bp(e, arguments, xp(this).constructor)
                     }
                     return r.prototype = Object.create(e.prototype, {
                         constructor: {
                             value: r,
                             enumerable: !1,
                             writable: !0,
                             configurable: !0
                         }
-                    }), bp(r, e)
-                }, Mp(e)
+                    }), wp(r, e)
+                }, jp(e)
             }
 
-            function jp(e, t, n) {
-                return jp = function() {
+            function bp(e, t, n) {
+                return bp = function() {
                     if ("undefined" === typeof Reflect || !Reflect.construct) return !1;
                     if (Reflect.construct.sham) return !1;
                     if ("function" === typeof Proxy) return !0;
                     try {
                         return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                     } catch (e) {
                         return !1
                     }
                 }() ? Reflect.construct.bind() : function(e, t, n) {
                     var r = [null];
                     r.push.apply(r, t);
                     var o = new(Function.bind.apply(e, r));
-                    return n && bp(o, n.prototype), o
-                }, jp.apply(null, arguments)
+                    return n && wp(o, n.prototype), o
+                }, bp.apply(null, arguments)
             }
 
-            function bp(e, t) {
-                return bp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+            function wp(e, t) {
+                return wp = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                     return e.__proto__ = t, e
-                }, bp(e, t)
+                }, wp(e, t)
             }
 
-            function wp(e) {
-                return wp = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+            function xp(e) {
+                return xp = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                     return e.__proto__ || Object.getPrototypeOf(e)
-                }, wp(e)
+                }, xp(e)
             }
-            var xp = function(e) {
+            var Np = function(e) {
                     function t(t, n, r, o) {
                         var i;
                         return (i = e.call(this, t) || this).code = n, i.name = r, i.statusCode = o, i
                     }
-                    return vp(t, e), t
-                }(Mp(Error)),
-                Np = function() {
+                    return Mp(t, e), t
+                }(jp(Error)),
+                Ip = function() {
                     function e(e, t, n) {
                         this.endpoint = t || "https://cognito-idp." + e + ".amazonaws.com/";
                         var r = (n || {}).credentials;
                         this.fetchOptions = r ? {
                             credentials: r
                         } : {}
                     }
                     var t = e.prototype;
                     return t.promisifyRequest = function(e, t) {
                         var n = this;
                         return new Promise((function(r, o) {
                             n.request(e, t, (function(e, t) {
-                                e ? o(new xp(e.message, e.code, e.name, e.statusCode)) : r(t)
+                                e ? o(new Np(e.message, e.code, e.name, e.statusCode)) : r(t)
                             }))
                         }))
                     }, t.requestWithRetry = function(e, t, n) {
                         var r = this;
                         (function(e, t, n) {
-                            void 0 === n && (n = Sp);
-                            return Lp(e, t, function(e) {
+                            void 0 === n && (n = kp);
+                            return Sp(e, t, function(e) {
                                 var t = 100,
                                     n = 100;
                                 return function(r) {
                                     var o = Math.pow(2, r) * t + n * Math.random();
                                     return !(o > e) && o
                                 }
                             }(n))
@@ -63356,15 +63359,15 @@
                         })).catch((function(e) {
                             return n(e)
                         }))
                     }, t.request = function(e, t, n) {
                         var r, o = {
                                 "Content-Type": "application/x-amz-json-1.1",
                                 "X-Amz-Target": "AWSCognitoIdentityProviderService." + e,
-                                "X-Amz-User-Agent": mp(),
+                                "X-Amz-User-Agent": vp(),
                                 "Cache-Control": "no-store"
                             },
                             i = Object.assign({}, this.fetchOptions, {
                                 headers: o,
                                 method: "POST",
                                 mode: "cors",
                                 body: JSON.stringify(t)
@@ -63392,47 +63395,47 @@
                             } catch (i) {
                                 return n(e)
                             } else e instanceof Error && "Network error" === e.message && (e.code = "NetworkError");
                             return n(e)
                         }))
                     }, e
                 }(),
-                Ip = {
+                Dp = {
                     debug: function() {}
                 },
-                Dp = function(e) {
+                Lp = function(e) {
                     return e && e.nonRetryable
                 };
 
-            function Lp(e, t, n, r) {
+            function Sp(e, t, n, r) {
                 if (void 0 === r && (r = 1), "function" !== typeof e) throw Error("functionToRetry must be a function");
-                return Ip.debug(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
-                    if (Ip.debug("error on " + e.name, o), Dp(o)) throw Ip.debug(e.name + " non retryable error", o), o;
+                return Dp.debug(e.name + " attempt #" + r + " with args: " + JSON.stringify(t)), e.apply(void 0, t).catch((function(o) {
+                    if (Dp.debug("error on " + e.name, o), Lp(o)) throw Dp.debug(e.name + " non retryable error", o), o;
                     var i = n(r, t, o);
-                    if (Ip.debug(e.name + " retrying in " + i + " ms"), !1 !== i) return new Promise((function(e) {
+                    if (Dp.debug(e.name + " retrying in " + i + " ms"), !1 !== i) return new Promise((function(e) {
                         return setTimeout(e, i)
                     })).then((function() {
-                        return Lp(e, t, n, r + 1)
+                        return Sp(e, t, n, r + 1)
                     }));
                     throw o
                 }))
             }
-            var Sp = 3e5;
-            var kp, Cp = function() {
+            var kp = 3e5;
+            var Cp, Ep = function() {
                     function e(e, t) {
                         var n = e || {},
                             r = n.UserPoolId,
                             o = n.ClientId,
                             i = n.endpoint,
                             a = n.fetchOptions,
                             s = n.AdvancedSecurityDataCollectionFlag;
                         if (!r || !o) throw new Error("Both UserPoolId and ClientId are required.");
                         if (r.length > 55 || !/^[\w-]+_[0-9a-zA-Z]+$/.test(r)) throw new Error("Invalid UserPoolId format.");
                         var u = r.split("_")[0];
-                        this.userPoolId = r, this.clientId = o, this.client = new Np(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new pp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
+                        this.userPoolId = r, this.clientId = o, this.client = new Ip(u, i, a), this.advancedSecurityDataCollectionFlag = !1 !== s, this.storage = e.Storage || (new fp).getStorage(), t && (this.wrapRefreshSessionCallback = t)
                     }
                     var t = e.prototype;
                     return t.getUserPoolId = function() {
                         return this.userPoolId
                     }, t.getUserPoolName = function() {
                         return this.getUserPoolId().split("_")[1]
                     }, t.getClientId = function() {
@@ -63451,15 +63454,15 @@
                             if (t) return o(t, null);
                             var r = {
                                     Username: e,
                                     Pool: a,
                                     Storage: a.storage
                                 },
                                 i = {
-                                    user: new hp(r),
+                                    user: new gp(r),
                                     userConfirmed: n.UserConfirmed,
                                     userSub: n.UserSub,
                                     codeDeliveryDetails: n.CodeDeliveryDetails
                                 };
                             return o(null, i)
                         }))
                     }, t.getCurrentUser = function() {
@@ -63467,15 +63470,15 @@
                             t = this.storage.getItem(e);
                         if (t) {
                             var n = {
                                 Username: t,
                                 Pool: this,
                                 Storage: this.storage
                             };
-                            return new hp(n)
+                            return new gp(n)
                         }
                         return null
                     }, t.getUserContextData = function(e) {
                         if ("undefined" !== typeof AmazonCognitoAdvancedSecurityData) {
                             var t = AmazonCognitoAdvancedSecurityData;
                             if (this.advancedSecurityDataCollectionFlag) {
                                 var n = t.getData(e, this.userPoolId, this.clientId);
@@ -63483,16 +63486,16 @@
                                     EncodedData: n
                                 }
                             }
                             return {}
                         }
                     }, e
                 }(),
-                Ep = n(5943),
-                Tp = function() {
+                Tp = n(5943),
+                Ap = function() {
                     function e(e) {
                         if (void 0 === e && (e = {}), e.domain && (this.domain = e.domain), e.path ? this.path = e.path : this.path = "/", Object.prototype.hasOwnProperty.call(e, "expires") ? this.expires = e.expires : this.expires = 365, Object.prototype.hasOwnProperty.call(e, "secure") ? this.secure = e.secure : this.secure = !0, Object.prototype.hasOwnProperty.call(e, "sameSite")) {
                             if (!["strict", "lax", "none"].includes(e.sameSite)) throw new Error('The sameSite value of cookieStorage must be "lax", "strict" or "none".');
                             if ("none" === e.sameSite && !this.secure) throw new Error("sameSite = None requires the Secure attribute in latest browser versions.");
                             this.sameSite = e.sameSite
                         } else this.sameSite = null
                     }
@@ -63500,127 +63503,127 @@
                     return t.setItem = function(e, t) {
                         var n = {
                             path: this.path,
                             expires: this.expires,
                             domain: this.domain,
                             secure: this.secure
                         };
-                        return this.sameSite && (n.sameSite = this.sameSite), Ep.set(e, t, n), Ep.get(e)
+                        return this.sameSite && (n.sameSite = this.sameSite), Tp.set(e, t, n), Tp.get(e)
                     }, t.getItem = function(e) {
-                        return Ep.get(e)
+                        return Tp.get(e)
                     }, t.removeItem = function(e) {
                         var t = {
                             path: this.path,
                             expires: this.expires,
                             domain: this.domain,
                             secure: this.secure
                         };
-                        return this.sameSite && (t.sameSite = this.sameSite), Ep.remove(e, t)
+                        return this.sameSite && (t.sameSite = this.sameSite), Tp.remove(e, t)
                     }, t.clear = function() {
-                        for (var e = Ep.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
+                        for (var e = Tp.get(), t = Object.keys(e).length, n = 0; n < t; ++n) this.removeItem(Object.keys(e)[n]);
                         return {}
                     }, e
                 }(),
-                Ap = n(2770),
-                zp = function(e) {
+                zp = n(2770),
+                Op = function(e) {
                     var t = window.open(e, "_self");
                     return t ? Promise.resolve(t) : Promise.reject()
                 },
-                Op = ("undefined" !== typeof Symbol && "function" === typeof Symbol.for && Symbol.for("INTERNAL_AWS_APPSYNC_REALTIME_PUBSUB_PROVIDER"), "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default"),
-                _p = function(e, t, n) {
-                    dl.dispatch("auth", {
+                _p = ("undefined" !== typeof Symbol && "function" === typeof Symbol.for && Symbol.for("INTERNAL_AWS_APPSYNC_REALTIME_PUBSUB_PROVIDER"), "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default"),
+                Up = function(e, t, n) {
+                    pl.dispatch("auth", {
                         event: e,
                         data: t,
                         message: n
-                    }, "Auth", Op)
+                    }, "Auth", _p)
                 },
-                Up = new ol("OAuth"),
-                Pp = function() {
+                Pp = new il("OAuth"),
+                Rp = function() {
                     function e(e) {
                         var t = e.config,
                             n = e.cognitoClientId,
                             r = e.scopes,
                             o = void 0 === r ? [] : r;
-                        if (this._urlOpener = t.urlOpener || zp, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
+                        if (this._urlOpener = t.urlOpener || Op, this._config = t, this._cognitoClientId = n, !this.isValidScopes(o)) throw Error("scopes must be a String Array");
                         this._scopes = o
                     }
                     return e.prototype.isValidScopes = function(e) {
                         return Array.isArray(e) && e.every((function(e) {
                             return "string" === typeof e
                         }))
                     }, e.prototype.oauthSignIn = function(e, t, n, r, o, i) {
-                        void 0 === e && (e = "code"), void 0 === o && (o = Gu.Cognito);
+                        void 0 === e && (e = "code"), void 0 === o && (o = Wu.Cognito);
                         var a = this._generateState(32),
                             s = i ? a + "-" + i.split("").map((function(e) {
                                 return e.charCodeAt(0).toString(16).padStart(2, "0")
                             })).join("") : a;
                         ! function(e) {
                             window.sessionStorage.setItem("oauth_state", e)
                         }(s);
                         var u, l = this._generateRandom(128);
                         u = l, window.sessionStorage.setItem("ouath_pkce_key", u);
                         var c = this._generateChallenge(l),
                             d = this._scopes.join(" "),
-                            p = Object.entries(Vu(Vu({
+                            p = Object.entries(Zu(Zu({
                                 redirect_uri: n,
                                 response_type: e,
                                 client_id: r,
                                 identity_provider: o,
                                 scope: d,
                                 state: s
                             }, "code" === e ? {
                                 code_challenge: c
                             } : {}), "code" === e ? {
                                 code_challenge_method: "S256"
                             } : {})).map((function(e) {
-                                var t = Ju(e, 2),
+                                var t = Ku(e, 2),
                                     n = t[0],
                                     r = t[1];
                                 return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                             })).join("&"),
                             f = "https://" + t + "/oauth2/authorize?" + p;
-                        Up.debug("Redirecting to " + f), this._urlOpener(f, n)
+                        Pp.debug("Redirecting to " + f), this._urlOpener(f, n)
                     }, e.prototype._handleCodeFlow = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s, u, l, c, d, p, f, h, g, y;
-                            return qu(this, (function(m) {
+                            return Ju(this, (function(m) {
                                 switch (m.label) {
                                     case 0:
-                                        return t = ((0, Ap.Qc)(e).query || "").split("&").map((function(e) {
+                                        return t = ((0, zp.Qc)(e).query || "").split("&").map((function(e) {
                                             return e.split("=")
                                         })).reduce((function(e, t) {
-                                            var n, r = Ju(t, 2),
+                                            var n, r = Ku(t, 2),
                                                 o = r[0],
                                                 i = r[1];
-                                            return Vu(Vu({}, e), ((n = {})[o] = i, n))
+                                            return Zu(Zu({}, e), ((n = {})[o] = i, n))
                                         }), {
                                             code: void 0
-                                        }).code, n = (0, Ap.Qc)(e).pathname || "/", r = (0, Ap.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", _p("codeFlow", {}, "Retrieving tokens from " + o), i = Xu(this._config) ? this._cognitoClientId : this._config.clientID, a = Xu(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
+                                        }).code, n = (0, zp.Qc)(e).pathname || "/", r = (0, zp.Qc)(this._config.redirectSignIn).pathname || "/", t && n === r ? (o = "https://" + this._config.domain + "/oauth2/token", Up("codeFlow", {}, "Retrieving tokens from " + o), i = $u(this._config) ? this._cognitoClientId : this._config.clientID, a = $u(this._config) ? this._config.redirectSignIn : this._config.redirectUri, s = function() {
                                             var e = window.sessionStorage.getItem("ouath_pkce_key");
                                             return window.sessionStorage.removeItem("ouath_pkce_key"), e
-                                        }(), u = Vu({
+                                        }(), u = Zu({
                                             grant_type: "authorization_code",
                                             code: t,
                                             client_id: i,
                                             redirect_uri: a
                                         }, s ? {
                                             code_verifier: s
-                                        } : {}), Up.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
-                                            var t = Ju(e, 2),
+                                        } : {}), Pp.debug("Calling token endpoint: " + o + " with", u), l = Object.entries(u).map((function(e) {
+                                            var t = Ku(e, 2),
                                                 n = t[0],
                                                 r = t[1];
                                             return encodeURIComponent(n) + "=" + encodeURIComponent(r)
                                         })).join("&"), c = {
-                                            category: Dl.Auth,
-                                            action: kl.FederatedSignIn
+                                            category: Ll.Auth,
+                                            action: Cl.FederatedSignIn
                                         }, [4, fetch(o, {
                                             method: "POST",
                                             headers: (y = {
                                                 "Content-Type": "application/x-www-form-urlencoded"
-                                            }, y["x-amz-user-agent"] = Xc(c), y),
+                                            }, y["x-amz-user-agent"] = $c(c), y),
                                             body: l
                                         })]) : [2];
                                     case 1:
                                         return [4, m.sent().json()];
                                     case 2:
                                         if (d = m.sent(), p = d.access_token, f = d.refresh_token, h = d.id_token, g = d.error) throw new Error(g);
                                         return [2, {
@@ -63628,70 +63631,70 @@
                                             refreshToken: f,
                                             idToken: h
                                         }]
                                 }
                             }))
                         }))
                     }, e.prototype._handleImplicitFlow = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t, n, r;
-                            return qu(this, (function(o) {
-                                return t = ((0, Ap.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                            return Ju(this, (function(o) {
+                                return t = ((0, zp.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                     return e.split("=")
                                 })).reduce((function(e, t) {
-                                    var n, r = Ju(t, 2),
+                                    var n, r = Ku(t, 2),
                                         o = r[0],
                                         i = r[1];
-                                    return Vu(Vu({}, e), ((n = {})[o] = i, n))
+                                    return Zu(Zu({}, e), ((n = {})[o] = i, n))
                                 }), {
                                     id_token: void 0,
                                     access_token: void 0
-                                }), n = t.id_token, r = t.access_token, _p("implicitFlow", {}, "Got tokens from " + e), Up.debug("Retrieving implicit tokens from " + e + " with"), [2, {
+                                }), n = t.id_token, r = t.access_token, Up("implicitFlow", {}, "Got tokens from " + e), Pp.debug("Retrieving implicit tokens from " + e + " with"), [2, {
                                     accessToken: r,
                                     idToken: n,
                                     refreshToken: null
                                 }]
                             }))
                         }))
                     }, e.prototype.handleAuthResponse = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s;
-                            return qu(this, (function(u) {
+                            return Ju(this, (function(u) {
                                 switch (u.label) {
                                     case 0:
-                                        if (u.trys.push([0, 5, , 6]), t = e ? Vu(Vu({}, ((0, Ap.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
+                                        if (u.trys.push([0, 5, , 6]), t = e ? Zu(Zu({}, ((0, zp.Qc)(e).hash || "#").substr(1).split("&").map((function(e) {
                                                 return e.split("=")
                                             })).reduce((function(e, t) {
-                                                var n = Ju(t, 2),
+                                                var n = Ku(t, 2),
                                                     r = n[0],
                                                     o = n[1];
                                                 return e[r] = o, e
-                                            }), {})), ((0, Ap.Qc)(e).query || "").split("&").map((function(e) {
+                                            }), {})), ((0, zp.Qc)(e).query || "").split("&").map((function(e) {
                                                 return e.split("=")
                                             })).reduce((function(e, t) {
-                                                var n = Ju(t, 2),
+                                                var n = Ku(t, 2),
                                                     r = n[0],
                                                     o = n[1];
                                                 return e[r] = o, e
                                             }), {})) : {}, n = t.error, r = t.error_description, n) throw new Error(r);
-                                        return o = this._validateState(t), Up.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
+                                        return o = this._validateState(t), Pp.debug("Starting " + this._config.responseType + " flow with " + e), "code" !== this._config.responseType ? [3, 2] : (i = [{}], [4, this._handleCodeFlow(e)]);
                                     case 1:
-                                        return [2, Vu.apply(void 0, [Vu.apply(void 0, i.concat([u.sent()])), {
+                                        return [2, Zu.apply(void 0, [Zu.apply(void 0, i.concat([u.sent()])), {
                                             state: o
                                         }])];
                                     case 2:
                                         return a = [{}], [4, this._handleImplicitFlow(e)];
                                     case 3:
-                                        return [2, Vu.apply(void 0, [Vu.apply(void 0, a.concat([u.sent()])), {
+                                        return [2, Zu.apply(void 0, [Zu.apply(void 0, a.concat([u.sent()])), {
                                             state: o
                                         }])];
                                     case 4:
                                         return [3, 6];
                                     case 5:
-                                        throw s = u.sent(), Up.debug("Error handling auth response.", s), s;
+                                        throw s = u.sent(), Pp.debug("Error handling auth response.", s), s;
                                     case 6:
                                         return [2]
                                 }
                             }))
                         }))
                     }, e.prototype._validateState = function(e) {
                         if (e) {
@@ -63700,33 +63703,33 @@
                                     return window.sessionStorage.removeItem("oauth_state"), e
                                 }(),
                                 n = e.state;
                             if (t && t !== n) throw new Error("Invalid state in OAuth flow");
                             return n
                         }
                     }, e.prototype.signOut = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t, n;
-                            return qu(this, (function(r) {
-                                return e = "https://" + this._config.domain + "/logout?", t = Xu(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = Xu(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
+                            return Ju(this, (function(r) {
+                                return e = "https://" + this._config.domain + "/logout?", t = $u(this._config) ? this._cognitoClientId : this._config.oauth.clientID, n = $u(this._config) ? this._config.redirectSignOut : this._config.returnTo, e += Object.entries({
                                     client_id: t,
                                     logout_uri: encodeURIComponent(n)
                                 }).map((function(e) {
-                                    var t = Ju(e, 2);
+                                    var t = Ku(e, 2);
                                     return t[0] + "=" + t[1]
-                                })).join("&"), _p("oAuthSignOut", {
+                                })).join("&"), Up("oAuthSignOut", {
                                     oAuth: "signOut"
-                                }, "Signing out from " + e), Up.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
+                                }, "Signing out from " + e), Pp.debug("Signing out from " + e), [2, this._urlOpener(e, n)]
                             }))
                         }))
                     }, e.prototype._generateState = function(e) {
                         for (var t = "", n = e, r = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"; n > 0; --n) t += r[Math.round(61 * Math.random())];
                         return t
                     }, e.prototype._generateChallenge = function(e) {
-                        var t = new Od.Sha256;
+                        var t = new _d.Sha256;
                         t.update(e);
                         var n = t.digestSync(),
                             r = Mt.lW.from(n).toString("base64");
                         return this._base64URL(r)
                     }, e.prototype._base64URL = function(e) {
                         return e.replace(/=/g, "").replace(/\+/g, "-").replace(/\//g, "_")
                     }, e.prototype._generateRandom = function(e) {
@@ -63739,126 +63742,126 @@
                         for (var t = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789", n = [], r = 0; r < e.byteLength; r += 1) {
                             var o = e[r] % 62;
                             n.push(t[o])
                         }
                         return n.join("")
                     }, e
                 }(),
-                Rp = Pp;
+                Fp = Rp;
             ! function(e) {
                 e.DEFAULT_MSG = "Authentication Error", e.EMPTY_EMAIL = "Email cannot be empty", e.EMPTY_PHONE = "Phone number cannot be empty", e.EMPTY_USERNAME = "Username cannot be empty", e.INVALID_USERNAME = "The username should either be a string or one of the sign in types", e.EMPTY_PASSWORD = "Password cannot be empty", e.EMPTY_CODE = "Confirmation code cannot be empty", e.SIGN_UP_ERROR = "Error creating account", e.NO_MFA = "No valid MFA method provided", e.INVALID_MFA = "Invalid MFA type", e.EMPTY_CHALLENGE = "Challenge response cannot be empty", e.NO_USER_SESSION = "Failed to get the session because the user is empty", e.NETWORK_ERROR = "Network Error", e.DEVICE_CONFIG = "Device tracking has not been configured in this User Pool", e.AUTOSIGNIN_ERROR = "Please use your credentials to sign in"
-            }(kp || (kp = {}));
-            var Fp = new ol("AuthError"),
-                Bp = function(e) {
+            }(Cp || (Cp = {}));
+            var Bp = new il("AuthError"),
+                Yp = function(e) {
                     function t(n) {
                         var r = this,
-                            o = Qp[n],
+                            o = Gp[n],
                             i = o.message,
                             a = o.log;
-                        return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, Fp.error(r.log), r
+                        return (r = e.call(this, i) || this).constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "AuthError", r.log = a || i, Bp.error(r.log), r
                     }
-                    return Qu(t, e), t
+                    return Gu(t, e), t
                 }(Error),
-                Yp = function(e) {
+                Qp = function(e) {
                     function t(n) {
                         var r = e.call(this, n) || this;
                         return r.constructor = t, Object.setPrototypeOf(r, t.prototype), r.name = "NoUserPoolError", r
                     }
-                    return Qu(t, e), t
-                }(Bp),
-                Qp = {
+                    return Gu(t, e), t
+                }(Yp),
+                Gp = {
                     noConfig: {
-                        message: kp.DEFAULT_MSG,
+                        message: Cp.DEFAULT_MSG,
                         log: "\n            Error: Amplify has not been configured correctly.\n            This error is typically caused by one of the following scenarios:\n\n            1. Make sure you're passing the awsconfig object to Amplify.configure() in your app's entry point\n                See https://aws-amplify.github.io/docs/js/authentication#configure-your-app for more information\n            \n            2. There might be multiple conflicting versions of amplify packages in your node_modules.\n\t\t\t\tRefer to our docs site for help upgrading Amplify packages (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js)\n        "
                     },
                     missingAuthConfig: {
-                        message: kp.DEFAULT_MSG,
+                        message: Cp.DEFAULT_MSG,
                         log: "\n            Error: Amplify has not been configured correctly. \n            The configuration object is missing required auth properties.\n            This error is typically caused by one of the following scenarios:\n\n            1. Did you run `amplify push` after adding auth via `amplify add auth`?\n                See https://aws-amplify.github.io/docs/js/authentication#amplify-project-setup for more information\n\n            2. This could also be caused by multiple conflicting versions of amplify packages, see (https://docs.amplify.aws/lib/troubleshooting/upgrading/q/platform/js) for help upgrading Amplify packages.\n        "
                     },
                     emptyUsername: {
-                        message: kp.EMPTY_USERNAME
+                        message: Cp.EMPTY_USERNAME
                     },
                     invalidUsername: {
-                        message: kp.INVALID_USERNAME
+                        message: Cp.INVALID_USERNAME
                     },
                     emptyPassword: {
-                        message: kp.EMPTY_PASSWORD
+                        message: Cp.EMPTY_PASSWORD
                     },
                     emptyCode: {
-                        message: kp.EMPTY_CODE
+                        message: Cp.EMPTY_CODE
                     },
                     signUpError: {
-                        message: kp.SIGN_UP_ERROR,
+                        message: Cp.SIGN_UP_ERROR,
                         log: "The first parameter should either be non-null string or object"
                     },
                     noMFA: {
-                        message: kp.NO_MFA
+                        message: Cp.NO_MFA
                     },
                     invalidMFA: {
-                        message: kp.INVALID_MFA
+                        message: Cp.INVALID_MFA
                     },
                     emptyChallengeResponse: {
-                        message: kp.EMPTY_CHALLENGE
+                        message: Cp.EMPTY_CHALLENGE
                     },
                     noUserSession: {
-                        message: kp.NO_USER_SESSION
+                        message: Cp.NO_USER_SESSION
                     },
                     deviceConfig: {
-                        message: kp.DEVICE_CONFIG
+                        message: Cp.DEVICE_CONFIG
                     },
                     networkError: {
-                        message: kp.NETWORK_ERROR
+                        message: Cp.NETWORK_ERROR
                     },
                     autoSignInError: {
-                        message: kp.AUTOSIGNIN_ERROR
+                        message: Cp.AUTOSIGNIN_ERROR
                     },
                     default: {
-                        message: kp.DEFAULT_MSG
+                        message: Cp.DEFAULT_MSG
                     }
                 },
-                Gp = new ol("AuthClass"),
-                Wp = "aws.cognito.signin.user.admin",
-                Hp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
-                Vp = function(e, t, n) {
-                    dl.dispatch("auth", {
+                Wp = new il("AuthClass"),
+                Hp = "aws.cognito.signin.user.admin",
+                Vp = "undefined" !== typeof Symbol && "function" === typeof Symbol.for ? Symbol.for("amplify_default") : "@@amplify_default",
+                Zp = function(e, t, n) {
+                    pl.dispatch("auth", {
                         event: e,
                         data: t,
                         message: n
-                    }, "Auth", Hp)
+                    }, "Auth", Vp)
                 },
-                Zp = function() {
+                qp = function() {
                     function e(e) {
                         var t = this;
-                        this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = Id, this.wrapRefreshSessionCallback = function(e) {
+                        this.userPool = null, this.user = null, this.oAuthFlowInProgress = !1, this.autoSignInInitiated = !1, this.inflightSessionPromise = null, this.inflightSessionPromiseCounter = 0, this.Credentials = Dd, this.wrapRefreshSessionCallback = function(e) {
                             return function(t, n) {
-                                return n ? Vp("tokenRefresh", void 0, "New token retrieved") : Vp("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
+                                return n ? Zp("tokenRefresh", void 0, "New token retrieved") : Zp("tokenRefresh_failure", t, "Failed to retrieve new token"), e(t, n)
                             }
-                        }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), dl.listen("auth", (function(e) {
+                        }, this.configure(e), this.currentCredentials = this.currentCredentials.bind(this), this.currentUserCredentials = this.currentUserCredentials.bind(this), pl.listen("auth", (function(e) {
                             switch (e.payload.event) {
                                 case "verify":
                                 case "signIn":
                                     t._storage.setItem("amplify-signin-with-hostedUI", "false");
                                     break;
                                 case "signOut":
                                     t._storage.removeItem("amplify-signin-with-hostedUI");
                                     break;
                                 case "cognitoHostedUI":
                                     t._storage.setItem("amplify-signin-with-hostedUI", "true")
                             }
-                        })), gp.category = "auth", yp(Kc.framework), Kc.observeFrameworkChanges((function() {
-                            yp(Kc.framework)
+                        })), yp.category = "auth", mp(Xc.framework), Xc.observeFrameworkChanges((function() {
+                            mp(Xc.framework)
                         }))
                     }
                     return e.prototype.getModuleName = function() {
                         return "Auth"
                     }, e.prototype.configure = function(e) {
                         var t = this;
                         if (!e) return this._config || {};
-                        Gp.debug("configure Auth");
-                        var n = Object.assign({}, this._config, vd(e).Auth, e);
+                        Wp.debug("configure Auth");
+                        var n = Object.assign({}, this._config, Md(e).Auth, e);
                         this._config = n;
                         var r = this._config,
                             o = r.userPoolId,
                             i = r.userPoolWebClientId,
                             a = r.cookieStorage,
                             s = r.oauth,
                             u = r.region,
@@ -63866,64 +63869,64 @@
                             c = r.mandatorySignIn,
                             d = r.refreshHandlers,
                             p = r.identityPoolRegion,
                             f = r.clientMetadata,
                             h = r.endpoint,
                             g = r.storage;
                         if (g) {
-                            if (!this._isValidAuthStorage(g)) throw Gp.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
+                            if (!this._isValidAuthStorage(g)) throw Wp.error("The storage in the Auth config is not valid!"), new Error("Empty storage object");
                             this._storage = g
-                        } else this._storage = a ? new Tp(a) : e.ssr ? new Sd : (new hl).getStorage();
+                        } else this._storage = a ? new Ap(a) : e.ssr ? new kd : (new gl).getStorage();
                         if (this._storageSync = Promise.resolve(), "function" === typeof this._storage.sync && (this._storageSync = this._storage.sync()), o) {
                             var y = {
                                 UserPoolId: o,
                                 ClientId: i,
                                 endpoint: h
                             };
-                            y.Storage = this._storage, this.userPool = new Cp(y, this.wrapRefreshSessionCallback)
+                            y.Storage = this._storage, this.userPool = new Ep(y, this.wrapRefreshSessionCallback)
                         }
                         this.Credentials.configure({
                             mandatorySignIn: c,
                             region: u,
                             userPoolId: o,
                             identityPoolId: l,
                             refreshHandlers: d,
                             storage: this._storage,
                             identityPoolRegion: p
                         });
-                        var m = s ? Xu(this._config.oauth) ? s : s.awsCognito : void 0;
+                        var m = s ? $u(this._config.oauth) ? s : s.awsCognito : void 0;
                         if (m) {
                             var v = Object.assign({
                                 cognitoClientId: i,
                                 UserPoolId: o,
                                 domain: m.domain,
                                 scopes: m.scope,
                                 redirectSignIn: m.redirectSignIn,
                                 redirectSignOut: m.redirectSignOut,
                                 responseType: m.responseType,
                                 Storage: this._storage,
                                 urlOpener: m.urlOpener,
                                 clientMetadata: f
                             }, m.options);
-                            this._oAuthHandler = new Rp({
+                            this._oAuthHandler = new Fp({
                                 scopes: v.scopes,
                                 config: v,
                                 cognitoClientId: v.cognitoClientId
                             });
                             var M = {};
                             ! function(e) {
-                                if (gl().isBrowser && window.location) e({
+                                if (yl().isBrowser && window.location) e({
                                     url: window.location.href
                                 });
-                                else if (!gl().isNode) throw new Error("Not supported")
+                                else if (!yl().isNode) throw new Error("Not supported")
                             }((function(e) {
                                 var n = e.url;
                                 M[n] || (M[n] = !0, t._handleAuthResponse(n))
                             }))
-                        }(Vp("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (Vp("autoSignIn_failure", null, Wu.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
+                        }(Zp("configured", null, "The Auth category has been configured successfully"), this.autoSignInInitiated || "function" !== typeof this._storage.getItem) || (this.isTrueStorageValue("amplify-polling-started") && (Zp("autoSignIn_failure", null, Hu.AutoSignInError), this._storage.removeItem("amplify-auto-sign-in")), this._storage.removeItem("amplify-polling-started"));
                         return this._config
                     }, e.prototype.signUp = function(e) {
                         for (var t, n, r, o = this, i = [], a = 1; a < arguments.length; a++) i[a - 1] = arguments[a];
                         if (!this.userPool) return this.rejectNoUserPool();
                         var s, u = null,
                             l = null,
                             c = [],
@@ -63933,187 +63936,187 @@
                             },
                             f = {},
                             h = {};
                         if (e && "string" === typeof e) {
                             u = e, l = i ? i[0] : null;
                             var g = i ? i[1] : null,
                                 y = i ? i[2] : null;
-                            g && c.push(new lp({
+                            g && c.push(new cp({
                                 Name: "email",
                                 Value: g
-                            })), y && c.push(new lp({
+                            })), y && c.push(new cp({
                                 Name: "phone_number",
                                 Value: y
                             }))
                         } else {
-                            if (!e || "object" !== typeof e) return this.rejectAuthError(Wu.SignUpError);
+                            if (!e || "object" !== typeof e) return this.rejectAuthError(Hu.SignUpError);
                             u = e.username, l = e.password, e && e.clientMetadata ? s = e.clientMetadata : this._config.clientMetadata && (s = this._config.clientMetadata);
                             var m = e.attributes;
                             m && Object.keys(m).map((function(e) {
-                                c.push(new lp({
+                                c.push(new cp({
                                     Name: e,
                                     Value: m[e]
                                 }))
                             }));
                             var v = e.validationData;
                             v && (d = [], Object.keys(v).map((function(e) {
-                                d.push(new lp({
+                                d.push(new cp({
                                     Name: e,
                                     Value: v[e]
                                 }))
                             }))), (p = null !== (t = e.autoSignIn) && void 0 !== t ? t : {
                                 enabled: !1
                             }).enabled && (this._storage.setItem("amplify-auto-sign-in", "true"), f = null !== (n = p.validationData) && void 0 !== n ? n : {}, h = null !== (r = p.clientMetaData) && void 0 !== r ? r : {})
                         }
-                        return u ? l ? (Gp.debug("signUp attrs:", c), Gp.debug("signUp validation data:", d), new Promise((function(e, t) {
+                        return u ? l ? (Wp.debug("signUp attrs:", c), Wp.debug("signUp validation data:", d), new Promise((function(e, t) {
                             o.userPool.signUp(u, l, c, d, (function(n, r) {
-                                n ? (Vp("signUp_failure", n, u + " failed to signup"), t(n)) : (Vp("signUp", r, u + " has signed up successfully"), p.enabled && o.handleAutoSignIn(u, l, f, h, r), e(r))
+                                n ? (Zp("signUp_failure", n, u + " failed to signup"), t(n)) : (Zp("signUp", r, u + " has signed up successfully"), p.enabled && o.handleAutoSignIn(u, l, f, h, r), e(r))
                             }), s)
-                        }))) : this.rejectAuthError(Wu.EmptyPassword) : this.rejectAuthError(Wu.EmptyUsername)
+                        }))) : this.rejectAuthError(Hu.EmptyPassword) : this.rejectAuthError(Hu.EmptyUsername)
                     }, e.prototype.handleAutoSignIn = function(e, t, n, r, o) {
                         this.autoSignInInitiated = !0;
-                        var i = new Cd({
+                        var i = new Ed({
                             Username: e,
                             Password: t,
                             ValidationData: n,
                             ClientMetadata: r
                         });
                         o.userConfirmed ? this.signInAfterUserConfirmed(i) : "link" === this._config.signUpVerificationMethod ? this.handleLinkAutoSignIn(i) : this.handleCodeAutoSignIn(i)
                     }, e.prototype.handleCodeAutoSignIn = function(e) {
                         var t = this;
-                        dl.listen("auth", (function n(r) {
+                        pl.listen("auth", (function n(r) {
                             "confirmSignUp" === r.payload.event && t.signInAfterUserConfirmed(e, n)
                         }))
                     }, e.prototype.handleLinkAutoSignIn = function(e) {
                         var t = this;
                         this._storage.setItem("amplify-polling-started", "true");
                         var n = Date.now(),
                             r = setInterval((function() {
-                                Date.now() - n > 18e4 ? (clearInterval(r), Vp("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
+                                Date.now() - n > 18e4 ? (clearInterval(r), Zp("autoSignIn_failure", null, "Please confirm your account and use your credentials to sign in."), t._storage.removeItem("amplify-auto-sign-in")) : t.signInAfterUserConfirmed(e, null, r)
                             }), 5e3)
                     }, e.prototype.signInAfterUserConfirmed = function(e, t, n) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var r, o, i = this;
-                            return qu(this, (function(a) {
+                            return Ju(this, (function(a) {
                                 switch (a.label) {
                                     case 0:
                                         r = this.createCognitoUser(e.getUsername()), a.label = 1;
                                     case 1:
                                         return a.trys.push([1, 3, , 4]), [4, r.authenticateUser(e, this.authCallbacks(r, (function(r) {
-                                            Vp("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && dl.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
+                                            Zp("autoSignIn", r, e.getUsername() + " has signed in successfully"), t && pl.remove("auth", t), n && (clearInterval(n), i._storage.removeItem("amplify-polling-started")), i._storage.removeItem("amplify-auto-sign-in")
                                         }), (function(e) {
-                                            Gp.error(e), i._storage.removeItem("amplify-auto-sign-in")
+                                            Wp.error(e), i._storage.removeItem("amplify-auto-sign-in")
                                         })))];
                                     case 2:
                                         return a.sent(), [3, 4];
                                     case 3:
-                                        return o = a.sent(), Gp.error(o), [3, 4];
+                                        return o = a.sent(), Wp.error(o), [3, 4];
                                     case 4:
                                         return [2]
                                 }
                             }))
                         }))
                     }, e.prototype.confirmSignUp = function(e, t, n) {
                         var r = this;
                         if (!this.userPool) return this.rejectNoUserPool();
-                        if (!e) return this.rejectAuthError(Wu.EmptyUsername);
-                        if (!t) return this.rejectAuthError(Wu.EmptyCode);
+                        if (!e) return this.rejectAuthError(Hu.EmptyUsername);
+                        if (!t) return this.rejectAuthError(Hu.EmptyCode);
                         var o, i = this.createCognitoUser(e),
                             a = !n || "boolean" !== typeof n.forceAliasCreation || n.forceAliasCreation;
                         return n && n.clientMetadata ? o = n.clientMetadata : this._config.clientMetadata && (o = this._config.clientMetadata), new Promise((function(n, s) {
                             i.confirmRegistration(t, a, (function(t, o) {
-                                t ? s(t) : (Vp("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (Vp("autoSignIn_failure", null, Wu.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
+                                t ? s(t) : (Zp("confirmSignUp", o, e + " has been confirmed successfully"), r.isTrueStorageValue("amplify-auto-sign-in") && !r.autoSignInInitiated && (Zp("autoSignIn_failure", null, Hu.AutoSignInError), r._storage.removeItem("amplify-auto-sign-in")), n(o))
                             }), o)
                         }))
                     }, e.prototype.isTrueStorageValue = function(e) {
                         var t = this._storage.getItem(e);
                         return !!t && "true" === t
                     }, e.prototype.resendSignUp = function(e, t) {
                         if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                        if (!e) return this.rejectAuthError(Wu.EmptyUsername);
+                        if (!e) return this.rejectAuthError(Hu.EmptyUsername);
                         var n = this.createCognitoUser(e);
                         return new Promise((function(e, r) {
                             n.resendConfirmationCode((function(t, n) {
                                 t ? r(t) : e(n)
                             }), t)
                         }))
                     }, e.prototype.signIn = function(e, t, n) {
                         if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
                         var r = null,
                             o = null,
                             i = {};
                         if ("string" === typeof e) r = e, o = t;
                         else {
-                            if (!e.username) return this.rejectAuthError(Wu.InvalidUsername);
-                            "undefined" !== typeof t && Gp.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
+                            if (!e.username) return this.rejectAuthError(Hu.InvalidUsername);
+                            "undefined" !== typeof t && Wp.warn("The password should be defined under the first parameter object!"), r = e.username, o = e.password, i = e.validationData
                         }
-                        if (!r) return this.rejectAuthError(Wu.EmptyUsername);
-                        var a = new Cd({
+                        if (!r) return this.rejectAuthError(Hu.EmptyUsername);
+                        var a = new Ed({
                             Username: r,
                             Password: o,
                             ValidationData: i,
                             ClientMetadata: n
                         });
                         return o ? this.signInWithPassword(a) : this.signInWithoutPassword(a)
                     }, e.prototype.authCallbacks = function(e, t, n) {
                         var r = this,
                             o = this;
                         return {
                             onSuccess: function(i) {
-                                return Zu(r, void 0, void 0, (function() {
+                                return qu(r, void 0, void 0, (function() {
                                     var r, a, s, u;
-                                    return qu(this, (function(l) {
+                                    return Ju(this, (function(l) {
                                         switch (l.label) {
                                             case 0:
-                                                Gp.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
+                                                Wp.debug(i), delete e.challengeName, delete e.challengeParam, l.label = 1;
                                             case 1:
                                                 return l.trys.push([1, 4, 5, 9]), [4, this.Credentials.clear()];
                                             case 2:
                                                 return l.sent(), [4, this.Credentials.set(i, "session")];
                                             case 3:
-                                                return r = l.sent(), Gp.debug("succeed to get cognito credentials", r), [3, 9];
+                                                return r = l.sent(), Wp.debug("succeed to get cognito credentials", r), [3, 9];
                                             case 4:
-                                                return a = l.sent(), Gp.debug("cannot get cognito credentials", a), [3, 9];
+                                                return a = l.sent(), Wp.debug("cannot get cognito credentials", a), [3, 9];
                                             case 5:
                                                 return l.trys.push([5, 7, , 8]), [4, this.currentUserPoolUser()];
                                             case 6:
-                                                return s = l.sent(), o.user = s, Vp("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
+                                                return s = l.sent(), o.user = s, Zp("signIn", s, "A user " + e.getUsername() + " has been signed in"), t(s), [3, 8];
                                             case 7:
-                                                return u = l.sent(), Gp.error("Failed to get the signed in user", u), n(u), [3, 8];
+                                                return u = l.sent(), Wp.error("Failed to get the signed in user", u), n(u), [3, 8];
                                             case 8:
                                                 return [7];
                                             case 9:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             },
                             onFailure: function(t) {
-                                Gp.debug("signIn failure", t), Vp("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
+                                Wp.debug("signIn failure", t), Zp("signIn_failure", t, e.getUsername() + " failed to signin"), n(t)
                             },
                             customChallenge: function(n) {
-                                Gp.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
+                                Wp.debug("signIn custom challenge answer required"), e.challengeName = "CUSTOM_CHALLENGE", e.challengeParam = n, t(e)
                             },
                             mfaRequired: function(n, r) {
-                                Gp.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
+                                Wp.debug("signIn MFA required"), e.challengeName = n, e.challengeParam = r, t(e)
                             },
                             mfaSetup: function(n, r) {
-                                Gp.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
+                                Wp.debug("signIn mfa setup", n), e.challengeName = n, e.challengeParam = r, t(e)
                             },
                             newPasswordRequired: function(n, r) {
-                                Gp.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
+                                Wp.debug("signIn new password"), e.challengeName = "NEW_PASSWORD_REQUIRED", e.challengeParam = {
                                     userAttributes: n,
                                     requiredAttributes: r
                                 }, t(e)
                             },
                             totpRequired: function(n, r) {
-                                Gp.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
+                                Wp.debug("signIn totpRequired"), e.challengeName = n, e.challengeParam = r, t(e)
                             },
                             selectMFAType: function(n, r) {
-                                Gp.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
+                                Wp.debug("signIn selectMFAType", n), e.challengeName = n, e.challengeParam = r, t(e)
                             }
                         }
                     }, e.prototype.signInWithPassword = function(e) {
                         var t = this;
                         if (this.pendingSignIn) throw new Error("Pending sign-in attempt already in progress");
                         var n = this.createCognitoUser(e.getUsername());
                         return this.pendingSignIn = new Promise((function(r, o) {
@@ -64128,32 +64131,32 @@
                             n = this.createCognitoUser(e.getUsername());
                         return n.setAuthenticationFlowType("CUSTOM_AUTH"), new Promise((function(r, o) {
                             n.initiateAuth(e, t.authCallbacks(n, r, o))
                         }))
                     }, e.prototype.getMFAOptions = function(e) {
                         return new Promise((function(t, n) {
                             e.getMFAOptions((function(e, r) {
-                                if (e) return Gp.debug("get MFA Options failed", e), void n(e);
-                                Gp.debug("get MFA options success", r), t(r)
+                                if (e) return Wp.debug("get MFA Options failed", e), void n(e);
+                                Wp.debug("get MFA options success", r), t(r)
                             }))
                         }))
                     }, e.prototype.getPreferredMFA = function(e, t) {
                         var n = this,
                             r = this;
                         return new Promise((function(o, i) {
                             var a = n._config.clientMetadata,
                                 s = !!t && t.bypassCache;
                             e.getUserData((function(t, a) {
-                                return Zu(n, void 0, void 0, (function() {
+                                return qu(n, void 0, void 0, (function() {
                                     var n, s;
-                                    return qu(this, (function(u) {
+                                    return Ju(this, (function(u) {
                                         switch (u.label) {
                                             case 0:
                                                 if (!t) return [3, 5];
-                                                if (Gp.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                                if (Wp.debug("getting preferred mfa failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                                 u.label = 1;
                                             case 1:
                                                 return u.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                             case 2:
                                                 return u.sent(), [3, 4];
                                             case 3:
                                                 return n = u.sent(), i(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -64171,29 +64174,29 @@
                         }))
                     }, e.prototype._getMfaTypeFromUserData = function(e) {
                         var t = null,
                             n = e.PreferredMfaSetting;
                         if (n) t = n;
                         else {
                             var r = e.UserMFASettingList;
-                            if (r) 0 === r.length ? t = "NOMFA" : Gp.debug("invalid case for getPreferredMFA", e);
+                            if (r) 0 === r.length ? t = "NOMFA" : Wp.debug("invalid case for getPreferredMFA", e);
                             else t = e.MFAOptions ? "SMS_MFA" : "NOMFA"
                         }
                         return t
                     }, e.prototype._getUserData = function(e, t) {
                         var n = this;
                         return new Promise((function(r, o) {
                             e.getUserData((function(t, i) {
-                                return Zu(n, void 0, void 0, (function() {
+                                return qu(n, void 0, void 0, (function() {
                                     var n;
-                                    return qu(this, (function(a) {
+                                    return Ju(this, (function(a) {
                                         switch (a.label) {
                                             case 0:
                                                 if (!t) return [3, 5];
-                                                if (Gp.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
+                                                if (Wp.debug("getting user data failed", t), !this.isSessionInvalid(t)) return [3, 4];
                                                 a.label = 1;
                                             case 1:
                                                 return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                             case 2:
                                                 return a.sent(), [3, 4];
                                             case 3:
                                                 return n = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + n.message)), [2];
@@ -64205,17 +64208,17 @@
                                                 return [2]
                                         }
                                     }))
                                 }))
                             }), t)
                         }))
                     }, e.prototype.setPreferredMFA = function(e, t) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var n, r, o, i, a, s, u = this;
-                            return qu(this, (function(l) {
+                            return Ju(this, (function(l) {
                                 switch (l.label) {
                                     case 0:
                                         return n = this._config.clientMetadata, [4, this._getUserData(e, {
                                             bypassCache: !0,
                                             clientMetadata: n
                                         })];
                                     case 1:
@@ -64245,15 +64248,15 @@
                                     case 5:
                                         if ("NOMFA" === (s = l.sent())) return [2, Promise.resolve("No change for mfa type")];
                                         if ("SMS_MFA" === s) o = {
                                             PreferredMfa: !1,
                                             Enabled: !1
                                         };
                                         else {
-                                            if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(Wu.InvalidMFA)];
+                                            if ("SOFTWARE_TOKEN_MFA" !== s) return [2, this.rejectAuthError(Hu.InvalidMFA)];
                                             i = {
                                                 PreferredMfa: !1,
                                                 Enabled: !1
                                             }
                                         }
                                         return a && 0 !== a.length && a.forEach((function(e) {
                                             "SMS_MFA" === e ? o = {
@@ -64261,27 +64264,27 @@
                                                 Enabled: !1
                                             } : "SOFTWARE_TOKEN_MFA" === e && (i = {
                                                 PreferredMfa: !1,
                                                 Enabled: !1
                                             })
                                         })), [3, 7];
                                     case 6:
-                                        return Gp.debug("no validmfa method provided"), [2, this.rejectAuthError(Wu.NoMFA)];
+                                        return Wp.debug("no validmfa method provided"), [2, this.rejectAuthError(Hu.NoMFA)];
                                     case 7:
                                         return this, [2, new Promise((function(t, r) {
                                             e.setUserMfaPreference(o, i, (function(o, i) {
-                                                if (o) return Gp.debug("Set user mfa preference error", o), r(o);
-                                                Gp.debug("Set user mfa success", i), Gp.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
-                                                    return Zu(u, void 0, void 0, (function() {
+                                                if (o) return Wp.debug("Set user mfa preference error", o), r(o);
+                                                Wp.debug("Set user mfa success", i), Wp.debug("Caching the latest user data into local"), e.getUserData((function(n, o) {
+                                                    return qu(u, void 0, void 0, (function() {
                                                         var o;
-                                                        return qu(this, (function(a) {
+                                                        return Ju(this, (function(a) {
                                                             switch (a.label) {
                                                                 case 0:
                                                                     if (!n) return [3, 5];
-                                                                    if (Gp.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
+                                                                    if (Wp.debug("getting user data failed", n), !this.isSessionInvalid(n)) return [3, 4];
                                                                     a.label = 1;
                                                                 case 1:
                                                                     return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                                 case 2:
                                                                     return a.sent(), [3, 4];
                                                                 case 3:
                                                                     return o = a.sent(), r(new Error("Session is invalid due to: " + n.message + " and failed to clean up invalid session: " + o.message)), [2];
@@ -64300,206 +64303,206 @@
                                         }))]
                                 }
                             }))
                         }))
                     }, e.prototype.disableSMS = function(e) {
                         return new Promise((function(t, n) {
                             e.disableMFA((function(e, r) {
-                                if (e) return Gp.debug("disable mfa failed", e), void n(e);
-                                Gp.debug("disable mfa succeed", r), t(r)
+                                if (e) return Wp.debug("disable mfa failed", e), void n(e);
+                                Wp.debug("disable mfa succeed", r), t(r)
                             }))
                         }))
                     }, e.prototype.enableSMS = function(e) {
                         return new Promise((function(t, n) {
                             e.enableMFA((function(e, r) {
-                                if (e) return Gp.debug("enable mfa failed", e), void n(e);
-                                Gp.debug("enable mfa succeed", r), t(r)
+                                if (e) return Wp.debug("enable mfa failed", e), void n(e);
+                                Wp.debug("enable mfa succeed", r), t(r)
                             }))
                         }))
                     }, e.prototype.setupTOTP = function(e) {
                         return new Promise((function(t, n) {
                             e.associateSoftwareToken({
                                 onFailure: function(e) {
-                                    Gp.debug("associateSoftwareToken failed", e), n(e)
+                                    Wp.debug("associateSoftwareToken failed", e), n(e)
                                 },
                                 associateSecretCode: function(e) {
-                                    Gp.debug("associateSoftwareToken success", e), t(e)
+                                    Wp.debug("associateSoftwareToken success", e), t(e)
                                 }
                             })
                         }))
                     }, e.prototype.verifyTotpToken = function(e, t) {
                         var n;
-                        Gp.debug("verification totp token", e, t), e && "function" === typeof e.getSignInUserSession && (n = e.getSignInUserSession());
+                        Wp.debug("verification totp token", e, t), e && "function" === typeof e.getSignInUserSession && (n = e.getSignInUserSession());
                         var r = null === n || void 0 === n ? void 0 : n.isValid();
                         return new Promise((function(n, o) {
                             e.verifySoftwareToken(t, "My TOTP device", {
                                 onFailure: function(e) {
-                                    Gp.debug("verifyTotpToken failed", e), o(e)
+                                    Wp.debug("verifyTotpToken failed", e), o(e)
                                 },
                                 onSuccess: function(t) {
-                                    r || Vp("signIn", e, "A user " + e.getUsername() + " has been signed in"), Vp("verify", e, "A user " + e.getUsername() + " has been verified"), Gp.debug("verifyTotpToken success", t), n(t)
+                                    r || Zp("signIn", e, "A user " + e.getUsername() + " has been signed in"), Zp("verify", e, "A user " + e.getUsername() + " has been verified"), Wp.debug("verifyTotpToken success", t), n(t)
                                 }
                             })
                         }))
                     }, e.prototype.confirmSignIn = function(e, t, n, r) {
                         var o = this;
-                        if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Wu.EmptyCode);
+                        if (void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Hu.EmptyCode);
                         var i = this;
                         return new Promise((function(a, s) {
                             e.sendMFACode(t, {
                                 onSuccess: function(t) {
-                                    return Zu(o, void 0, void 0, (function() {
+                                    return qu(o, void 0, void 0, (function() {
                                         var n, r, o, s;
-                                        return qu(this, (function(u) {
+                                        return Ju(this, (function(u) {
                                             switch (u.label) {
                                                 case 0:
-                                                    Gp.debug(t), u.label = 1;
+                                                    Wp.debug(t), u.label = 1;
                                                 case 1:
                                                     return u.trys.push([1, 4, 5, 10]), [4, this.Credentials.clear()];
                                                 case 2:
                                                     return u.sent(), [4, this.Credentials.set(t, "session")];
                                                 case 3:
-                                                    return n = u.sent(), Gp.debug("succeed to get cognito credentials", n), [3, 10];
+                                                    return n = u.sent(), Wp.debug("succeed to get cognito credentials", n), [3, 10];
                                                 case 4:
-                                                    return r = u.sent(), Gp.debug("cannot get cognito credentials", r), [3, 10];
+                                                    return r = u.sent(), Wp.debug("cannot get cognito credentials", r), [3, 10];
                                                 case 5:
                                                     i.user = e, u.label = 6;
                                                 case 6:
                                                     return u.trys.push([6, 8, , 9]), [4, this.currentUserPoolUser()];
                                                 case 7:
                                                     return o = u.sent(), e.attributes = o.attributes, [3, 9];
                                                 case 8:
-                                                    return s = u.sent(), Gp.debug("cannot get updated Cognito User", s), [3, 9];
+                                                    return s = u.sent(), Wp.debug("cannot get updated Cognito User", s), [3, 9];
                                                 case 9:
-                                                    return Vp("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                    return Zp("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                                 case 10:
                                                     return [2]
                                             }
                                         }))
                                     }))
                                 },
                                 onFailure: function(e) {
-                                    Gp.debug("confirm signIn failure", e), s(e)
+                                    Wp.debug("confirm signIn failure", e), s(e)
                                 }
                             }, n, r)
                         }))
                     }, e.prototype.completeNewPassword = function(e, t, n, r) {
                         var o = this;
-                        if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Wu.EmptyPassword);
+                        if (void 0 === n && (n = {}), void 0 === r && (r = this._config.clientMetadata), !t) return this.rejectAuthError(Hu.EmptyPassword);
                         var i = this;
                         return new Promise((function(a, s) {
                             e.completeNewPasswordChallenge(t, n, {
                                 onSuccess: function(t) {
-                                    return Zu(o, void 0, void 0, (function() {
+                                    return qu(o, void 0, void 0, (function() {
                                         var n, r;
-                                        return qu(this, (function(o) {
+                                        return Ju(this, (function(o) {
                                             switch (o.label) {
                                                 case 0:
-                                                    Gp.debug(t), o.label = 1;
+                                                    Wp.debug(t), o.label = 1;
                                                 case 1:
                                                     return o.trys.push([1, 4, 5, 6]), [4, this.Credentials.clear()];
                                                 case 2:
                                                     return o.sent(), [4, this.Credentials.set(t, "session")];
                                                 case 3:
-                                                    return n = o.sent(), Gp.debug("succeed to get cognito credentials", n), [3, 6];
+                                                    return n = o.sent(), Wp.debug("succeed to get cognito credentials", n), [3, 6];
                                                 case 4:
-                                                    return r = o.sent(), Gp.debug("cannot get cognito credentials", r), [3, 6];
+                                                    return r = o.sent(), Wp.debug("cannot get cognito credentials", r), [3, 6];
                                                 case 5:
-                                                    return i.user = e, Vp("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
+                                                    return i.user = e, Zp("signIn", e, "A user " + e.getUsername() + " has been signed in"), a(e), [7];
                                                 case 6:
                                                     return [2]
                                             }
                                         }))
                                     }))
                                 },
                                 onFailure: function(e) {
-                                    Gp.debug("completeNewPassword failure", e), Vp("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
+                                    Wp.debug("completeNewPassword failure", e), Zp("completeNewPassword_failure", e, o.user + " failed to complete the new password flow"), s(e)
                                 },
                                 mfaRequired: function(t, n) {
-                                    Gp.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
+                                    Wp.debug("signIn MFA required"), e.challengeName = t, e.challengeParam = n, a(e)
                                 },
                                 mfaSetup: function(t, n) {
-                                    Gp.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                    Wp.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                                 },
                                 totpRequired: function(t, n) {
-                                    Gp.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
+                                    Wp.debug("signIn mfa setup", t), e.challengeName = t, e.challengeParam = n, a(e)
                                 }
                             }, r)
                         }))
                     }, e.prototype.sendCustomChallengeAnswer = function(e, t, n) {
                         var r = this;
                         if (void 0 === n && (n = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                        if (!t) return this.rejectAuthError(Wu.EmptyChallengeResponse);
+                        if (!t) return this.rejectAuthError(Hu.EmptyChallengeResponse);
                         return new Promise((function(o, i) {
                             e.sendCustomChallengeAnswer(t, r.authCallbacks(e, o, i), n)
                         }))
                     }, e.prototype.deleteUserAttributes = function(e, t) {
                         var n = this;
                         return new Promise((function(r, o) {
                             n.userSession(e).then((function(n) {
                                 e.deleteAttributes(t, (function(e, t) {
                                     return e ? o(e) : r(t)
                                 }))
                             }))
                         }))
                     }, e.prototype.deleteUser = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t, n = this;
-                            return qu(this, (function(r) {
+                            return Ju(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
                                         return r.trys.push([0, 2, , 3]), [4, this._storageSync];
                                     case 1:
                                         return r.sent(), [3, 3];
                                     case 2:
-                                        throw e = r.sent(), Gp.debug("Failed to sync cache info into memory", e), new Error(e);
+                                        throw e = r.sent(), Wp.debug("Failed to sync cache info into memory", e), new Error(e);
                                     case 3:
                                         return t = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(e, r) {
-                                            return Zu(n, void 0, void 0, (function() {
+                                            return qu(n, void 0, void 0, (function() {
                                                 var n, o = this;
-                                                return qu(this, (function(i) {
+                                                return Ju(this, (function(i) {
                                                     if (this.userPool) {
-                                                        if (!(n = this.userPool.getCurrentUser())) return Gp.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
+                                                        if (!(n = this.userPool.getCurrentUser())) return Wp.debug("Failed to get user from user pool"), [2, r(new Error("No current user."))];
                                                         n.getSession((function(i, a) {
-                                                            return Zu(o, void 0, void 0, (function() {
+                                                            return qu(o, void 0, void 0, (function() {
                                                                 var o, a = this;
-                                                                return qu(this, (function(s) {
+                                                                return Ju(this, (function(s) {
                                                                     switch (s.label) {
                                                                         case 0:
                                                                             if (!i) return [3, 5];
-                                                                            if (Gp.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
+                                                                            if (Wp.debug("Failed to get the user session", i), !this.isSessionInvalid(i)) return [3, 4];
                                                                             s.label = 1;
                                                                         case 1:
                                                                             return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(n)];
                                                                         case 2:
                                                                             return s.sent(), [3, 4];
                                                                         case 3:
                                                                             return o = s.sent(), r(new Error("Session is invalid due to: " + i.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                                         case 4:
                                                                             return [2, r(i)];
                                                                         case 5:
                                                                             n.deleteUser((function(o, i) {
                                                                                 if (o) r(o);
                                                                                 else {
-                                                                                    Vp("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
+                                                                                    Zp("userDeleted", i, "The authenticated user has been deleted."), n.signOut(), a.user = null;
                                                                                     try {
                                                                                         a.cleanCachedItems()
                                                                                     } catch (s) {
-                                                                                        Gp.debug("failed to clear cached items")
+                                                                                        Wp.debug("failed to clear cached items")
                                                                                     }
-                                                                                    t ? a.oAuthSignOutRedirect(e, r) : (Vp("signOut", a.user, "A user has been signed out"), e(i))
+                                                                                    t ? a.oAuthSignOutRedirect(e, r) : (Zp("signOut", a.user, "A user has been signed out"), e(i))
                                                                                 }
                                                                             })), s.label = 6;
                                                                         case 6:
                                                                             return [2]
                                                                     }
                                                                 }))
                                                             }))
                                                         }))
-                                                    } else Gp.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
+                                                    } else Wp.debug("no Congito User pool"), r(new Error("Cognito User pool does not exist"));
                                                     return [2]
                                                 }))
                                             }))
                                         }))]
                                 }
                             }))
                         }))
@@ -64514,17 +64517,17 @@
                                     if ("sub" !== u && u.indexOf("_verified") < 0) {
                                         var l = {
                                             Name: u,
                                             Value: t[u]
                                         };
                                         o.push(l)
                                     } e.updateAttributes(o, (function(e, n, o) {
-                                    if (e) return Vp("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
+                                    if (e) return Zp("updateUserAttributes_failure", e, "Failed to update attributes"), s(e);
                                     var i = r.createUpdateAttributesResultList(t, null === o || void 0 === o ? void 0 : o.CodeDeliveryDetailsList);
-                                    return Vp("updateUserAttributes", i, "Attributes successfully updated"), a(n)
+                                    return Zp("updateUserAttributes", i, "Attributes successfully updated"), a(n)
                                 }), n)
                             }))
                         }))
                     }, e.prototype.createUpdateAttributesResultList = function(e, t) {
                         var n = {};
                         return Object.keys(e).forEach((function(e) {
                             n[e] = {
@@ -64570,73 +64573,73 @@
                     }, e.prototype.isPasswordResetRequiredError = function(e) {
                         return this.isErrorWithMessage(e) && "Password reset required for the user" === e.message
                     }, e.prototype.isSignedInHostedUI = function() {
                         return this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI")
                     }, e.prototype.isSessionInvalid = function(e) {
                         return this.isUserDisabledError(e) || this.isUserDoesNotExistError(e) || this.isTokenRevokedError(e) || this.isRefreshTokenRevokedError(e) || this.isRefreshTokenExpiredError(e) || this.isPasswordResetRequiredError(e)
                     }, e.prototype.cleanUpInvalidSession = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t = this;
-                            return qu(this, (function(n) {
+                            return Ju(this, (function(n) {
                                 switch (n.label) {
                                     case 0:
                                         e.signOut(), this.user = null, n.label = 1;
                                     case 1:
                                         return n.trys.push([1, 3, , 4]), [4, this.cleanCachedItems()];
                                     case 2:
                                         return n.sent(), [3, 4];
                                     case 3:
-                                        return n.sent(), Gp.debug("failed to clear cached items"), [3, 4];
+                                        return n.sent(), Wp.debug("failed to clear cached items"), [3, 4];
                                     case 4:
                                         return this.isSignedInHostedUI() ? [2, new Promise((function(e, n) {
                                             t.oAuthSignOutRedirect(e, n)
-                                        }))] : (Vp("signOut", this.user, "A user has been signed out"), [2])
+                                        }))] : (Zp("signOut", this.user, "A user has been signed out"), [2])
                                 }
                             }))
                         }))
                     }, e.prototype.currentUserPoolUser = function(e) {
                         var t = this;
                         return this.userPool ? new Promise((function(n, r) {
                             t._storageSync.then((function() {
-                                return Zu(t, void 0, void 0, (function() {
+                                return qu(t, void 0, void 0, (function() {
                                     var t, o, i, a, s, u, l = this;
-                                    return qu(this, (function(c) {
+                                    return Ju(this, (function(c) {
                                         switch (c.label) {
                                             case 0:
-                                                return this.isOAuthInProgress() ? (Gp.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
+                                                return this.isOAuthInProgress() ? (Wp.debug("OAuth signIn in progress, waiting for resolution..."), [4, new Promise((function(e) {
                                                     var t = setTimeout((function() {
-                                                        Gp.debug("OAuth signIn in progress timeout"), dl.remove("auth", n), e()
+                                                        Wp.debug("OAuth signIn in progress timeout"), pl.remove("auth", n), e()
                                                     }), 1e4);
 
                                                     function n(r) {
                                                         var o = r.payload.event;
-                                                        "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Gp.debug("OAuth signIn resolved: " + o), clearTimeout(t), dl.remove("auth", n), e())
+                                                        "cognitoHostedUI" !== o && "cognitoHostedUI_failure" !== o || (Wp.debug("OAuth signIn resolved: " + o), clearTimeout(t), pl.remove("auth", n), e())
                                                     }
-                                                    dl.listen("auth", n)
+                                                    pl.listen("auth", n)
                                                 }))]) : [3, 2];
                                             case 1:
                                                 c.sent(), c.label = 2;
                                             case 2:
-                                                if (!(t = this.userPool.getCurrentUser())) return Gp.debug("Failed to get user from user pool"), r("No current user"), [2];
+                                                if (!(t = this.userPool.getCurrentUser())) return Wp.debug("Failed to get user from user pool"), r("No current user"), [2];
                                                 c.label = 3;
                                             case 3:
                                                 return c.trys.push([3, 7, , 8]), [4, this._userSession(t)];
                                             case 4:
                                                 return o = c.sent(), (i = !!e && e.bypassCache) ? [4, this.Credentials.clear()] : [3, 6];
                                             case 5:
                                                 c.sent(), c.label = 6;
                                             case 6:
-                                                return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Wp) ? (t.getUserData((function(e, o) {
-                                                    return Zu(l, void 0, void 0, (function() {
+                                                return a = this._config.clientMetadata, s = o.getAccessToken().decodePayload().scope, (void 0 === s ? "" : s).split(" ").includes(Hp) ? (t.getUserData((function(e, o) {
+                                                    return qu(l, void 0, void 0, (function() {
                                                         var i, a, s, u, l, c, d;
-                                                        return qu(this, (function(p) {
+                                                        return Ju(this, (function(p) {
                                                             switch (p.label) {
                                                                 case 0:
                                                                     if (!e) return [3, 7];
-                                                                    if (Gp.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
+                                                                    if (Wp.debug("getting user data failed", e), !this.isSessionInvalid(e)) return [3, 5];
                                                                     p.label = 1;
                                                                 case 1:
                                                                     return p.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                                 case 2:
                                                                     return p.sent(), [3, 4];
                                                                 case 3:
                                                                     return i = p.sent(), r(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + i.message)), [2];
@@ -64646,114 +64649,114 @@
                                                                     n(t), p.label = 6;
                                                                 case 6:
                                                                     return [2];
                                                                 case 7:
                                                                     for (a = o.PreferredMfaSetting || "NOMFA", s = [], u = 0; u < o.UserAttributes.length; u++) l = {
                                                                         Name: o.UserAttributes[u].Name,
                                                                         Value: o.UserAttributes[u].Value
-                                                                    }, c = new lp(l), s.push(c);
+                                                                    }, c = new cp(l), s.push(c);
                                                                     return d = this.attributesToObject(s), Object.assign(t, {
                                                                         attributes: d,
                                                                         preferredMFA: a
                                                                     }), [2, n(t)]
                                                             }
                                                         }))
                                                     }))
                                                 }), {
                                                     bypassCache: i,
                                                     clientMetadata: a
-                                                }), [3, 8]) : (Gp.debug("Unable to get the user data because the " + Wp + " is not in the scopes of the access token"), [2, n(t)]);
+                                                }), [3, 8]) : (Wp.debug("Unable to get the user data because the " + Hp + " is not in the scopes of the access token"), [2, n(t)]);
                                             case 7:
                                                 return u = c.sent(), r(u), [3, 8];
                                             case 8:
                                                 return [2]
                                         }
                                     }))
                                 }))
                             })).catch((function(e) {
-                                return Gp.debug("Failed to sync cache info into memory", e), r(e)
+                                return Wp.debug("Failed to sync cache info into memory", e), r(e)
                             }))
                         })) : this.rejectNoUserPool()
                     }, e.prototype.isOAuthInProgress = function() {
                         return this.oAuthFlowInProgress
                     }, e.prototype.currentAuthenticatedUser = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t, n, r, o, i;
-                            return qu(this, (function(a) {
+                            return Ju(this, (function(a) {
                                 switch (a.label) {
                                     case 0:
-                                        Gp.debug("getting current authenticated user"), t = null, a.label = 1;
+                                        Wp.debug("getting current authenticated user"), t = null, a.label = 1;
                                     case 1:
                                         return a.trys.push([1, 3, , 4]), [4, this._storageSync];
                                     case 2:
                                         return a.sent(), [3, 4];
                                     case 3:
-                                        throw n = a.sent(), Gp.debug("Failed to sync cache info into memory", n), n;
+                                        throw n = a.sent(), Wp.debug("Failed to sync cache info into memory", n), n;
                                     case 4:
                                         try {
-                                            (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = Vu(Vu({}, r.user), {
+                                            (r = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))) && (t = Zu(Zu({}, r.user), {
                                                 token: r.token
                                             }))
                                         } catch (s) {
-                                            Gp.debug("cannot load federated user from auth storage")
+                                            Wp.debug("cannot load federated user from auth storage")
                                         }
-                                        return t ? (this.user = t, Gp.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
+                                        return t ? (this.user = t, Wp.debug("get current authenticated federated user", this.user), [2, this.user]) : [3, 5];
                                     case 5:
-                                        Gp.debug("get current authenticated userpool user"), o = null, a.label = 6;
+                                        Wp.debug("get current authenticated userpool user"), o = null, a.label = 6;
                                     case 6:
                                         return a.trys.push([6, 8, , 9]), [4, this.currentUserPoolUser(e)];
                                     case 7:
                                         return o = a.sent(), [3, 9];
                                     case 8:
-                                        return "No userPool" === (i = a.sent()) && Gp.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Gp.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
+                                        return "No userPool" === (i = a.sent()) && Wp.error("Cannot get the current user because the user pool is missing. Please make sure the Auth module is configured with a valid Cognito User Pool ID"), Wp.debug("The user is not authenticated by the error", i), [2, Promise.reject("The user is not authenticated")];
                                     case 9:
                                         return this.user = o, [2, this.user]
                                 }
                             }))
                         }))
                     }, e.prototype.currentSession = function() {
                         var e = this;
-                        return Gp.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
+                        return Wp.debug("Getting current session"), this.userPool ? new Promise((function(t, n) {
                             e.currentUserPoolUser().then((function(r) {
                                 e.userSession(r).then((function(e) {
                                     t(e)
                                 })).catch((function(e) {
-                                    Gp.debug("Failed to get the current session", e), n(e)
+                                    Wp.debug("Failed to get the current session", e), n(e)
                                 }))
                             })).catch((function(e) {
-                                Gp.debug("Failed to get the current user", e), n(e)
+                                Wp.debug("Failed to get the current user", e), n(e)
                             }))
                         })) : Promise.reject(new Error("No User Pool in the configuration."))
                     }, e.prototype._userSession = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t, n, r = this;
-                            return qu(this, (function(o) {
+                            return Ju(this, (function(o) {
                                 switch (o.label) {
                                     case 0:
-                                        if (!e) return Gp.debug("the user is null"), [2, this.rejectAuthError(Wu.NoUserSession)];
+                                        if (!e) return Wp.debug("the user is null"), [2, this.rejectAuthError(Hu.NoUserSession)];
                                         t = this._config.clientMetadata, 0 === this.inflightSessionPromiseCounter && (this.inflightSessionPromise = new Promise((function(n, o) {
                                             e.getSession((function(t, i) {
-                                                return Zu(r, void 0, void 0, (function() {
+                                                return qu(r, void 0, void 0, (function() {
                                                     var r;
-                                                    return qu(this, (function(a) {
+                                                    return Ju(this, (function(a) {
                                                         switch (a.label) {
                                                             case 0:
                                                                 if (!t) return [3, 5];
-                                                                if (Gp.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
+                                                                if (Wp.debug("Failed to get the session from user", e), !this.isSessionInvalid(t)) return [3, 4];
                                                                 a.label = 1;
                                                             case 1:
                                                                 return a.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(e)];
                                                             case 2:
                                                                 return a.sent(), [3, 4];
                                                             case 3:
                                                                 return r = a.sent(), o(new Error("Session is invalid due to: " + t.message + " and failed to clean up invalid session: " + r.message)), [2];
                                                             case 4:
                                                                 return o(t), [2];
                                                             case 5:
-                                                                return Gp.debug("Succeed to get the user session", i), n(i), [2]
+                                                                return Wp.debug("Succeed to get the user session", i), n(i), [2]
                                                         }
                                                     }))
                                                 }))
                                             }), {
                                                 clientMetadata: t
                                             })
                                         }))), this.inflightSessionPromiseCounter++, o.label = 1;
@@ -64767,43 +64770,43 @@
                                         return [2]
                                 }
                             }))
                         }))
                     }, e.prototype.userSession = function(e) {
                         return this._userSession(e)
                     }, e.prototype.currentUserCredentials = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t, n = this;
-                            return qu(this, (function(r) {
+                            return Ju(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
-                                        Gp.debug("Getting current user credentials"), r.label = 1;
+                                        Wp.debug("Getting current user credentials"), r.label = 1;
                                     case 1:
                                         return r.trys.push([1, 3, , 4]), [4, this._storageSync];
                                     case 2:
                                         return r.sent(), [3, 4];
                                     case 3:
-                                        throw e = r.sent(), Gp.debug("Failed to sync cache info into memory", e), e;
+                                        throw e = r.sent(), Wp.debug("Failed to sync cache info into memory", e), e;
                                     case 4:
                                         t = null;
                                         try {
                                             t = JSON.parse(this._storage.getItem("aws-amplify-federatedInfo"))
                                         } catch (o) {
-                                            Gp.debug("failed to get or parse item aws-amplify-federatedInfo", o)
+                                            Wp.debug("failed to get or parse item aws-amplify-federatedInfo", o)
                                         }
                                         return t ? [2, this.Credentials.refreshFederatedToken(t)] : [2, this.currentSession().then((function(e) {
-                                            return Gp.debug("getting session success", e), n.Credentials.set(e, "session")
+                                            return Wp.debug("getting session success", e), n.Credentials.set(e, "session")
                                         })).catch((function() {
-                                            return Gp.debug("getting guest credentials"), n.Credentials.set(null, "guest")
+                                            return Wp.debug("getting guest credentials"), n.Credentials.set(null, "guest")
                                         }))]
                                 }
                             }))
                         }))
                     }, e.prototype.currentCredentials = function() {
-                        return Gp.debug("getting current credentials"), this.Credentials.get()
+                        return Wp.debug("getting current credentials"), this.Credentials.get()
                     }, e.prototype.verifyUserAttribute = function(e, t, n) {
                         return void 0 === n && (n = this._config.clientMetadata), new Promise((function(r, o) {
                             e.getAttributeVerificationCode(t, {
                                 onSuccess: function(e) {
                                     return r(e)
                                 },
                                 onFailure: function(e) {
@@ -64817,289 +64820,289 @@
                                 onSuccess: function(e) {
                                     r(e)
                                 },
                                 onFailure: function(e) {
                                     o(e)
                                 }
                             })
-                        })) : this.rejectAuthError(Wu.EmptyCode)
+                        })) : this.rejectAuthError(Hu.EmptyCode)
                     }, e.prototype.verifyCurrentUserAttribute = function(e) {
                         var t = this;
                         return t.currentUserPoolUser().then((function(n) {
                             return t.verifyUserAttribute(n, e)
                         }))
                     }, e.prototype.verifyCurrentUserAttributeSubmit = function(e, t) {
                         var n = this;
                         return n.currentUserPoolUser().then((function(r) {
                             return n.verifyUserAttributeSubmit(r, e, t)
                         }))
                     }, e.prototype.cognitoIdentitySignOut = function(e, t) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var n, r, o = this;
-                            return qu(this, (function(i) {
+                            return Ju(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
                                         return i.trys.push([0, 2, , 3]), [4, this._storageSync];
                                     case 1:
                                         return i.sent(), [3, 3];
                                     case 2:
-                                        throw n = i.sent(), Gp.debug("Failed to sync cache info into memory", n), n;
+                                        throw n = i.sent(), Wp.debug("Failed to sync cache info into memory", n), n;
                                     case 3:
                                         return r = this._oAuthHandler && "true" === this._storage.getItem("amplify-signin-with-hostedUI"), [2, new Promise((function(n, i) {
                                             if (e && e.global) {
-                                                Gp.debug("user global sign out", t);
+                                                Wp.debug("user global sign out", t);
                                                 var a = o._config.clientMetadata;
                                                 t.getSession((function(e, a) {
-                                                    return Zu(o, void 0, void 0, (function() {
+                                                    return qu(o, void 0, void 0, (function() {
                                                         var o, a = this;
-                                                        return qu(this, (function(s) {
+                                                        return Ju(this, (function(s) {
                                                             switch (s.label) {
                                                                 case 0:
                                                                     if (!e) return [3, 5];
-                                                                    if (Gp.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
+                                                                    if (Wp.debug("failed to get the user session", e), !this.isSessionInvalid(e)) return [3, 4];
                                                                     s.label = 1;
                                                                 case 1:
                                                                     return s.trys.push([1, 3, , 4]), [4, this.cleanUpInvalidSession(t)];
                                                                 case 2:
                                                                     return s.sent(), [3, 4];
                                                                 case 3:
                                                                     return o = s.sent(), i(new Error("Session is invalid due to: " + e.message + " and failed to clean up invalid session: " + o.message)), [2];
                                                                 case 4:
                                                                     return [2, i(e)];
                                                                 case 5:
                                                                     return t.globalSignOut({
                                                                         onSuccess: function(e) {
-                                                                            if (Gp.debug("global sign out success"), !r) return n();
+                                                                            if (Wp.debug("global sign out success"), !r) return n();
                                                                             a.oAuthSignOutRedirect(n, i)
                                                                         },
                                                                         onFailure: function(e) {
-                                                                            return Gp.debug("global sign out failed", e), i(e)
+                                                                            return Wp.debug("global sign out failed", e), i(e)
                                                                         }
                                                                     }), [2]
                                                             }
                                                         }))
                                                     }))
                                                 }), {
                                                     clientMetadata: a
                                                 })
-                                            } else Gp.debug("user sign out", t), t.signOut((function() {
+                                            } else Wp.debug("user sign out", t), t.signOut((function() {
                                                 if (!r) return n();
                                                 o.oAuthSignOutRedirect(n, i)
                                             }))
                                         }))]
                                 }
                             }))
                         }))
                     }, e.prototype.oAuthSignOutRedirect = function(e, t) {
-                        gl().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
+                        yl().isBrowser ? this.oAuthSignOutRedirectOrReject(t) : this.oAuthSignOutAndResolve(e)
                     }, e.prototype.oAuthSignOutAndResolve = function(e) {
                         this._oAuthHandler.signOut(), e()
                     }, e.prototype.oAuthSignOutRedirectOrReject = function(e) {
                         this._oAuthHandler.signOut(), setTimeout((function() {
                             return e(Error("Signout timeout fail"))
                         }), 3e3)
                     }, e.prototype.signOut = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t;
-                            return qu(this, (function(n) {
+                            return Ju(this, (function(n) {
                                 switch (n.label) {
                                     case 0:
                                         return n.trys.push([0, 2, , 3]), [4, this.cleanCachedItems()];
                                     case 1:
                                         return n.sent(), [3, 3];
                                     case 2:
-                                        return n.sent(), Gp.debug("failed to clear cached items"), [3, 3];
+                                        return n.sent(), Wp.debug("failed to clear cached items"), [3, 3];
                                     case 3:
                                         return this.userPool ? (t = this.userPool.getCurrentUser()) ? [4, this.cognitoIdentitySignOut(e, t)] : [3, 5] : [3, 7];
                                     case 4:
                                         return n.sent(), [3, 6];
                                     case 5:
-                                        Gp.debug("no current Cognito user"), n.label = 6;
+                                        Wp.debug("no current Cognito user"), n.label = 6;
                                     case 6:
                                         return [3, 8];
                                     case 7:
-                                        Gp.debug("no Cognito User pool"), n.label = 8;
+                                        Wp.debug("no Cognito User pool"), n.label = 8;
                                     case 8:
-                                        return Vp("signOut", this.user, "A user has been signed out"), this.user = null, [2]
+                                        return Zp("signOut", this.user, "A user has been signed out"), this.user = null, [2]
                                 }
                             }))
                         }))
                     }, e.prototype.cleanCachedItems = function() {
-                        return Zu(this, void 0, void 0, (function() {
-                            return qu(this, (function(e) {
+                        return qu(this, void 0, void 0, (function() {
+                            return Ju(this, (function(e) {
                                 switch (e.label) {
                                     case 0:
                                         return [4, this.Credentials.clear()];
                                     case 1:
                                         return e.sent(), [2]
                                 }
                             }))
                         }))
                     }, e.prototype.changePassword = function(e, t, n, r) {
                         var o = this;
                         return void 0 === r && (r = this._config.clientMetadata), new Promise((function(i, a) {
                             o.userSession(e).then((function(o) {
                                 e.changePassword(t, n, (function(e, t) {
-                                    return e ? (Gp.debug("change password failure", e), a(e)) : i(t)
+                                    return e ? (Wp.debug("change password failure", e), a(e)) : i(t)
                                 }), r)
                             }))
                         }))
                     }, e.prototype.forgotPassword = function(e, t) {
                         if (void 0 === t && (t = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                        if (!e) return this.rejectAuthError(Wu.EmptyUsername);
+                        if (!e) return this.rejectAuthError(Hu.EmptyUsername);
                         var n = this.createCognitoUser(e);
                         return new Promise((function(r, o) {
                             n.forgotPassword({
                                 onSuccess: function() {
                                     r()
                                 },
                                 onFailure: function(t) {
-                                    Gp.debug("forgot password failure", t), Vp("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
+                                    Wp.debug("forgot password failure", t), Zp("forgotPassword_failure", t, e + " forgotPassword failed"), o(t)
                                 },
                                 inputVerificationCode: function(t) {
-                                    Vp("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
+                                    Zp("forgotPassword", n, e + " has initiated forgot password flow"), r(t)
                                 }
                             }, t)
                         }))
                     }, e.prototype.forgotPasswordSubmit = function(e, t, n, r) {
                         if (void 0 === r && (r = this._config.clientMetadata), !this.userPool) return this.rejectNoUserPool();
-                        if (!e) return this.rejectAuthError(Wu.EmptyUsername);
-                        if (!t) return this.rejectAuthError(Wu.EmptyCode);
-                        if (!n) return this.rejectAuthError(Wu.EmptyPassword);
+                        if (!e) return this.rejectAuthError(Hu.EmptyUsername);
+                        if (!t) return this.rejectAuthError(Hu.EmptyCode);
+                        if (!n) return this.rejectAuthError(Hu.EmptyPassword);
                         var o = this.createCognitoUser(e);
                         return new Promise((function(i, a) {
                             o.confirmPassword(t, n, {
                                 onSuccess: function(t) {
-                                    Vp("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
+                                    Zp("forgotPasswordSubmit", o, e + " forgotPasswordSubmit successful"), i(t)
                                 },
                                 onFailure: function(t) {
-                                    Vp("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
+                                    Zp("forgotPasswordSubmit_failure", t, e + " forgotPasswordSubmit failed"), a(t)
                                 }
                             }, r)
                         }))
                     }, e.prototype.currentUserInfo = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t, n, r, o, i, a;
-                            return qu(this, (function(s) {
+                            return Ju(this, (function(s) {
                                 switch (s.label) {
                                     case 0:
                                         return (e = this.Credentials.getCredSource()) && "aws" !== e && "userPool" !== e ? [3, 9] : [4, this.currentUserPoolUser().catch((function(e) {
-                                            return Gp.error(e)
+                                            return Wp.error(e)
                                         }))];
                                     case 1:
                                         if (!(a = s.sent())) return [2, null];
                                         s.label = 2;
                                     case 2:
                                         return s.trys.push([2, 8, , 9]), [4, this.userAttributes(a)];
                                     case 3:
                                         t = s.sent(), n = this.attributesToObject(t), r = null, s.label = 4;
                                     case 4:
                                         return s.trys.push([4, 6, , 7]), [4, this.currentCredentials()];
                                     case 5:
                                         return r = s.sent(), [3, 7];
                                     case 6:
-                                        return o = s.sent(), Gp.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
+                                        return o = s.sent(), Wp.debug("Failed to retrieve credentials while getting current user info", o), [3, 7];
                                     case 7:
                                         return [2, {
                                             id: r ? r.identityId : void 0,
                                             username: a.getUsername(),
                                             attributes: n
                                         }];
                                     case 8:
-                                        return i = s.sent(), Gp.error("currentUserInfo error", i), [2, {}];
+                                        return i = s.sent(), Wp.error("currentUserInfo error", i), [2, {}];
                                     case 9:
                                         return "federated" === e ? [2, (a = this.user) || {}] : [2]
                                 }
                             }))
                         }))
                     }, e.prototype.federatedSignIn = function(e, t, n) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var r, o, i, a, s, u, l, c, d, p, f;
-                            return qu(this, (function(h) {
+                            return Ju(this, (function(h) {
                                 switch (h.label) {
                                     case 0:
                                         if (!this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation requires either a User Pool or Identity Pool in config");
                                         if ("undefined" === typeof e && this._config.identityPoolId && !this._config.userPoolId) throw new Error("Federation with Identity Pools requires tokens passed as arguments");
-                                        return Ku(e) || (g = e) && ["customProvider"].find((function(e) {
+                                        return Xu(e) || (g = e) && ["customProvider"].find((function(e) {
                                             return g.hasOwnProperty(e)
                                         })) || function(e) {
                                             return e && !!["customState"].find((function(t) {
                                                 return e.hasOwnProperty(t)
                                             }))
                                         }(e) || "undefined" === typeof e ? (r = e || {
-                                            provider: Gu.Cognito
-                                        }, s = Ku(r) ? r.provider : r.customProvider, Ku(r), o = r.customState, this._config.userPoolId && (i = Xu(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = Xu(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
+                                            provider: Wu.Cognito
+                                        }, s = Xu(r) ? r.provider : r.customProvider, Xu(r), o = r.customState, this._config.userPoolId && (i = $u(this._config.oauth) ? this._config.userPoolWebClientId : this._config.oauth.clientID, a = $u(this._config.oauth) ? this._config.oauth.redirectSignIn : this._config.oauth.redirectUri, this._oAuthHandler.oauthSignIn(this._config.oauth.responseType, this._config.oauth.domain, a, i, s, o)), [3, 4]) : [3, 1];
                                     case 1:
                                         s = e;
                                         try {
-                                            (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Gp.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
+                                            (u = JSON.stringify(JSON.parse(this._storage.getItem("aws-amplify-federatedInfo")).user)) && Wp.warn("There is already a signed in user: " + u + " in your app.\n\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\t\tYou should not call Auth.federatedSignIn method again as it may cause unexpected behavior.")
                                         } catch (y) {}
                                         return l = t.token, c = t.identity_id, d = t.expires_at, [4, this.Credentials.set({
                                             provider: s,
                                             token: l,
                                             identity_id: c,
                                             user: n,
                                             expires_at: d
                                         }, "federation")];
                                     case 2:
                                         return p = h.sent(), [4, this.currentAuthenticatedUser()];
                                     case 3:
-                                        return f = h.sent(), Vp("signIn", f, "A user " + f.username + " has been signed in"), Gp.debug("federated sign in credentials", p), [2, p];
+                                        return f = h.sent(), Zp("signIn", f, "A user " + f.username + " has been signed in"), Wp.debug("federated sign in credentials", p), [2, p];
                                     case 4:
                                         return [2]
                                 }
                                 var g
                             }))
                         }))
                     }, e.prototype._handleAuthResponse = function(e) {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var t, n, r, o, i, a, s, u, l, c, d, p, f, h;
-                            return qu(this, (function(g) {
+                            return Ju(this, (function(g) {
                                 switch (g.label) {
                                     case 0:
-                                        if (this.oAuthFlowInProgress) return Gp.debug("Skipping URL " + e + " current flow in progress"), [2];
+                                        if (this.oAuthFlowInProgress) return Wp.debug("Skipping URL " + e + " current flow in progress"), [2];
                                         g.label = 1;
                                     case 1:
                                         if (g.trys.push([1, , 8, 9]), this.oAuthFlowInProgress = !0, !this._config.userPoolId) throw new Error("OAuth responses require a User Pool defined in config");
-                                        if (Vp("parsingCallbackUrl", {
+                                        if (Zp("parsingCallbackUrl", {
                                                 url: e
-                                            }, "The callback url is being parsed"), t = e || (gl().isBrowser ? window.location.href : ""), n = !!((0, Ap.Qc)(t).query || "").split("&").map((function(e) {
+                                            }, "The callback url is being parsed"), t = e || (yl().isBrowser ? window.location.href : ""), n = !!((0, zp.Qc)(t).query || "").split("&").map((function(e) {
                                                 return e.split("=")
                                             })).find((function(e) {
-                                                var t = Ju(e, 1)[0];
+                                                var t = Ku(e, 1)[0];
                                                 return "code" === t || "error" === t
-                                            })), r = !!((0, Ap.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
+                                            })), r = !!((0, zp.Qc)(t).hash || "#").substr(1).split("&").map((function(e) {
                                                 return e.split("=")
                                             })).find((function(e) {
-                                                var t = Ju(e, 1)[0];
+                                                var t = Ku(e, 1)[0];
                                                 return "access_token" === t || "error" === t
                                             })), !n && !r) return [3, 7];
                                         this._storage.setItem("amplify-redirected-from-hosted-ui", "true"), g.label = 2;
                                     case 2:
                                         return g.trys.push([2, 6, , 7]), [4, this._oAuthHandler.handleAuthResponse(t)];
                                     case 3:
-                                        return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new ip({
-                                            IdToken: new np({
+                                        return o = g.sent(), i = o.accessToken, a = o.idToken, s = o.refreshToken, u = o.state, l = new ap({
+                                            IdToken: new rp({
                                                 IdToken: a
                                             }),
-                                            RefreshToken: new rp({
+                                            RefreshToken: new op({
                                                 RefreshToken: s
                                             }),
-                                            AccessToken: new ep({
+                                            AccessToken: new tp({
                                                 AccessToken: i
                                             })
                                         }), c = void 0, this._config.identityPoolId ? [4, this.Credentials.set(l, "session")] : [3, 5];
                                     case 4:
-                                        c = g.sent(), Gp.debug("AWS credentials", c), g.label = 5;
+                                        c = g.sent(), Wp.debug("AWS credentials", c), g.label = 5;
                                     case 5:
-                                        return d = /-/.test(u), (p = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Vp("signIn", p, "A user " + p.getUsername() + " has been signed in"), Vp("cognitoHostedUI", p, "A user " + p.getUsername() + " has been signed in via Cognito Hosted UI"), d && (f = u.split("-").splice(1).join("-"), Vp("customOAuthState", f.match(/.{2}/g).map((function(e) {
+                                        return d = /-/.test(u), (p = this.createCognitoUser(l.getIdToken().decodePayload()["cognito:username"])).setSignInUserSession(l), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Zp("signIn", p, "A user " + p.getUsername() + " has been signed in"), Zp("cognitoHostedUI", p, "A user " + p.getUsername() + " has been signed in via Cognito Hosted UI"), d && (f = u.split("-").splice(1).join("-"), Zp("customOAuthState", f.match(/.{2}/g).map((function(e) {
                                             return String.fromCharCode(parseInt(e, 16))
                                         })).join(""), "State for user " + p.getUsername())), [2, c];
                                     case 6:
-                                        return h = g.sent(), Gp.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Vp("signIn_failure", h, "The OAuth response flow failed"), Vp("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), Vp("customState_failure", h, "A failure occurred when returning state"), [3, 7];
+                                        return h = g.sent(), Wp.debug("Error in cognito hosted auth response", h), window && "undefined" !== typeof window.history && window.history.replaceState({}, null, this._config.oauth.redirectSignIn), Zp("signIn_failure", h, "The OAuth response flow failed"), Zp("cognitoHostedUI_failure", h, "A failure occurred when returning to the Cognito Hosted UI"), Zp("customState_failure", h, "A failure occurred when returning state"), [3, 7];
                                     case 7:
                                         return [3, 9];
                                     case 8:
                                         return this.oAuthFlowInProgress = !1, [7];
                                     case 9:
                                         return [2]
                                 }
@@ -65124,86 +65127,86 @@
                     }, e.prototype.createCognitoUser = function(e) {
                         var t = {
                             Username: e,
                             Pool: this.userPool
                         };
                         t.Storage = this._storage;
                         var n = this._config.authenticationFlowType,
-                            r = new hp(t);
+                            r = new gp(t);
                         return n && r.setAuthenticationFlowType(n), r
                     }, e.prototype._isValidAuthStorage = function(e) {
                         return !!e && "function" === typeof e.getItem && "function" === typeof e.setItem && "function" === typeof e.removeItem && "function" === typeof e.clear
                     }, e.prototype.noUserPoolErrorHandler = function(e) {
-                        return !e || e.userPoolId && e.identityPoolId ? Wu.NoConfig : Wu.MissingAuthConfig
+                        return !e || e.userPoolId && e.identityPoolId ? Hu.NoConfig : Hu.MissingAuthConfig
                     }, e.prototype.rejectAuthError = function(e) {
-                        return Promise.reject(new Bp(e))
+                        return Promise.reject(new Yp(e))
                     }, e.prototype.rejectNoUserPool = function() {
                         var e = this.noUserPoolErrorHandler(this._config);
-                        return Promise.reject(new Yp(e))
+                        return Promise.reject(new Qp(e))
                     }, e.prototype.rememberDevice = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t;
-                            return qu(this, (function(n) {
+                            return Ju(this, (function(n) {
                                 switch (n.label) {
                                     case 0:
                                         return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                     case 1:
                                         return e = n.sent(), [3, 3];
                                     case 2:
-                                        return t = n.sent(), Gp.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                        return t = n.sent(), Wp.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                     case 3:
                                         return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                             e.setDeviceStatusRemembered({
                                                 onSuccess: function(e) {
                                                     t(e)
                                                 },
                                                 onFailure: function(e) {
-                                                    "InvalidParameterException" === e.code ? n(new Bp(Wu.DeviceConfig)) : "NetworkError" === e.code ? n(new Bp(Wu.NetworkError)) : n(e)
+                                                    "InvalidParameterException" === e.code ? n(new Yp(Hu.DeviceConfig)) : "NetworkError" === e.code ? n(new Yp(Hu.NetworkError)) : n(e)
                                                 }
                                             })
                                         }))]
                                 }
                             }))
                         }))
                     }, e.prototype.forgetDevice = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t;
-                            return qu(this, (function(n) {
+                            return Ju(this, (function(n) {
                                 switch (n.label) {
                                     case 0:
                                         return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                     case 1:
                                         return e = n.sent(), [3, 3];
                                     case 2:
-                                        return t = n.sent(), Gp.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
+                                        return t = n.sent(), Wp.debug("The user is not authenticated by the error", t), [2, Promise.reject("The user is not authenticated")];
                                     case 3:
                                         return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                             e.forgetDevice({
                                                 onSuccess: function(e) {
                                                     t(e)
                                                 },
                                                 onFailure: function(e) {
-                                                    "InvalidParameterException" === e.code ? n(new Bp(Wu.DeviceConfig)) : "NetworkError" === e.code ? n(new Bp(Wu.NetworkError)) : n(e)
+                                                    "InvalidParameterException" === e.code ? n(new Yp(Hu.DeviceConfig)) : "NetworkError" === e.code ? n(new Yp(Hu.NetworkError)) : n(e)
                                                 }
                                             })
                                         }))]
                                 }
                             }))
                         }))
                     }, e.prototype.fetchDevices = function() {
-                        return Zu(this, void 0, void 0, (function() {
+                        return qu(this, void 0, void 0, (function() {
                             var e, t;
-                            return qu(this, (function(n) {
+                            return Ju(this, (function(n) {
                                 switch (n.label) {
                                     case 0:
                                         return n.trys.push([0, 2, , 3]), [4, this.currentUserPoolUser()];
                                     case 1:
                                         return e = n.sent(), [3, 3];
                                     case 2:
-                                        throw t = n.sent(), Gp.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
+                                        throw t = n.sent(), Wp.debug("The user is not authenticated by the error", t), new Error("The user is not authenticated");
                                     case 3:
                                         return e.getCachedDeviceKeyAndPassword(), [2, new Promise((function(t, n) {
                                             var r = {
                                                 onSuccess: function(e) {
                                                     var n = e.Devices.map((function(e) {
                                                         var t = e.DeviceAttributes.find((function(e) {
                                                             return "device_name" === e.Name
@@ -65212,28 +65215,28 @@
                                                             id: e.DeviceKey,
                                                             name: t.Value
                                                         }
                                                     }));
                                                     t(n)
                                                 },
                                                 onFailure: function(e) {
-                                                    "InvalidParameterException" === e.code ? n(new Bp(Wu.DeviceConfig)) : "NetworkError" === e.code ? n(new Bp(Wu.NetworkError)) : n(e)
+                                                    "InvalidParameterException" === e.code ? n(new Yp(Hu.DeviceConfig)) : "NetworkError" === e.code ? n(new Yp(Hu.NetworkError)) : n(e)
                                                 }
                                             };
                                             e.listDevices(60, null, r)
                                         }))]
                                 }
                             }))
                         }))
                     }, e
                 }(),
-                qp = new Zp(null);
-            $l.register(qp);
-            var Jp = "#FEFEFE",
-                Kp = function(e) {
+                Jp = new qp(null);
+            ec.register(Jp);
+            var Kp = "#FEFEFE",
+                Xp = function(e) {
                     var t = e.hide,
                         n = je().environ,
                         r = Fa(),
                         o = Ua(rn.Url("/cognito_config", !1), {
                             cache: !0,
                             onData: function(e) {
                                 var t = {
@@ -65245,15 +65248,15 @@
                                         domain: e.domain,
                                         scope: e.scope,
                                         prompt: "select_account",
                                         redirectSignIn: e.callback,
                                         responseType: "code"
                                     }
                                 };
-                                qp.configure(t)
+                                Jp.configure(t)
                             }
                         });
                     var i = (0, wo.jsx)("div", {
                         children: (0, wo.jsxs)("div", {
                             className: "title-font",
                             style: {
                                 marginTop: "4pt",
@@ -65281,52 +65284,52 @@
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             transform: "scale(1.1)",
                             marginTop: "10pt",
                             marginBottom: "40pt"
                         },
-                        children: (0, wo.jsx)(Xp, {
+                        children: (0, wo.jsx)($p, {
                             links: i,
                             children: o.loading ? (0, wo.jsx)(wo.Fragment, {
                                 children: (0, wo.jsx)(Lo, {
                                     condition: !0,
                                     color: ln.GetForegroundColor(),
                                     bold: !1,
                                     size: "140px",
                                     label: "Loading configuration "
                                 })
                             }) : (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsx)("div", {
                                     style: {
                                         paddingTop: "0pt"
                                     }
-                                }), (0, wo.jsx)($p, {
+                                }), (0, wo.jsx)(ef, {
                                     signin: function() {
-                                        Bt.Set("env", tn.PreferredName(n, r)), Bt.Set("signinvia", "Google"), qp.federatedSignIn({
+                                        Bt.Set("env", tn.PreferredName(n, r)), Bt.Set("signinvia", "Google"), Jp.federatedSignIn({
                                             provider: "Google",
                                             prompt: "select_account"
                                         }, {
                                             prompt: "select_account"
                                         })
                                     }
                                 }), (0, wo.jsx)("div", {
                                     style: {
                                         paddingTop: "6pt"
                                     }
-                                }), (0, wo.jsx)(ef, {
+                                }), (0, wo.jsx)(tf, {
                                     signin: function() {
                                         window.alert("Sign in with GitHub via Cognito not supported.")
                                     }
                                 })]
                             })
                         })
                     })
                 },
-                Xp = function(e) {
+                $p = function(e) {
                     var t = e.links,
                         n = e.children;
                     return (0, wo.jsx)("div", {
                         className: "container",
                         style: {
                             width: "265pt",
                             marginTop: "30pt"
@@ -65337,15 +65340,15 @@
                                     border: "2px solid var(--box-fg)",
                                     padding: "2px 2px 2px 2px",
                                     borderRadius: "6px",
                                     overflow: "hidden"
                                 },
                                 children: (0, wo.jsxs)("div", {
                                     style: {
-                                        background: Jp,
+                                        background: Kp,
                                         border: "1px solid var(--box-fg)",
                                         borderRadius: "6px",
                                         overflow: "hidden"
                                     },
                                     children: [(0, wo.jsx)("div", {
                                         style: {
                                             background: "var(--box-fg)",
@@ -65370,17 +65373,17 @@
                                 })
                             }), t && (0, wo.jsx)(wo.Fragment, {
                                 children: t
                             })]
                         })
                     })
                 },
-                $p = function(e) {
+                ef = function(e) {
                     var t = e.signin;
-                    return (0, wo.jsxs)(tf, {
+                    return (0, wo.jsxs)(nf, {
                         signin: t,
                         children: [(0, wo.jsx)("img", {
                             alt: "google",
                             src: on.GoogleLoginLogo(),
                             style: {
                                 position: "relative",
                                 marginTop: "-2px"
@@ -65392,17 +65395,17 @@
                                 fontSize: "12pt",
                                 marginLeft: "10pt"
                             },
                             children: "Sign in with Google"
                         })]
                     })
                 },
-                ef = function(e) {
+                tf = function(e) {
                     var t = e.signin;
-                    return (0, wo.jsxs)(tf, {
+                    return (0, wo.jsxs)(nf, {
                         signin: t,
                         children: [(0, wo.jsx)("img", {
                             alt: "github",
                             src: on.GitHubLoginLogo(),
                             style: {
                                 position: "relative",
                                 marginTop: "-2px",
@@ -65415,30 +65418,30 @@
                                 fontSize: "12pt",
                                 marginLeft: "7pt"
                             },
                             children: "Sign in with GitHub"
                         })]
                     })
                 },
-                tf = function(e) {
+                nf = function(e) {
                     var t = e.signin,
                         n = e.children;
                     return (0, wo.jsx)("div", {
                         style: {
-                            background: Jp,
+                            background: Kp,
                             padding: "0 10pt 0 10pt"
                         },
                         children: (0, wo.jsx)("button", {
                             className: "signin-as-button",
                             onClick: t,
                             children: n
                         })
                     })
                 },
-                nf = function(e) {
+                rf = function(e) {
                     var t = l($e(), 1)[0],
                         n = t.get("code"),
                         r = t.get("state"),
                         o = sessionStorage.getItem("oauth_state"),
                         i = sessionStorage.getItem("ouath_pkce_key"),
                         a = Me(),
                         s = "".concat(rn.Url("/cognito/callback", !1), "?code=").concat(n, "&code_verifier=").concat(i, "&state=").concat(r, "&state_verifier=").concat(o),
@@ -65461,28 +65464,28 @@
                         var c = Bt.Get("signinvia");
                         return (0, wo.jsx)("div", {
                             style: {
                                 transform: "scale(1.1)",
                                 marginTop: "10pt",
                                 marginBottom: "40pt"
                             },
-                            children: (0, wo.jsx)(Xp, {
+                            children: (0, wo.jsx)($p, {
                                 children: (0, wo.jsx)(Lo, {
                                     condition: u.loading,
                                     color: ln.GetForegroundColor(),
                                     bold: !1,
                                     size: 140,
                                     label: "Signing in via ".concat(c)
                                 })
                             })
                         })
                     }
                 },
-                rf = n(9712),
-                of = function(e) {
+                of = n(9712),
+                af = function(e) {
                     var n, r, o, i, a, s, u, c, d, p, f, h = Fa(),
                         g = l((0, t.useState)(!1), 2),
                         y = g[0],
                         m = g[1],
                         v = l((0, t.useState)(!1), 2),
                         M = v[0],
                         j = v[1],
@@ -65528,15 +65531,15 @@
                                     theme: {
                                         primaryColor: "blue",
                                         backgroundColor: "blue",
                                         logo: ""
                                     },
                                     allowedConnections: null === w || void 0 === w || null === (o = w.data) || void 0 === o ? void 0 : o.connections
                                 };
-                                return new rf.default(null === w || void 0 === w || null === (i = w.data) || void 0 === i ? void 0 : i.client, null === w || void 0 === w || null === (a = w.data) || void 0 === a ? void 0 : a.domain, s)
+                                return new of.default(null === w || void 0 === w || null === (i = w.data) || void 0 === i ? void 0 : i.client, null === w || void 0 === w || null === (a = w.data) || void 0 === a ? void 0 : a.domain, s)
                             }().show(), navigator.userAgent.toLowerCase().indexOf("firefox") > -1 && (document.getElementById("login_auth_container").style.height = "200", document.getElementById("login_auth_container").style.background = "white", document.getElementById("login_auth_container").style.borderStyle = "none"), document.getElementById("login_auth_container").firstChild.firstChild.style.paddingLeft = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingRight = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingTop = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.paddingBottom = "1", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", document.getElementById("login_auth_container").firstChild.firstChild.style.fontWeight = "bold", m(!0)
                     }
                     if ((h.loading || w.loading) && !h.error) return (0, wo.jsx)(wo.Fragment, {
                         children: "Loading ..."
                     });
                     if (h.error) return (0, wo.jsx)(ua, {
                         error: h.error,
@@ -65580,15 +65583,15 @@
                                         position: "bottom",
                                         text: "AWS Account Alias: ".concat(null === h || void 0 === h || null === (c = h.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name)
                                     })]
                                 }), (0, wo.jsx)("br", {})]
                             })]
                         })
                     };
-                    return N ? (0, wo.jsx)(Kp, {
+                    return N ? (0, wo.jsx)(Xp, {
                         hide: function() {
                             return I(!1)
                         }
                     }) : (0, wo.jsx)(wo.Fragment, {
                         children: co.IsLoggedIn(h) ? (0, wo.jsx)(t.Fragment, {
                             children: (0, wo.jsxs)("div", {
                                 className: "container",
@@ -65655,21 +65658,21 @@
                                                     }), (0, wo.jsxs)("div", {
                                                         style: {
                                                             fontSize: "small",
                                                             marginTop: "6pt",
                                                             paddingTop: "5pt",
                                                             borderTop: "1px solid"
                                                         },
-                                                        children: ["Session started: ", (0, wo.jsx)(Cs.Live, {
+                                                        children: ["Session started: ", (0, wo.jsx)(Es.Live, {
                                                             start: co.Token().authenticated_at,
                                                             verbose: !0,
                                                             fallback: "just now",
                                                             suffix: "ago",
                                                             tooltip: !0
-                                                        }), "\xa0", (0, wo.jsx)("br", {}), "Session expires: ", (0, wo.jsx)(Cs.Live, {
+                                                        }), "\xa0", (0, wo.jsx)("br", {}), "Session expires: ", (0, wo.jsx)(Es.Live, {
                                                             end: co.Token().authenticated_until,
                                                             verbose: !0,
                                                             fallback: "now",
                                                             suffix: "from now",
                                                             tooltip: !0
                                                         }), "\xa0", (0, wo.jsx)("br", {}), "Click ", (0, wo.jsx)("span", {
                                                             style: {
@@ -65936,15 +65939,15 @@
                                             fontSize: "large"
                                         },
                                         children: [po.Warning, "\xa0\xa0Not Logged In"]
                                     }), Bt.HasAuthToken() && co.SessionExpired() && (0, wo.jsx)("small", {
                                         children: (0, wo.jsx)(oa, {
                                             id: "tooltip-nologin",
                                             position: "bottom",
-                                            text: "".concat(Cs.Format(co.Token().authenticated_until, new Date, !0, "", "Login expired:", "ago"))
+                                            text: "".concat(Es.Format(co.Token().authenticated_until, new Date, !0, "", "Login expired:", "ago"))
                                         })
                                     }), (0, wo.jsx)(aa, {
                                         top: "6pt",
                                         bottom: "6pt"
                                     }), "Click ", (0, wo.jsx)("u", {
                                         style: {
                                             cursor: "pointer"
@@ -66207,15 +66210,15 @@
                                         b && !y && T()
                                     }), 10), "")]
                                 })]
                             })]
                         })
                     })
                 },
-                af = function(e) {
+                sf = function(e) {
                     var n = Fa(),
                         r = je().environCompare,
                         o = l((0, t.useState)(!1), 2),
                         i = o[0],
                         a = o[1],
                         s = l((0, t.useState)("all"), 2),
                         u = s[0],
@@ -66561,15 +66564,15 @@
                                     display: "none"
                                 },
                                 children: d.yaml()
                             })]
                         })
                     })
                 },
-                sf = function(e) {
+                uf = function(e) {
                     var t = {
                             fontFamily: "monospace",
                             background: e.toggled ? "var(--box-fg)" : "inherit",
                             color: e.toggled ? "var(--box-bg)" : "inherit",
                             fontSize: "10pt",
                             fontWeight: "bold",
                             border: "1pt black solid",
@@ -66627,27 +66630,27 @@
                             id: "tooltip-toggle-".concat(n),
                             position: "bottom",
                             size: "small",
                             text: "Click to ".concat(e.toggled ? "hide" : "show", " raw ").concat(e.yaml ? "YAML" : "JSON", " data.")
                         })]
                     })
                 },
-                uf = function(e) {
+                lf = function(e) {
                     var n, r = l((0, t.useState)(!1), 2),
                         o = r[0],
                         i = r[1],
                         a = function() {
                             return i(!o)
                         },
                         s = (0, t.useRef)(null);
                     return e.disabled ? (0, wo.jsx)(wo.Fragment, {
                         children: e.children
                     }) : (0, wo.jsxs)("div", {
                         children: [(e.both || !o) && (0, wo.jsxs)(wo.Fragment, {
-                            children: [(0, wo.jsx)(sf, {
+                            children: [(0, wo.jsx)(uf, {
                                 toggle: a,
                                 toggled: o,
                                 data: e.data,
                                 yaml: e.yaml
                             }), (0, wo.jsx)("div", {
                                 ref: s,
                                 children: e.children
@@ -66662,15 +66665,15 @@
                             }) : (0, wo.jsxs)(wo.Fragment, {
                                 children: [(0, wo.jsxs)("small", {
                                     children: [(0, wo.jsx)("b", {
                                         style: {
                                             float: "left"
                                         },
                                         children: e.title || "Raw ".concat(e.yaml ? "YAML" : "JSON", " Data")
-                                    }), (0, wo.jsx)(sf, {
+                                    }), (0, wo.jsx)(uf, {
                                         toggle: a,
                                         toggled: o,
                                         data: e.data,
                                         yaml: e.yaml
                                     })]
                                 }), (0, wo.jsx)("br", {}), (0, wo.jsx)(aa, {
                                     top: "4pt",
@@ -66690,31 +66693,31 @@
                                 }) : (0, wo.jsx)(wo.Fragment, {
                                     children: no.Format(e.data)
                                 })
                             })]
                         }) : (0, wo.jsx)(wo.Fragment, {})]
                     })
                 },
-                lf = {
+                cf = {
                     color: "var(--box-fg)",
                     fontWeight: "bold",
                     paddingTop: "1pt",
                     verticalAlign: "top",
                     width: "5%",
                     paddingRight: "8pt",
                     whiteSpace: "nowrap"
                 },
-                cf = {
+                df = {
                     verticalAlign: "top"
                 };
 
-            function df(e) {
+            function pf(e) {
                 return /^\*+$/.test(e)
             }
-            var pf = function(e) {
+            var ff = function(e) {
                     var t = e.showVpcs,
                         n = e.toggleVpcs,
                         r = e.showSecurityGroups,
                         o = e.toggleSecurityGroups,
                         i = e.showSubnetsPublic,
                         a = e.toggleSubnetsPublic,
                         s = e.showSubnetsPrivate,
@@ -66767,15 +66770,15 @@
                                 },
                                 onClick: o,
                                 children: "Security Groups"
                             })]
                         })]
                     })
                 },
-                ff = function(e) {
+                hf = function(e) {
                     var t = e.showEcsClusters,
                         n = e.toggleEcsClusters;
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
                                 children: "AWS Elastic Container Service"
                             })
@@ -66792,15 +66795,15 @@
                                 },
                                 onClick: n,
                                 children: "Clusters"
                             })
                         })]
                     })
                 },
-                hf = function(e) {
+                gf = function(e) {
                     var t = e.showGac,
                         n = e.toggleGac,
                         r = e.showEcosystem,
                         o = e.toggleEcosystem;
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
@@ -66829,15 +66832,15 @@
                                 },
                                 onClick: n,
                                 children: "Global Application Configuration"
                             })]
                         })]
                     })
                 },
-                gf = function(e) {
+                yf = function(e) {
                     var t, n, r = e.keyedState,
                         o = e.hide,
                         i = "true" === (null === (t = $e()[0]) || void 0 === t || null === (n = t.get("all")) || void 0 === n ? void 0 : n.toLowerCase()),
                         a = Ua("/aws/vpcs".concat(i ? "/all" : ""), {
                             cache: !0
                         });
                     return (0, wo.jsxs)("div", {
@@ -66878,24 +66881,24 @@
                                     marginTop: "2pt"
                                 },
                                 children: (0, wo.jsx)(Lo, {
                                     label: "Loading VPCs"
                                 })
                             }), a.map((function(e) {
                                 return (0, wo.jsx)("div", {
-                                    children: (0, wo.jsx)(yf, {
+                                    children: (0, wo.jsx)(mf, {
                                         vpc: e,
                                         keyedState: null === r || void 0 === r ? void 0 : r.keyed(e.id)
                                     })
                                 }, e.id)
                             }))]
                         })]
                     })
                 },
-                yf = function(e) {
+                mf = function(e) {
                     var t = e.vpc,
                         n = e.keyedState,
                         r = l(Va(n), 2),
                         o = r[0],
                         i = r[1],
                         a = function(e) {
                             return o[e]
@@ -66943,55 +66946,55 @@
                                     bottom: "2pt"
                                 })]
                             }), (0, wo.jsx)("table", {
                                 width: "100%",
                                 children: (0, wo.jsxs)("tbody", {
                                     children: [(0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "ID:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: t.id
                                         })]
                                     }), (null === t || void 0 === t ? void 0 : t.stack) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Stack:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.stack
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "CIDR:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.cidr
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Status:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.status
                                         })]
                                     }), (0, wo.jsx)(aa, {
                                         top: "2pt",
                                         bottom: "2pt",
                                         table: 2
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return t.id, s("showSubnetsPublic")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Public Subnets:"
                                         }), (0, wo.jsx)("td", {
                                             children: u() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67007,29 +67010,29 @@
                                     }), u() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(mf, {
+                                                children: (0, wo.jsx)(vf, {
                                                     type: "public",
                                                     vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                     notitle: !0,
                                                     keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-public")
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return s("showSubnetsPrivate")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Private Subnets:"
                                         }), (0, wo.jsx)("td", {
                                             children: c() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67045,29 +67048,29 @@
                                     }), c() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(mf, {
+                                                children: (0, wo.jsx)(vf, {
                                                     type: "private",
                                                     vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                     notitle: !0,
                                                     keyedState: null === n || void 0 === n ? void 0 : n.keyed("subnets-private")
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return s("showSecurityGroups")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Security Groups:"
                                         }), (0, wo.jsx)("td", {
                                             children: d() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67083,28 +67086,28 @@
                                     }), d() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(Mf, {
+                                                children: (0, wo.jsx)(jf, {
                                                     vpcId: null === t || void 0 === t ? void 0 : t.id,
                                                     notitle: !0,
                                                     keyedState: null === n || void 0 === n ? void 0 : n.keyed("security-groups")
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return s("showTags")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Tags:"
                                         }), (0, wo.jsx)("td", {
                                             children: p() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67120,26 +67123,26 @@
                                     }), p() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(xf, {
+                                                children: (0, wo.jsx)(Nf, {
                                                     tags: null === t || void 0 === t ? void 0 : t.tags
                                                 })
                                             })
                                         })
                                     })]
                                 })
                             })]
                         })
                     })
                 },
-                mf = function(e) {
+                vf = function(e) {
                     var t, n, r = e.vpcId,
                         o = e.type,
                         i = e.hide,
                         a = e.notitle,
                         s = e.keyedState,
                         u = "true" === (null === (t = $e()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                         l = r ? "?vpc=".concat(r) : "",
@@ -67178,28 +67181,28 @@
                                 children: (0, wo.jsx)(Lo, {
                                     label: "Loading subnets"
                                 })
                             }), null === (n = c.filter((function(e) {
                                 return !o || e.type === o
                             }))) || void 0 === n ? void 0 : n.map((function(e) {
                                 return (0, wo.jsxs)("div", {
-                                    children: [(0, wo.jsx)(vf, {
+                                    children: [(0, wo.jsx)(Mf, {
                                         subnet: e,
                                         keyedState: null === s || void 0 === s ? void 0 : s.keyed(e.id)
                                     }), (0, wo.jsx)("div", {
                                         style: {
                                             height: "4pt"
                                         }
                                     })]
                                 }, e.id)
                             }))]
                         })]
                     })
                 },
-                vf = function(e) {
+                Mf = function(e) {
                     var t = e.subnet,
                         n = e.keyedState,
                         r = l(Va(n), 2),
                         o = r[0],
                         i = r[1],
                         a = function() {
                             return o["showTags"]
@@ -67248,74 +67251,74 @@
                                     bottom: "2pt"
                                 })]
                             }), (0, wo.jsx)("table", {
                                 width: "100%",
                                 children: (0, wo.jsxs)("tbody", {
                                     children: [(0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "ID:"
                                         }), (0, wo.jsxs)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: [null === t || void 0 === t ? void 0 : t.id, (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                 children: null === t || void 0 === t ? void 0 : t.subnet_arn
                                             })]
                                         })]
                                     }), (null === t || void 0 === t ? void 0 : t.stack) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Stack:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.stack
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "CIDR:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.cidr
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Zone:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.zone
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "VPC:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.vpc
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Status:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.status
                                         })]
                                     }), (0, wo.jsx)(aa, {
                                         top: "4pt",
                                         bottom: "2pt",
                                         table: 2
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return i(et({}, e = "showTags", !o[e]));
                                             var e
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Tags:"
                                         }), (0, wo.jsx)("td", {
                                             children: a() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67331,26 +67334,26 @@
                                     }), a() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(xf, {
+                                                children: (0, wo.jsx)(Nf, {
                                                     tags: null === t || void 0 === t ? void 0 : t.tags
                                                 })
                                             })
                                         })
                                     })]
                                 })
                             })]
                         })
                     })
                 },
-                Mf = function(e) {
+                jf = function(e) {
                     var t, n = e.vpcId,
                         r = e.notitle,
                         o = e.keyedState,
                         i = e.hide,
                         a = "true" === (null === (t = $e()[0].get("all")) || void 0 === t ? void 0 : t.toLowerCase()),
                         s = n ? "?vpc=".concat(n) : "",
                         u = Ua("/aws/security_groups".concat(a ? "/all" : "").concat(s), {
@@ -67388,28 +67391,28 @@
                                     marginTop: "2pt"
                                 },
                                 children: (0, wo.jsx)(Lo, {
                                     label: "Loading security groups"
                                 })
                             }), u.map((function(e) {
                                 return (0, wo.jsxs)("div", {
-                                    children: [(0, wo.jsx)(jf, {
+                                    children: [(0, wo.jsx)(bf, {
                                         securityGroup: e,
                                         keyedState: null === o || void 0 === o ? void 0 : o.keyed(e.id)
                                     }), (0, wo.jsx)("div", {
                                         style: {
                                             height: "4pt"
                                         }
                                     })]
                                 }, e.id)
                             }))]
                         })]
                     })
                 },
-                jf = function(e) {
+                bf = function(e) {
                     var t = e.securityGroup,
                         n = e.keyedState,
                         r = l(Va(n), 2),
                         o = r[0],
                         i = r[1],
                         a = function(e) {
                             return o[e]
@@ -67452,60 +67455,60 @@
                                     bottom: "2pt"
                                 })]
                             }), (0, wo.jsx)("table", {
                                 width: "100%",
                                 children: (0, wo.jsxs)("tbody", {
                                     children: [(0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "ID:"
                                         }), (0, wo.jsxs)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: [null === t || void 0 === t ? void 0 : t.id, (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                 children: null === t || void 0 === t ? void 0 : t.securityGroup
                                             })]
                                         })]
                                     }), (null === t || void 0 === t ? void 0 : t.stack) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Stack:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.stack
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Description:"
                                         }), (0, wo.jsx)("td", {
                                             style: {
                                                 whiteSpace: "break-spaces",
                                                 wordBreak: "break-all"
                                             },
                                             children: null === t || void 0 === t ? void 0 : t.description
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "VPC:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.vpc
                                         })]
                                     }), (0, wo.jsx)(aa, {
                                         top: "4pt",
                                         bottom: "2pt",
                                         table: 2
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return s("showInboundRules")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Inbound Rules:"
                                         }), (0, wo.jsx)("td", {
                                             children: u() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsxs)("small", {
                                                     children: [(0, wo.jsx)("u", {
                                                         children: "Hide"
                                                     }), "\xa0", po.DownArrowHollow]
@@ -67521,27 +67524,27 @@
                                     }), u() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(bf, {
+                                                children: (0, wo.jsx)(wf, {
                                                     securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                     direction: "inbound"
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return s("showOutboundRules")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Outbound Rules:"
                                         }), (0, wo.jsx)("td", {
                                             children: c() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67557,27 +67560,27 @@
                                     }), c() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(bf, {
+                                                children: (0, wo.jsx)(wf, {
                                                     securityGroupId: null === t || void 0 === t ? void 0 : t.id,
                                                     direction: "outbound"
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         onClick: function() {
                                             return s("showTags")
                                         },
                                         className: "pointer",
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Tags:"
                                         }), (0, wo.jsx)("td", {
                                             children: d() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -67593,26 +67596,26 @@
                                     }), d() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
                                                 colSpan: "2",
-                                                children: (0, wo.jsx)(xf, {
+                                                children: (0, wo.jsx)(Nf, {
                                                     tags: null === t || void 0 === t ? void 0 : t.tags
                                                 })
                                             })
                                         })
                                     })]
                                 })
                             })]
                         })
                     })
                 },
-                bf = function(e) {
+                wf = function(e) {
                     var t = e.securityGroupId,
                         n = e.direction,
                         r = "inbound" === n ? "?direction=inbound" : "outbound" === n ? "?direction=outbound" : "",
                         o = Ua("/aws/security_group_rules/".concat(t).concat(r), {
                             cache: !0
                         });
                     return (0, wo.jsxs)(wo.Fragment, {
@@ -67622,26 +67625,26 @@
                                 paddingBottom: "10pt"
                             },
                             children: (0, wo.jsx)(Lo, {
                                 label: "Loading security group rules"
                             })
                         }), null === o || void 0 === o ? void 0 : o.map((function(e) {
                             return (0, wo.jsxs)("div", {
-                                children: [(0, wo.jsx)(wf, {
+                                children: [(0, wo.jsx)(xf, {
                                     securityGroupRule: e
                                 }), (0, wo.jsx)("div", {
                                     style: {
                                         height: "4pt"
                                     }
                                 })]
                             }, e.id)
                         }))]
                     })
                 },
-                wf = function(e) {
+                xf = function(e) {
                     var t = e.securityGroupRule;
 
                     function n(e) {
                         var t, n;
                         if ("TCP" === (null === e || void 0 === e || null === (t = e.protocol) || void 0 === t ? void 0 : t.toUpperCase())) {
                             if (22 === (null === e || void 0 === e ? void 0 : e.port_from) && 22 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "SSH";
                             if (443 === (null === e || void 0 === e ? void 0 : e.port_from) && 443 === (null === e || void 0 === e ? void 0 : e.port_thru)) return "HTTPS";
@@ -67694,78 +67697,78 @@
                                     bottom: "2pt"
                                 })]
                             }), (0, wo.jsx)("table", {
                                 width: "100%",
                                 children: (0, wo.jsxs)("tbody", {
                                     children: [(0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Direction:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null !== t && void 0 !== t && t.egress ? "Outbound" : "Inbound"
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Protocol:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: r(t)
                                         })]
                                     }), n(t) !== r(t) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Type:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: n(t)
                                         })]
                                     }), o(t) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Port:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: o(t)
                                         })]
                                     }), (null === t || void 0 === t ? void 0 : t.cidr) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "CIDR:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.cidr
                                         })]
                                     }), (null === t || void 0 === t ? void 0 : t.description) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Description:"
                                         }), (0, wo.jsx)("td", {
                                             style: {
                                                 whiteSpace: "break-spaces",
                                                 wordBreak: "break-all"
                                             },
                                             children: null === t || void 0 === t ? void 0 : t.description
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Security Group:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === t || void 0 === t ? void 0 : t.security_group
                                         })]
                                     })]
                                 })
                             })]
                         })
                     })
                 },
-                xf = function(e) {
+                Nf = function(e) {
                     var t;
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%"
                         },
                         children: (0, wo.jsx)("div", {
@@ -67779,15 +67782,15 @@
                                         return (0, wo.jsxs)("li", {
                                             children: [(0, wo.jsx)("b", {
                                                 children: t
                                             }), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("div", {
                                                 style: {
                                                     wordBreak: "break-all"
                                                 },
-                                                children: df(e.tags[t]) ? (0, wo.jsx)(wo.Fragment, {
+                                                children: pf(e.tags[t]) ? (0, wo.jsx)(wo.Fragment, {
                                                     children: (0, wo.jsx)("span", {
                                                         style: {
                                                             color: "red"
                                                         },
                                                         children: "REDACTED"
                                                     })
                                                 }) : (0, wo.jsx)(wo.Fragment, {
@@ -67801,15 +67804,15 @@
                                 children: (0, wo.jsx)("li", {
                                     children: "No tags."
                                 })
                             })
                         })
                     })
                 },
-                Nf = function(e) {
+                If = function(e) {
                     var t = Ua("/aws/stacks", {
                         cache: !0
                     });
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("div", {
                             children: (0, wo.jsx)("b", {
                                 children: "AWS Stacks"
@@ -67840,15 +67843,15 @@
                                         iff: r + 1 < t.length
                                     })]
                                 })
                             }))]
                         })]
                     })
                 },
-                If = function(e) {
+                Df = function(e) {
                     var t, n, r, o, i, a, s, u, c, d, p, f, h = e.stackName,
                         g = e.keyedState,
                         y = e.hide,
                         m = l(Va(g), 2),
                         v = m[0],
                         M = m[1],
                         j = Ua("/aws/stacks/".concat(h), {
@@ -67915,88 +67918,88 @@
                             children: j.loading ? (0, wo.jsx)(Lo, {
                                 label: "Loading stack info"
                             }) : (0, wo.jsx)("table", {
                                 width: "100%",
                                 children: (0, wo.jsxs)("tbody", {
                                     children: [(0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Name:"
                                         }), (0, wo.jsx)("td", {
-                                            style: nt(nt({}, cf), {}, {
+                                            style: nt(nt({}, df), {}, {
                                                 wordBreak: "break-all"
                                             }),
                                             children: h
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "ID:"
                                         }), (0, wo.jsx)("td", {
-                                            style: nt(nt({}, cf), {}, {
+                                            style: nt(nt({}, df), {}, {
                                                 wordBreak: "break-all"
                                             }),
                                             children: (0, wo.jsx)("small", {
                                                 children: null === (n = j.data) || void 0 === n ? void 0 : n.id
                                             })
                                         })]
                                     }), (null === (r = j.data) || void 0 === r ? void 0 : r.role_arn) && (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Role:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: (null === (o = j.data) || void 0 === o ? void 0 : o.role_arn) || po.EmptySet
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Description:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === (i = j.data) || void 0 === i ? void 0 : i.description
                                         })]
                                     }), (0, wo.jsx)(aa, {
                                         top: "2pt",
                                         bottom: "2pt",
                                         table: 2
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Status:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === (a = j.data) || void 0 === a ? void 0 : a.status
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Created:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === (s = j.data) || void 0 === s ? void 0 : s.created
                                         })]
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Updated:"
                                         }), (0, wo.jsx)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: null === (u = j.data) || void 0 === u ? void 0 : u.updated
                                         })]
                                     }), (0, wo.jsx)(aa, {
                                         top: "2pt",
                                         bottom: "2pt",
                                         table: 2
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Outputs:"
                                         }), (0, wo.jsxs)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: [x() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     className: "pointer",
                                                     onClick: N,
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -68021,25 +68024,25 @@
                                     }), x() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 colSpan: "2",
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
-                                                children: (0, wo.jsx)(Df, {
+                                                children: (0, wo.jsx)(Lf, {
                                                     stackName: h
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Parameters:"
                                         }), (0, wo.jsxs)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: [I() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     className: "pointer",
                                                     onClick: D,
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -68064,25 +68067,25 @@
                                     }), I() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 colSpan: "2",
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
-                                                children: (0, wo.jsx)(Lf, {
+                                                children: (0, wo.jsx)(Sf, {
                                                     stackName: h
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Resources:"
                                         }), (0, wo.jsxs)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: [L() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     className: "pointer",
                                                     onClick: S,
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -68107,25 +68110,25 @@
                                     }), L() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 colSpan: "2",
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
-                                                children: (0, wo.jsx)(Sf, {
+                                                children: (0, wo.jsx)(kf, {
                                                     stackName: h
                                                 })
                                             })
                                         })
                                     }), (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsx)("td", {
-                                            style: lf,
+                                            style: cf,
                                             children: "Template:"
                                         }), (0, wo.jsxs)("td", {
-                                            style: cf,
+                                            style: df,
                                             children: [k() ? (0, wo.jsx)(wo.Fragment, {
                                                 children: (0, wo.jsx)("small", {
                                                     className: "pointer",
                                                     onClick: C,
                                                     children: (0, wo.jsxs)("u", {
                                                         children: ["Hide\xa0", po.DownArrowHollow]
                                                     })
@@ -68150,26 +68153,26 @@
                                     }), k() && (0, wo.jsx)(wo.Fragment, {
                                         children: (0, wo.jsx)("tr", {
                                             children: (0, wo.jsx)("td", {
                                                 colSpan: "2",
                                                 style: {
                                                     paddingTop: "2pt"
                                                 },
-                                                children: (0, wo.jsx)(kf, {
+                                                children: (0, wo.jsx)(Cf, {
                                                     stackName: h
                                                 })
                                             })
                                         })
                                     })]
                                 })
                             })
                         })]
                     })
                 },
-                Df = function(e) {
+                Lf = function(e) {
                     var t, n = Ua("/aws/stacks/".concat(e.stackName, "/outputs"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
@@ -68196,15 +68199,15 @@
                                         return (0, wo.jsxs)("li", {
                                             children: [(0, wo.jsx)("b", {
                                                 children: e
                                             }), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("div", {
                                                 style: {
                                                     wordBreak: "break-all"
                                                 },
-                                                children: df(n.data[e]) ? (0, wo.jsx)(wo.Fragment, {
+                                                children: pf(n.data[e]) ? (0, wo.jsx)(wo.Fragment, {
                                                     children: (0, wo.jsx)("span", {
                                                         style: {
                                                             color: "red"
                                                         },
                                                         children: "REDACTED"
                                                     })
                                                 }) : (0, wo.jsx)(wo.Fragment, {
@@ -68214,15 +68217,15 @@
                                         }, e)
                                     })))
                                 })
                             })
                         })
                     })
                 },
-                Lf = function(e) {
+                Sf = function(e) {
                     var t, n = Ua("/aws/stacks/".concat(e.stackName, "/parameters"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
@@ -68249,15 +68252,15 @@
                                         return (0, wo.jsxs)("li", {
                                             children: [(0, wo.jsx)("b", {
                                                 children: e
                                             }), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("div", {
                                                 style: {
                                                     wordBreak: "break-all"
                                                 },
-                                                children: df(n.data[e]) ? (0, wo.jsx)(wo.Fragment, {
+                                                children: pf(n.data[e]) ? (0, wo.jsx)(wo.Fragment, {
                                                     children: (0, wo.jsx)("span", {
                                                         style: {
                                                             color: "red"
                                                         },
                                                         children: "REDACTED"
                                                     })
                                                 }) : (0, wo.jsx)(wo.Fragment, {
@@ -68267,15 +68270,15 @@
                                         }, e)
                                     })))
                                 })
                             })
                         })
                     })
                 },
-                Sf = function(e) {
+                kf = function(e) {
                     var t, n = Ua("/aws/stacks/".concat(e.stackName, "/resources"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%",
@@ -68305,15 +68308,15 @@
                                                     wordBreak: "break-all"
                                                 },
                                                 children: e
                                             }), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("div", {
                                                 style: {
                                                     wordBreak: "break-all"
                                                 },
-                                                children: df(n.data[e]) ? (0, wo.jsx)(wo.Fragment, {
+                                                children: pf(n.data[e]) ? (0, wo.jsx)(wo.Fragment, {
                                                     children: (0, wo.jsx)("span", {
                                                         style: {
                                                             color: "red"
                                                         },
                                                         children: "REDACTED"
                                                     })
                                                 }) : (0, wo.jsx)(wo.Fragment, {
@@ -68323,15 +68326,15 @@
                                         }, e)
                                     })))
                                 })
                             })
                         })
                     })
                 },
-                kf = function(e) {
+                Cf = function(e) {
                     var t = Ua("/aws/stacks/".concat(e.stackName, "/template"), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         style: {
                             width: "100%",
                             maxWidth: "100%"
@@ -68361,15 +68364,15 @@
                                     },
                                     children: Dt.IsObject(t.data) ? Ia.Format(t.data) : t.data
                                 })
                             })
                         })
                     })
                 },
-                Cf = function(e) {
+                Ef = function(e) {
                     var t, n, r, o, i = e.hide,
                         a = Ua("/info", {
                             cache: !0
                         });
                     return (0, wo.jsxs)("div", {
                         style: {
                             width: "100%",
@@ -68396,27 +68399,27 @@
                             className: "box margin",
                             children: [a.loading && (0, wo.jsx)(Lo, {
                                 label: "Loading Ecosystem"
                             }), !a.loading && Ia.Format(null === (r = a.data) || void 0 === r || null === (o = r.buckets) || void 0 === o ? void 0 : o.ecosystem)]
                         })]
                     })
                 },
-                Ef = function(e) {
+                Tf = function(e) {
                     var t, n, r, o, i = Ua("//aws/ecs/clusters/".concat(encodeURIComponent(e.cluster)), {
                         cache: !0
                     });
                     return (0, wo.jsx)("div", {
                         className: "box",
                         style: {
                             background: "inherit",
                             marginTop: "2pt",
                             marginBottom: "3pt",
                             overflow: "auto"
                         },
-                        children: (0, wo.jsx)(uf, {
+                        children: (0, wo.jsx)(lf, {
                             data: i.data,
                             yaml: !0,
                             both: !0,
                             children: (0, wo.jsxs)("small", {
                                 children: [e.clusterDisplayName != (null === (t = i.data) || void 0 === t ? void 0 : t.name) && (0, wo.jsxs)(wo.Fragment, {
                                     children: [(0, wo.jsx)("b", {
                                         children: "Name"
@@ -68426,15 +68429,15 @@
                                 }), ": ", null === (r = i.data) || void 0 === r ? void 0 : r.arn, " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("b", {
                                     children: "Deployed"
                                 }), ": ", null === (o = i.data) || void 0 === o ? void 0 : o.most_recent_deployed]
                             })
                         })
                     })
                 },
-                Tf = function(e) {
+                Af = function(e) {
                     var t, n = l(Va(e.keyedState), 2),
                         r = n[0],
                         o = n[1],
                         i = function() {
                             return r["detail"]
                         },
                         a = e.commonInitialSubstring ? null === (t = e.cluster) || void 0 === t ? void 0 : t.replace(e.commonInitialSubstring, "") : e.cluster;
@@ -68451,23 +68454,23 @@
                             children: a
                         }), (0, wo.jsx)(la, {
                             href: "https://us-east-1.console.aws.amazon.com/ecs/v2/clusters/".concat(a, "/services?region=us-east-1"),
                             style: {
                                 marginLeft: "6pt"
                             }
                         }), i() ? (0, wo.jsx)(wo.Fragment, {
-                            children: (0, wo.jsx)(Ef, {
+                            children: (0, wo.jsx)(Tf, {
                                 cluster: e.cluster,
                                 clusterDisplayName: a,
                                 keyedState: e.keyedState
                             })
                         }) : (0, wo.jsx)(wo.Fragment, {})]
                     })
                 },
-                Af = function(e) {
+                zf = function(e) {
                     var t = e.keyedState,
                         n = e.hide,
                         r = Ua("//aws/ecs/clusters"),
                         o = wt.LongestCommonInitialSubstring(r.data);
                     return (0, wo.jsxs)("div", {
                         style: {
                             marginBottom: "8pt"
@@ -68495,75 +68498,75 @@
                             className: "box lighten nomargin",
                             children: [r.loading && (0, wo.jsx)("div", {
                                 children: (0, wo.jsx)(Lo, {
                                     label: "Loading ECS clusters"
                                 })
                             }), r.map((function(e, n) {
                                 return (0, wo.jsxs)("div", {
-                                    children: [(0, wo.jsx)(Tf, {
+                                    children: [(0, wo.jsx)(Af, {
                                         cluster: e,
                                         commonInitialSubstring: o,
                                         keyedState: null === t || void 0 === t ? void 0 : t.keyed(e)
                                     }), n < r.length - 1 && (0, wo.jsx)(aa, {
                                         top: "2pt",
                                         bottom: "2pt",
                                         dotted: !0
                                     })]
                                 }, e)
                             }))]
                         })]
                     })
                 },
-                zf = function() {
+                Of = function() {
                     var e = Va(),
                         n = Za(),
                         r = [{
                             type: "stack",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(If, {
+                                return (0, wo.jsx)(Df, {
                                     stackName: e,
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }, {
                             type: "vpcs",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(gf, {
+                                return (0, wo.jsx)(yf, {
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }, {
                             type: "subnets-public",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(mf, {
+                                return (0, wo.jsx)(vf, {
                                     type: "public",
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }, {
                             type: "subnets-private",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(mf, {
+                                return (0, wo.jsx)(vf, {
                                     type: "private",
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }, {
                             type: "security-groups",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(Mf, {
+                                return (0, wo.jsx)(jf, {
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }, {
                             type: "gac",
                             create: function(e, t, n, r) {
@@ -68580,23 +68583,23 @@
                                         return n.unsetList("secrets", e), r()
                                     }
                                 })
                             }
                         }, {
                             type: "ecosystem",
                             create: function(e, t, n, r) {
-                                return (0, wo.jsx)(Cf, {
+                                return (0, wo.jsx)(Ef, {
                                     hide: n
                                 })
                             }
                         }, {
                             type: "ecs-clusters",
                             create: function(e, t, n, r) {
                                 var o = r.keyedState;
-                                return (0, wo.jsx)(Af, {
+                                return (0, wo.jsx)(zf, {
                                     keyedState: o.keyed(t),
                                     hide: n
                                 })
                             }
                         }],
                         o = Qa(r),
                         i = Qa(r);
@@ -68623,26 +68626,26 @@
                         children: (0, wo.jsx)("tbody", {
                             children: (0, wo.jsxs)("tr", {
                                 children: [(0, wo.jsxs)("td", {
                                     style: {
                                         verticalAlign: "top",
                                         paddingRight: "8pt"
                                     },
-                                    children: [(0, wo.jsx)(hf, {
+                                    children: [(0, wo.jsx)(gf, {
                                         showGac: function() {
                                             return o.selected("gac")
                                         },
                                         toggleGac: function() {
                                             return o.toggle("gac")
                                         },
                                         showEcosystem: function() {
                                             return o.selected("ecosystem")
                                         },
                                         toggleEcosystem: s
-                                    }), (0, wo.jsx)(pf, {
+                                    }), (0, wo.jsx)(ff, {
                                         keyedState: e,
                                         showVpcs: function() {
                                             return o.selected("vpcs")
                                         },
                                         toggleVpcs: a,
                                         showSubnetsPublic: function() {
                                             return i.selected("subnets-public")
@@ -68658,29 +68661,29 @@
                                         },
                                         showSecurityGroups: function() {
                                             return i.selected("security-groups")
                                         },
                                         toggleSecurityGroups: function() {
                                             return i.toggle("security-groups")
                                         }
-                                    }), (0, wo.jsx)(ff, {
+                                    }), (0, wo.jsx)(hf, {
                                         showEcsClusters: function() {
                                             return o.selected("ecs-clusters")
                                         },
                                         toggleEcsClusters: function() {
                                             return o.toggle("ecs-clusters")
                                         }
                                     }), (0, wo.jsx)(Ja, {
                                         toggleSecrets: function(e) {
                                             return o.toggle("secrets", e) ? n.setList("secrets", e) : n.unsetList("secrets", e)
                                         },
                                         selectedSecrets: function(e) {
                                             return o.selected("secrets", e)
                                         }
-                                    }), (0, wo.jsx)(Nf, {
+                                    }), (0, wo.jsx)(If, {
                                         toggleStack: function(e) {
                                             return o.toggle("stack", e)
                                         },
                                         selectedStack: function(e) {
                                             return o.selected("stack", e)
                                         }
                                     })]
@@ -68709,15 +68712,15 @@
                                         }, t.key)
                                     }))
                                 })]
                             })
                         })
                     })
                 },
-                Of = function(e) {
+                _f = function(e) {
                     var t = Fa();
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "container",
                             id: "login_container",
                             children: (0, wo.jsxs)("div", {
                                 className: "boxstyle check-warn",
@@ -68746,56 +68749,56 @@
                                         })
                                     }), " page."]
                                 })]
                             })
                         })
                     })
                 },
-                _f = function() {
+                Uf = function() {
                     var e = me().state.url;
                     return e.startsWith(window.location.origin) && (e = e.substring(window.location.origin.length)), (0, wo.jsx)(ze, {
                         to: e,
                         replace: !0
                     })
                 },
-                Uf = function(e) {
+                Pf = function(e) {
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsx)("div", {
                             className: "box thickborder",
                             style: {
                                 marginBottom: "6pt"
                             },
                             children: (0, wo.jsx)(pa, {
                                 certificate: e.certificate
                             })
                         })
                     })
                 },
-                Pf = function(e) {
+                Rf = function(e) {
                     var t, n = l($e(), 1)[0].get("hostname"),
                         r = Ua("/certificates?hostname=".concat(n));
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
-                                    children: (0, wo.jsx)(Uf, {
+                                    children: (0, wo.jsx)(Pf, {
                                         certificate: e
                                     })
                                 }, e.serial_number)
                             }))]
                         })
                     })
                 },
-                Rf = function(e) {
+                Ff = function(e) {
                     var t = Ua("/portal_access_key");
                     return (0, wo.jsx)(wo.Fragment, {
                         children: (0, wo.jsxs)("div", {
                             className: "container",
                             style: {
                                 width: "800pt"
                             },
@@ -68809,15 +68812,15 @@
                                 children: (0, wo.jsx)(ca, {
                                     accessKey: t.data
                                 })
                             })]
                         })
                     })
                 },
-                Ff = function() {
+                Bf = function() {
                     var e = Ua("/users/projects", {
                             cache: !0
                         }),
                         t = Ua("/users/roles", {
                             cache: !0
                         }),
                         n = Ua("/users/institutions", {
@@ -68875,15 +68878,15 @@
                                 return (null === e || void 0 === e ? void 0 : e.map((function(e) {
                                     return o.title(e)
                                 })).join(", ")) || ""
                             }
                         };
                     return o
                 },
-                Bf = [{
+                Yf = [{
                     name: "email",
                     label: "Email Address",
                     type: "email",
                     focus: !0,
                     required: !0
                 }, {
                     name: "first_name",
@@ -68930,38 +68933,38 @@
                 }, {
                     name: "uuid",
                     label: "UUID",
                     readonly: !0,
                     readonlyOverridableOnCreate: !0,
                     readonlyOverridableOnCreateMessage: "Warning: Only set UUID if you know what you are doing."
                 }],
-                Yf = {
+                Qf = {
                     PrincipalInvestigatorLine: function(e) {
                         var t, n, r = e.institution,
-                            o = Ff();
+                            o = Bf();
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
                         var e = Fa(),
-                            n = tn.IsFoursightFourfront(e) ? Bf.filter((function(e) {
+                            n = tn.IsFoursightFourfront(e) ? Yf.filter((function(e) {
                                 return "project" !== e.name && "role" !== e.name && "institution" !== e.name
-                            })) : Bf;
+                            })) : Yf;
                         return (0, t.useState)(no.Clone(n))
                     }
                 },
-                Qf = function(e) {
+                Gf = function(e) {
                     var t = Ua("/users/".concat(e.email, "?raw=true"));
                     return (0, wo.jsxs)("pre", {
                         className: "box",
                         children: [(0, wo.jsx)("span", {
                             style: {
                                 float: "right",
                                 marginTop: "-6pt",
@@ -68975,15 +68978,15 @@
                         }), t.loading ? (0, wo.jsx)(wo.Fragment, {
                             children: (0, wo.jsx)(Lo, {})
                         }) : (0, wo.jsx)(wo.Fragment, {
                             children: Ia.Format(t.data)
                         })]
                     })
                 },
-                Gf = function(e) {
+                Wf = function(e) {
                     var n = {
                             color: "var(--box-fg)",
                             fontWeight: "bold",
                             fontSize: "small",
                             paddingTop: "1pt",
                             verticalAlign: "top",
                             width: "5%",
@@ -69092,16 +69095,16 @@
                                         })]
                                     }, o.name)
                                 }))
                             })
                         })
                     })
                 },
-                Wf = function(e) {
-                    var t = Ff(),
+                Hf = function(e) {
+                    var t = Bf(),
                         n = [{
                             label: "Email",
                             name: "email"
                         }, {
                             label: "First Name",
                             name: "first_name"
                         }, {
@@ -69124,61 +69127,61 @@
                             name: "role",
                             map: function(n) {
                                 return t.userRoleTitle(e.user, e.user.project)
                             }
                         }, {
                             label: "Roles",
                             name: "roles",
-                            ui: (0, wo.jsx)(Hf, {
+                            ui: (0, wo.jsx)(Vf, {
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
-                                return (0, wo.jsx)(Yf.PrincipalInvestigatorLine, {
+                                return (0, wo.jsx)(Qf.PrincipalInvestigatorLine, {
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
-                                return Ss.Format(e)
+                                return ks.Format(e)
                             }
                         }, {
                             label: "Updated",
                             name: "updated",
                             map: function(e) {
-                                return Ss.Format(e)
+                                return ks.Format(e)
                             }
                         }, {
                             label: "UUID",
                             name: "uuid"
                         }];
                     return tn.IsFoursightFourfront(Fa()) && (n = n.filter((function(e) {
                         return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
-                    }))), (0, wo.jsx)(Gf, {
+                    }))), (0, wo.jsx)(Wf, {
                         keys: n,
                         value: e.user,
                         separators: !0
                     })
                 },
-                Hf = function(e) {
-                    var t = Ff();
+                Vf = function(e) {
+                    var t = Bf();
                     return (0, wo.jsx)("div", {
                         className: "box lighten",
                         style: {
                             marginTop: "2pt",
                             marginBottom: "2pt"
                         },
                         children: (0, wo.jsx)("table", {
@@ -69241,15 +69244,15 @@
                                         })]
                                     }, e.project)
                                 }))]
                             })
                         })
                     })
                 },
-                Vf = function(e) {
+                Zf = function(e) {
                     var n, r, o, i = je().email,
                         a = l((0, t.useState)(!1), 2),
                         s = a[0],
                         u = a[1],
                         c = Me();
                     var d = Ua({
                         url: "/users/".concat(i),
@@ -69365,25 +69368,25 @@
                                                 float: "right",
                                                 fontSize: "small",
                                                 marginTop: "-1pt",
                                                 marginRight: "2pt"
                                             },
                                             children: "Edit"
                                         })]
-                                    }), s ? (0, wo.jsx)(Qf, {
+                                    }), s ? (0, wo.jsx)(Gf, {
                                         email: e.email
-                                    }) : (0, wo.jsx)(Wf, {
+                                    }) : (0, wo.jsx)(Hf, {
                                         user: e
                                     })]
                                 }, e.uuid)
                             }))]
                         })
                     })
                 },
-                Zf = function(e) {
+                qf = function(e) {
                     var n = Ua(e.url, {
                             nofetch: !0,
                             cache: !0
                         }),
                         r = l((0, t.useState)(e.selected), 2),
                         o = r[0],
                         i = r[1];
@@ -69416,15 +69419,15 @@
                                 }, e.id) : null
                             }))]
                         }), e.subComponent && (0, wo.jsx)(wo.Fragment, {
                             children: e.subComponent(o)
                         })]
                     })
                 },
-                qf = function(e) {
+                Jf = function(e) {
                     var n = e.input,
                         r = e.valueOf,
                         o = e.handleChange,
                         i = e.isDisabled,
                         a = l((0, t.useState)(n.readonly), 2),
                         s = a[0],
                         u = a[1];
@@ -69483,15 +69486,15 @@
                                         children: n.readonlyOverridableOnCreateMessage
                                     })
                                 })]
                             })]
                         })]
                     })
                 },
-                Jf = function(e) {
+                Kf = function(e) {
                     var n = e.inputs,
                         r = (e.setInputs, e.title, e.loading),
                         o = e.onCreate,
                         i = e.onUpdate,
                         a = e.onDelete,
                         s = e.onCancel,
                         u = e.onRefresh,
@@ -69742,27 +69745,27 @@
                                                             }), (0, wo.jsx)("option", {
                                                                 value: !0,
                                                                 children: "True"
                                                             })]
                                                         })
                                                     }) : (0, wo.jsx)(wo.Fragment, {
                                                         children: "select" === e.type ? (0, wo.jsx)(wo.Fragment, {
-                                                            children: (0, wo.jsx)(Zf, {
+                                                            children: (0, wo.jsx)(qf, {
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
-                                                            children: (0, wo.jsx)(qf, {
+                                                            children: (0, wo.jsx)(Jf, {
                                                                 input: e,
                                                                 valueOf: _,
                                                                 handleChange: A,
                                                                 isDisabled: B,
                                                                 isCreate: !Dt.IsNull(o)
                                                             })
                                                         })
@@ -69925,28 +69928,28 @@
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                Kf = function() {
+                Xf = function() {
                     var e = Ua(rn.Url("/users"), {
                             method: "POST",
                             nofetch: !0
                         }),
-                        n = l(Yf.useUserInputs(), 2),
+                        n = l(Qf.useUserInputs(), 2),
                         r = n[0],
                         o = (n[1], Me());
                     return (0, t.useEffect)((function() {
                         var e = r.find((function(e) {
                             return "institution" === e.name
                         }));
                         e && (e.subComponent = function(e) {
-                            return (0, wo.jsx)(Yf.PrincipalInvestigatorLine, {
+                            return (0, wo.jsx)(Qf.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         })
                     }), []), (0, wo.jsx)("center", {
                         children: (0, wo.jsx)("table", {
                             children: (0, wo.jsxs)("tbody", {
                                 children: [(0, wo.jsx)("tr", {
@@ -69973,15 +69976,15 @@
                                                     children: "List"
                                                 })
                                             })
                                         })]
                                     })
                                 }), (0, wo.jsx)("tr", {
                                     children: (0, wo.jsx)("td", {
-                                        children: (0, wo.jsx)(Jf, {
+                                        children: (0, wo.jsx)(Kf, {
                                             title: "Edit User",
                                             inputs: r,
                                             onCreate: function(t) {
                                                 t.admin ? (delete t.admin, t = nt(nt({}, t), {}, {
                                                     groups: ["admin"]
                                                 })) : (delete t.admin, t = nt(nt({}, t), {}, {
                                                     groups: []
@@ -70001,17 +70004,17 @@
                                         })
                                     })
                                 })]
                             })
                         })
                     })
                 },
-                Xf = function() {
+                $f = function() {
                     var e = je().uuid,
-                        n = l(Yf.useUserInputs(), 2),
+                        n = l(Qf.useUserInputs(), 2),
                         r = n[0],
                         o = n[1],
                         i = l((0, t.useState)(!1), 2),
                         a = i[0],
                         s = i[1],
                         u = l(ws(), 1)[0],
                         d = Ua({
@@ -70021,41 +70024,41 @@
                                 o((function(t) {
                                     var n, r = c(t);
                                     try {
                                         for (r.s(); !(n = r.n()).done;) {
                                             var o, i = n.value;
                                             "email" === i.name ? i.value = e.email : "first_name" === i.name ? i.value = e.first_name : "last_name" === i.name ? i.value = e.last_name : "admin" === i.name ? i.value = !(null === (o = e.groups) || void 0 === o || !o.includes("admin")) : "project" === i.name ? i.value = e.project : "role" === i.name ? i.value = function(t) {
                                                 return void 0 === t || null === t ? "-" : f.userRole(e, t || (null === e || void 0 === e ? void 0 : e.project)) || "-"
-                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = Ss.Format(e.created) : "updated" === i.name ? i.value = Ss.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
+                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = ks.Format(e.created) : "updated" === i.name ? i.value = ks.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
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
-                        f = Ff(),
+                        f = Bf(),
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
-                            return (0, wo.jsx)(Yf.PrincipalInvestigatorLine, {
+                            return (0, wo.jsx)(Qf.PrincipalInvestigatorLine, {
                                 institution: e
                             })
                         })
                     }), [e]), (0, wo.jsx)("center", {
                         children: (0, wo.jsx)("table", {
                             children: (0, wo.jsxs)("tbody", {
                                 children: [(0, wo.jsx)("tr", {
@@ -70096,15 +70099,15 @@
                                                 children: ["The specified user was not found: ", e, " ", (0, wo.jsx)("p", {}), (0, wo.jsx)("button", {
                                                     className: "button cancel",
                                                     onClick: g,
                                                     children: "Cancel"
                                                 })]
                                             })
                                         }) : (0, wo.jsx)(wo.Fragment, {
-                                            children: (0, wo.jsx)(Jf, {
+                                            children: (0, wo.jsx)(Kf, {
                                                 title: "Edit User",
                                                 inputs: r,
                                                 setInputs: o,
                                                 onUpdate: function(t) {
                                                     var n, r = (null === (n = d.get("groups")) || void 0 === n ? void 0 : n.filter((function(e) {
                                                         return "admin" !== e
                                                     }))) || [];
@@ -70139,17 +70142,14 @@
                                         })
                                     })
                                 })]
                             })
                         })
                     })
                 },
-                $f = {
-                    Format: uo.FormatDate
-                },
                 eh = function(e) {
                     var n, r = e.columns,
                         o = e.data,
                         i = e.update,
                         a = e.initialSort,
                         s = e.children,
                         u = l($e(), 2),
@@ -70231,15 +70231,15 @@
                             border: "0",
                             children: (0, wo.jsx)("tbody", {
                                 children: (0, wo.jsxs)("tr", {
                                     children: [(0, wo.jsx)("td", {
                                         style: {
                                             width: "90%"
                                         },
-                                        children: (0, wo.jsx)(vu, {
+                                        children: (0, wo.jsx)(Mu, {
                                             pages: T,
                                             page: k,
                                             onChange: function(e) {
                                                 var t = e.selected;
                                                 m(t * f)
                                             },
                                             refresh: R,
@@ -70342,15 +70342,15 @@
                         i = Ua(),
                         a = l((0, t.useState)(r.get("search") || ""), 2),
                         s = a[0],
                         u = a[1],
                         c = l((0, t.useState)(wt.HasValue(s)), 2),
                         d = c[0],
                         p = c[1],
-                        f = Ff();
+                        f = Bf();
 
                     function h(t) {
                         var n = t.limit,
                             o = t.offset,
                             a = t.sort,
                             s = t.search,
                             u = t.onDone;
@@ -70596,22 +70596,22 @@
                                                 size: "small",
                                                 text: "Status: ".concat(e.status)
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: nt(nt({}, g), {}, {
                                                 whiteSpace: "nowrap"
                                             }),
-                                            children: [e.updated ? $f.Format(e.updated) : $f.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                            children: [e.updated ? Ns.Format(e.updated) : Ns.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                 children: e.updated ? uo.Format(e.updated) : uo.Format(e.created)
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: nt(nt({}, g), {}, {
                                                 whiteSpace: "nowrap"
                                             }),
-                                            children: [$f.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                            children: [Ns.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                 children: uo.Format(e.created)
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: nt(nt({}, g), {}, {
                                                 whiteSpace: "nowrap"
                                             }),
                                             children: ["\xa0\xa0", (0, wo.jsx)("button", {
@@ -70630,23 +70630,23 @@
                 nh = function() {
                     var e = Fa();
 
                     function t() {
                         return "/api/react/".concat(tn.PreferredName(tn.Default(e)), "/login")
                     }
                     return (0, wo.jsx)(He, {
-                        children: (0, wo.jsxs)(Uu, {
-                            children: [(0, wo.jsx)(_u, {}), (0, wo.jsx)("div", {
+                        children: (0, wo.jsxs)(Pu, {
+                            children: [(0, wo.jsx)(Uu, {}), (0, wo.jsx)("div", {
                                 style: {
                                     margin: "14pt"
                                 },
                                 children: (0, wo.jsxs)(Ue, {
                                     children: [(0, wo.jsx)(Oe, {
                                         path: "/api/react/cognito/callback",
-                                        element: (0, wo.jsx)(nf, {})
+                                        element: (0, wo.jsx)(rf, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/",
                                         element: (0, wo.jsx)(ze, {
                                             to: t()
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api",
@@ -70667,121 +70667,121 @@
                                         path: "/api/react/:environ/accounts",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
                                             children: (0, wo.jsx)(fs, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/env",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(Iu, {})
+                                            children: (0, wo.jsx)(Du, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/env",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(Iu, {})
+                                            children: (0, wo.jsx)(Du, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/login",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(of, {})
+                                            children: (0, wo.jsx)(af, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/checks",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(lu, {})
+                                            children: (0, wo.jsx)(cu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/checksnew",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(gu, {})
+                                            children: (0, wo.jsx)(yu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/checks/:check/history",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(xu, {})
+                                            children: (0, wo.jsx)(Nu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/home",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Pu, {})
+                                            children: (0, wo.jsx)(Ru, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/info",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Bu, {})
+                                            children: (0, wo.jsx)(Yu, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
                                             children: (0, wo.jsx)(th, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users/:email",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Vf, {})
+                                            children: (0, wo.jsx)(Zf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users/edit/:uuid",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Xf, {})
+                                            children: (0, wo.jsx)($f, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/users/create",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Kf, {})
+                                            children: (0, wo.jsx)(Xf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/gac/:environCompare",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(af, {})
+                                            children: (0, wo.jsx)(sf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/aws/s3",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
                                             children: (0, wo.jsx)(js, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/aws/infrastructure",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(zf, {})
+                                            children: (0, wo.jsx)(Of, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/certificates",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(Pf, {})
+                                            children: (0, wo.jsx)(Rf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/portal_access_key",
                                         element: (0, wo.jsx)(wa.KnownEnvRequired, {
-                                            children: (0, wo.jsx)(Rf, {})
+                                            children: (0, wo.jsx)(Ff, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/apicache",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
                                             children: (0, wo.jsx)(vs, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/forbidden",
-                                        element: (0, wo.jsx)(Lu, {})
+                                        element: (0, wo.jsx)(Su, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/error",
                                         element: (0, wo.jsx)(ma, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/error",
                                         element: (0, wo.jsx)(ma, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/redirect",
-                                        element: (0, wo.jsx)(_f, {})
+                                        element: (0, wo.jsx)(Uf, {})
                                     }), (0, wo.jsx)(Oe, {
                                         path: "*",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(Of, {})
+                                            children: (0, wo.jsx)(_f, {})
                                         })
                                     })]
                                 })
-                            }), (0, wo.jsx)(Du, {})]
+                            }), (0, wo.jsx)(Lu, {})]
                         })
                     })
                 },
                 rh = o.createRoot(document.getElementById("root"));
             "1" === Bt.Get("test_mode_strict_mode") ? rh.render((0, wo.jsx)(t.StrictMode, {
                 children: (0, wo.jsx)(nh, {})
             })) : rh.render((0, wo.jsx)("table", {
```

### Comparing `foursight_core-4.3.0.2b2/foursight_core/route_prefixes.py` & `foursight_core-4.3.0.2b3/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/routes.py` & `foursight_core-4.3.0.2b3/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/run_result.py` & `foursight_core-4.3.0.2b3/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/s3_connection.py` & `foursight_core-4.3.0.2b3/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0.2b3/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/sqs_utils.py` & `foursight_core-4.3.0.2b3/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/stage.py` & `foursight_core-4.3.0.2b3/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/base.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/header.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/history.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/info.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/unused.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/user.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/users.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0.2b3/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b2/pyproject.toml` & `foursight_core-4.3.0.2b3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0.2b2"  # TODO: To become 4.4.0
+version = "4.3.0.2b3"  # TODO: To become 4.4.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.3.0.2b2/PKG-INFO` & `foursight_core-4.3.0.2b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0.2b2
+Version: 4.3.0.2b3
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

