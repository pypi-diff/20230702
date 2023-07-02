# Comparing `tmp/foursight_core-4.3.0.2b4.tar.gz` & `tmp/foursight_core-4.3.0.2b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.3.0.2b4.tar", max compression
+gzip compressed data, was "foursight_core-4.3.0.2b5.tar", max compression
```

## Comparing `foursight_core-4.3.0.2b4.tar` & `foursight_core-4.3.0.2b5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-07-02 10:48:00.437516 foursight_core-4.3.0.2b4/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/app.py
--rw-r--r--   0        0        0   103622 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/app_utils.py
--rw-r--r--   0        0        0     1283 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/boto_s3.py
--rw-r--r--   0        0        0     1305 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/boto_sqs.py
--rw-r--r--   0        0        0     2589 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     7293 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-07-02 10:48:00.441516 foursight_core-4.3.0.2b4/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/decorators.py
--rw-r--r--   0        0        0    15846 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/deploy.py
--rw-r--r--   0        0        0     8169 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/environment.py
--rw-r--r--   0        0        0    11948 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5597 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/package.py
--rw-r--r--   0        0        0    16912 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     6629 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    22994 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3065 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6104 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28009 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20464 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6213 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4720 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     4096 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9466 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5216 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    88080 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11210 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    35908 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4805 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11953 2023-07-02 10:48:00.445516 foursight_core-4.3.0.2b4/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1862153 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/routes.py
--rw-r--r--   0        0        0    22941 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/run_result.py
--rw-r--r--   0        0        0     6380 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     5442 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1500 2023-07-02 10:48:00.457516 foursight_core-4.3.0.2b4/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-02 11:05:17.039921 foursight_core-4.3.0.2b5/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/app.py
+-rw-r--r--   0        0        0   103622 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/boto_s3.py
+-rw-r--r--   0        0        0     1305 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/boto_sqs.py
+-rw-r--r--   0        0        0     2589 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     7293 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-07-02 11:05:17.043921 foursight_core-4.3.0.2b5/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15846 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8169 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/environment.py
+-rw-r--r--   0        0        0    11948 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5597 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3065 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6104 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6213 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     4096 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5216 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    88080 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    35908 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11953 2023-07-02 11:05:17.047921 foursight_core-4.3.0.2b5/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1862184 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/routes.py
+-rw-r--r--   0        0        0    22941 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6380 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     5442 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1500 2023-07-02 11:05:17.059921 foursight_core-4.3.0.2b5/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 foursight_core-4.3.0.2b5/PKG-INFO
```

### Comparing `foursight_core-4.3.0.2b4/LICENSE.txt` & `foursight_core-4.3.0.2b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/abstract_connection.py` & `foursight_core-4.3.0.2b5/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/app_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/boto_s3.py` & `foursight_core-4.3.0.2b5/foursight_core/boto_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/boto_sqs.py` & `foursight_core-4.3.0.2b5/foursight_core/boto_sqs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/buckets.py` & `foursight_core-4.3.0.2b5/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/check_schema.py` & `foursight_core-4.3.0.2b5/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/check_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/ecs_checks.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/scaling_checks.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/checks/test_checks.py` & `foursight_core-4.3.0.2b5/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/decorators.py` & `foursight_core-4.3.0.2b5/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/deploy.py` & `foursight_core-4.3.0.2b5/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/environment.py` & `foursight_core-4.3.0.2b5/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/es_connection.py` & `foursight_core-4.3.0.2b5/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/exceptions.py` & `foursight_core-4.3.0.2b5/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/fs_connection.py` & `foursight_core-4.3.0.2b5/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/identity.py` & `foursight_core-4.3.0.2b5/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/mapping.json` & `foursight_core-4.3.0.2b5/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/package.py` & `foursight_core-4.3.0.2b5/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/auth.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/auth.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/auth0_config.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/auth0_config.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/aws_network.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/aws_network.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/aws_s3.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/aws_stacks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/checks.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/cognito.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/cognito.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/encryption.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/envs.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/envs.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/gac.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/gac.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/misc_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/misc_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/react_api.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/react_api.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/react_api_base.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/react_api_base.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/react_routes.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/react_routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/react_ui.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/react_ui.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/ui/index.html` & `foursight_core-4.3.0.2b5/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.3.0.2b5/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.3.0.2b5/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.2c892067.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.86e7492f.js.LICENSE.txt */ ! function() {
     var e = {
             3339: function(e, t, n) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 }), t.RawSha256 = void 0;
                 var r = n(3277),
@@ -49657,15 +49657,94 @@
                                     },
                                     children: no.Format(n.data)
                                 })]
                             })]
                         })]
                     })
                 },
-                Ms = function(e) {
+                Ms = {
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
+                js = Ms,
+                bs = !1,
+                ws = !0,
+                xs = {
+                    Now: function() {
+                        return new Date
+                    },
+                    Format: function(e) {
+                        return uo.FormatDateTime(e, bs, ws, true)
+                    },
+                    Format24: function(e) {
+                        return uo.FormatDateTime(e, bs, ws, true)
+                    },
+                    Format12: function(e) {
+                        return uo.FormatDateTime(e, bs, ws, false)
+                    },
+                    FormatVerbose: function(e) {
+                        return uo.FormatDateTime(e, true, ws, false)
+                    },
+                    Live: js.FormatDateTime
+                },
+                Ns = function(e) {
                     var t = e.columns,
                         n = e.list,
                         r = e.update,
                         o = e.refresh,
                         i = e.sort,
                         a = void 0 === i ? null : i,
                         s = e.state,
@@ -49863,15 +49942,15 @@
                                     },
                                     colSpan: "6"
                                 })
                             })]
                         }), M]
                     })
                 },
-                js = function(e) {
+                Is = function(e) {
                     var n = je().environ,
                         r = Ua(rn.Url("/aws/s3/buckets", n), {
                             initial: []
                         }),
                         o = Ua({
                             initial: []
                         }),
@@ -50079,15 +50158,15 @@
                                             style: {
                                                 height: "1px",
                                                 background: ln.GetForegroundColor(),
                                                 marginBottom: "1pt"
                                             }
                                         }), (0, wo.jsxs)("table", {
                                             width: "100%",
-                                            children: [(0, wo.jsxs)(Ms, {
+                                            children: [(0, wo.jsxs)(Ns, {
                                                 columns: [{
                                                     label: "Key",
                                                     key: "key"
                                                 }, {
                                                     label: "Size",
                                                     key: "size",
                                                     align: "right"
@@ -50153,15 +50232,15 @@
                                                             }), (0, wo.jsxs)("td", {
                                                                 align: "right",
                                                                 children: [e.size, "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     whiteSpace: "nowrap"
                                                                 },
-                                                                children: [e.modified, "\xa0\xa0"]
+                                                                children: [xs.Format(e.modified), "\xa0\xa0"]
                                                             })]
                                                         }, n), n < r.keys.length - 1 && (0, wo.jsxs)(wo.Fragment, {
                                                             children: [(0, wo.jsx)("tr", {
                                                                 children: (0, wo.jsx)("td", {
                                                                     style: {
                                                                         paddingTop: "4pt"
                                                                     }
@@ -50351,26 +50430,26 @@
                                         })]
                                     })
                                 })
                             })
                         })
                     })
                 },
-                bs = Da((function() {
+                Ds = Da((function() {
                     return Bt.IsReadOnlyMode()
                 })),
-                ws = function() {
-                    var e = l(La(bs), 2),
+                Ls = function() {
+                    var e = l(La(Ds), 2),
                         t = e[0],
                         n = e[1];
                     return [t, function(e) {
                         n(e), Bt.SetReadOnlyMode(e)
                     }]
                 },
-                xs = function() {
+                Ss = function() {
                     var e, t = null === (e = Ua("/checks_validation").data) || void 0 === e ? void 0 : e.actions_with_no_associated_check;
                     return t ? (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsxs)("div", {
                             className: "box error thickborder",
                             style: {
                                 width: "60%",
                                 fontSize: "small"
@@ -50395,95 +50474,16 @@
                                         })
                                     }), (0, wo.jsx)("br", {})]
                                 })
                             }))]
                         }), (0, wo.jsx)("br", {})]
                     }) : (0, wo.jsx)(wo.Fragment, {})
                 },
-                Ns = {
-                    Format: uo.FormatDate
-                },
-                Is = {
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
-                Ds = Is,
-                Ls = !1,
-                Ss = !0,
                 ks = {
-                    Now: function() {
-                        return new Date
-                    },
-                    Format: function(e) {
-                        return uo.FormatDateTime(e, Ls, Ss, true)
-                    },
-                    Format24: function(e) {
-                        return uo.FormatDateTime(e, Ls, Ss, true)
-                    },
-                    Format12: function(e) {
-                        return uo.FormatDateTime(e, Ls, Ss, false)
-                    },
-                    FormatVerbose: function(e) {
-                        return uo.FormatDateTime(e, true, Ss, false)
-                    },
-                    Live: Ds.FormatDateTime
+                    Format: uo.FormatDate
                 },
                 Cs = function(e) {
                     var t, n = e.status;
                     return function(e) {
                         return "ok" == e || "done" == e || e.includes("pass") || e.includes("success")
                     }(n = (null === (t = n) || void 0 === t ? void 0 : t.toLowerCase(n).trim()) || "") ? (0, wo.jsx)("b", {
                         style: {
@@ -50518,15 +50518,15 @@
                         children: n
                     })
                 },
                 Es = {
                     Ago: uo.Ago,
                     Format: uo.FormatDuration,
                     FromNow: uo.FromNow,
-                    Live: Ds.FormatDuration
+                    Live: js.FormatDuration
                 };
 
             function Ts(e) {
                 e.update()
             }
 
             function As(e) {
@@ -51220,15 +51220,15 @@
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
                                         children: i.__result.get("timestamp")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result ".concat(i.name),
                                         text: "Click to " + (i.__showingResultDetails ? "hide" : "show") + " latest result."
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-latest-result-timestamp ".concat(i.name),
-                                        text: Es.Format(i.__result.get("timestamp"), ks.Now(), !0, null, null, "ago")
+                                        text: Es.Format(i.__result.get("timestamp"), xs.Now(), !0, null, null, "ago")
                                     })]
                                 }), i.__showingResultDetails && (0, wo.jsx)(wo.Fragment, {
                                     children: i.__result.get("uuid") ? (0, wo.jsx)(wo.Fragment, {
                                         children: d ? (0, wo.jsx)(wo.Fragment, {
                                             children: i.__result.get("action") ? (0, wo.jsxs)(wo.Fragment, {
                                                 children: ["\xa0|\xa0", (0, wo.jsx)("span", {
                                                     id: "tooltip-view-latest-result-summary ".concat(i.name),
@@ -51651,15 +51651,15 @@
                 },
                 tu = function(e) {
                     var t = e.check,
                         n = e.env,
                         r = e.groupList,
                         o = e.historyList,
                         i = e.style,
-                        a = l(ws(), 1)[0],
+                        a = l(Ls(), 1)[0],
                         s = hs();
                     if (t.__queueingCheckRun) return t.__queueingCheckRun && (0, wo.jsxs)("div", {
                         className: "check-run-wait-button",
                         style: i,
                         children: [(0, wo.jsx)("span", {
                             id: "tooltip-queueing",
                             children: (0, wo.jsx)("i", {
@@ -51972,15 +51972,15 @@
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: ks.Format(n.__queuedCheckRun + "+00:00")
+                                        children: xs.Format(n.__queuedCheckRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this check run.",
@@ -52079,15 +52079,15 @@
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         onClick: function() {
                                             return s(!a)
                                         },
                                         style: {
                                             cursor: "pointer"
                                         },
-                                        children: ks.Format(n.__queuedActionRun + "+00:00")
+                                        children: xs.Format(n.__queuedActionRun + "+00:00")
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-1 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
                                         position: "bottom"
                                     }), (0, wo.jsx)(oa, {
                                         id: "tooltip-view-run-action-uuid-2 ".concat(n.name),
                                         text: "Click to " + (a ? "hide" : "show") + " UUID for this action run.",
@@ -52336,15 +52336,15 @@
                             }
                         }), i.__showingHistory && (0, wo.jsx)(wo.Fragment, {
                             children: (null === (n = i.__resultHistory) || void 0 === n || null === (r = n.data) || void 0 === r || null === (o = r.list) || void 0 === o ? void 0 : o.length) > 0 ? (0, wo.jsx)(wo.Fragment, {
                                 children: (0, wo.jsxs)("table", {
                                     style: {
                                         width: "100%"
                                     },
-                                    children: [(0, wo.jsx)(Ms, {
+                                    children: [(0, wo.jsx)(Ns, {
                                         loading: i.__resultHistory.loading,
                                         columns: h,
                                         list: i.__resultHistory.data.list,
                                         refresh: y,
                                         update: function(e) {
                                             return a.update()
                                         },
@@ -52400,15 +52400,15 @@
                                                                 id: "tooltip-history-timestamp-".concat(i.name, "-").concat(n),
                                                                 onClick: function() {
                                                                     u(i, e, l(e), a)
                                                                 },
                                                                 style: {
                                                                     cursor: "pointer"
                                                                 },
-                                                                children: ks.Format(d(e))
+                                                                children: xs.Format(d(e))
                                                             }), (0, wo.jsx)(oa, {
                                                                 id: "tooltip-history-timestamp-".concat(i.name, "-").concat(n),
                                                                 text: uo.Ago(d(e)),
                                                                 position: "right",
                                                                 shape: "squared"
                                                             }), "\xa0\xa0"]
                                                         }), (0, wo.jsxs)("td", {
@@ -52843,15 +52843,15 @@
                         o = e.env,
                         i = e.groupList,
                         a = e.fetchResult,
                         s = e.runActionAllowedState,
                         u = l((0, t.useState)(!1), 2),
                         c = u[0],
                         d = u[1],
-                        p = l(ws(), 1)[0],
+                        p = l(Ls(), 1)[0],
                         f = hs();
 
                     function h() {
                         if (c) {
                             var e;
                             d(!1);
                             var t = null === (e = r.__result) || void 0 === e ? void 0 : e.get("action");
@@ -53448,15 +53448,15 @@
                                             onClick: O,
                                             children: po.X
                                         }), (0, wo.jsxs)("table", {
                                             style: {
                                                 width: "100%"
                                             },
                                             border: "0",
-                                            children: [(0, wo.jsx)(Ms, {
+                                            children: [(0, wo.jsx)(Ns, {
                                                 columns: [{
                                                     label: "__refresh"
                                                 }, {
                                                     label: "Timestamp",
                                                     key: "timestamp"
                                                 }, {
                                                     label: "Check",
@@ -53533,19 +53533,19 @@
                                                                     children: po.X
                                                                 }), "\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 id: "recent-runs-timestamp ".concat(i),
                                                                 style: {
                                                                     width: "20%"
                                                                 },
-                                                                children: [Ns.Format(e.timestamp), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                                                children: [ks.Format(e.timestamp), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                                     children: uo.Format(e.timestamp)
                                                                 }), (0, wo.jsx)(oa, {
                                                                     id: "recent-runs-timestamp ".concat(i),
-                                                                    text: Es.Format(e.timestamp, ks.Now(), !0, null, null, "agoy")
+                                                                    text: Es.Format(e.timestamp, xs.Now(), !0, null, null, "agoy")
                                                                 }), "\xa0\xa0"]
                                                             }), (0, wo.jsxs)("td", {
                                                                 style: {
                                                                     width: "45%"
                                                                 },
                                                                 children: [(0, wo.jsx)("b", {
                                                                     style: {
@@ -53914,15 +53914,15 @@
                                                 children: [(0, wo.jsx)("td", {
                                                     style: c,
                                                     children: "Updated:"
                                                 }), (0, wo.jsx)("td", {
                                                     style: l,
                                                     children: (0, wo.jsx)("span", {
                                                         id: "tooltip-lambda-updated-".concat(u.lambda_name),
-                                                        children: ks.Format(u.lambda_modified)
+                                                        children: xs.Format(u.lambda_modified)
                                                     })
                                                 }), (0, wo.jsx)(oa, {
                                                     id: "tooltip-lambda-updated-".concat(u.lambda_name),
                                                     text: uo.Ago(u.lambda_modified),
                                                     position: "right",
                                                     shape: "squared"
                                                 })]
@@ -54073,15 +54073,15 @@
                             children: (0, wo.jsx)(xo, {
                                 loading: c.loading,
                                 color: ln.GetForegroundColor(),
                                 size: 90
                             })
                         })
                     }) : (0, wo.jsxs)(wo.Fragment, {
-                        children: [(0, wo.jsx)(xs, {}), (0, wo.jsx)("div", {
+                        children: [(0, wo.jsx)(Ss, {}), (0, wo.jsx)("div", {
                             children: (0, wo.jsx)("table", {
                                 children: (0, wo.jsx)("tbody", {
                                     children: (0, wo.jsxs)("tr", {
                                         children: [(0, wo.jsxs)("td", {
                                             style: {
                                                 paddingLeft: "4pt",
                                                 verticalAlign: "top"
@@ -55558,15 +55558,15 @@
                                 }
                             }), (null === (r = o.get("list")) || void 0 === r ? void 0 : r.length) > 0 ? (0, wo.jsx)(wo.Fragment, {
                                 children: (0, wo.jsxs)("table", {
                                     style: {
                                         width: "100%"
                                     },
                                     className: "fg",
-                                    children: [(0, wo.jsx)(Ms, {
+                                    children: [(0, wo.jsx)(Ns, {
                                         columns: p,
                                         list: o.get("list"),
                                         state: {
                                             key: u,
                                             order: m.endsWith(".desc") ? -1 : 1
                                         },
                                         update: function(e, t) {
@@ -55639,15 +55639,15 @@
                                                             id: "tooltip-timestamp-".concat(n),
                                                             onClick: function() {
                                                                 return E(i, e, a(e))
                                                             },
                                                             style: {
                                                                 cursor: "pointer"
                                                             },
-                                                            children: u(e)
+                                                            children: xs.Format(u(e))
                                                         }), (0, wo.jsx)(oa, {
                                                             id: "tooltip-timestamp-".concat(n),
                                                             text: uo.Ago(u(e)),
                                                             position: "right",
                                                             shape: "squared"
                                                         }), "\xa0\xa0"]
                                                     }), (0, wo.jsxs)("td", {
@@ -56380,15 +56380,15 @@
                                     }), " page."]
                                 })]
                             })
                         })
                     })
                 },
                 ku = function() {
-                    var e = l(ws(), 2),
+                    var e = l(Ls(), 2),
                         t = e[0],
                         n = e[1];
                     return (0, wo.jsxs)(wo.Fragment, {
                         children: [(0, wo.jsx)("img", {
                             id: "tooltip-readonly",
                             alt: "lock",
                             src: t ? on.Lock() : on.Unlock(),
@@ -56970,15 +56970,15 @@
                                                 style: {
                                                     paddingRight: "10pt",
                                                     whiteSpace: "nowrap",
                                                     color: "#D6EAF8"
                                                 },
                                                 align: "right",
                                                 children: [(0, wo.jsx)("small", {
-                                                    children: (0, wo.jsx)(ks.Live, {
+                                                    children: (0, wo.jsx)(xs.Live, {
                                                         verbose: !0,
                                                         timezone: !1
                                                     })
                                                 }), (null === (c = k.app) || void 0 === c || null === (d = c.credentials) || void 0 === d ? void 0 : d.aws_account_name) && (0, wo.jsxs)(wo.Fragment, {
                                                     children: ["\xa0|\xa0", (0, wo.jsx)(qe, {
                                                         id: "tooltip-header-account",
                                                         to: $r.Path("/login"),
@@ -58489,15 +58489,15 @@
                             }), (0, wo.jsx)(Bu, {
                                 name: "Size",
                                 value: te.get("app.lambda.lambda_code_size"),
                                 monospace: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "Modified",
-                                value: ks.Format(te.get("app.lambda.lambda_modified")),
+                                value: xs.Format(te.get("app.lambda.lambda_modified")),
                                 monospace: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "Role",
                                 value: te.get("app.lambda.lambda_role"),
                                 monospace: !0,
                                 size: "2"
@@ -58562,15 +58562,15 @@
                             }), (0, wo.jsx)(oa, {
                                 id: "tooltip-info-clear",
                                 position: "bottom",
                                 size: "small",
                                 text: "Click to clear any server-side caches."
                             }), (0, wo.jsx)(Bu, {
                                 name: "App Deployed At",
-                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : (null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
+                                value: rn.IsLocal() ? "running locally" + (ft.IsLocalCrossOrigin() ? " (cross-origin)" : "") : xs.Format(null === (B = ee.app) || void 0 === B ? void 0 : B.deployed) + Es.Format(null === (Y = ee.app) || void 0 === Y ? void 0 : Y.deployed, new Date, !0, "just now", "|", "ago"),
                                 monospace: !0,
                                 copy: !0,
                                 optional: !0,
                                 size: "2"
                             }), (0, wo.jsx)(Bu, {
                                 name: "App Launched At",
                                 value: (null === (Q = ee.app) || void 0 === Q ? void 0 : Q.launched) + Es.Format(null === (G = ee.app) || void 0 === G ? void 0 : G.launched, new Date, !0, "just now", "|", "ago"),
@@ -69152,21 +69152,21 @@
                             map: function(e) {
                                 return t.statusTitle(e)
                             }
                         }, {
                             label: "Created",
                             name: "created",
                             map: function(e) {
-                                return ks.Format(e)
+                                return xs.Format(e)
                             }
                         }, {
                             label: "Updated",
                             name: "updated",
                             map: function(e) {
-                                return ks.Format(e)
+                                return xs.Format(e)
                             }
                         }, {
                             label: "UUID",
                             name: "uuid"
                         }];
                     return tn.IsFoursightFourfront(Fa()) && (n = n.filter((function(e) {
                         return "institution" !== e.name && "project" !== e.name && "roles" !== e.name && "role" !== e.name
@@ -70012,27 +70012,27 @@
                     var e = je().uuid,
                         n = l(Qf.useUserInputs(), 2),
                         r = n[0],
                         o = n[1],
                         i = l((0, t.useState)(!1), 2),
                         a = i[0],
                         s = i[1],
-                        u = l(ws(), 1)[0],
+                        u = l(Ls(), 1)[0],
                         d = Ua({
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
-                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = ks.Format(e.created) : "updated" === i.name ? i.value = ks.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
+                                            } : "institution" === i.name ? i.value = e.institution : "status" === i.name ? i.value = e.status : "created" === i.name ? i.value = xs.Format(e.created) : "updated" === i.name ? i.value = xs.Format(e.updated) : "uuid" === i.name && (i.value = e.uuid)
                                         }
                                     } catch (a) {
                                         r.e(a)
                                     } finally {
                                         r.f()
                                     }
                                     return p(t)
@@ -70310,15 +70310,15 @@
                                 marginTop: "4pt",
                                 paddingTop: "8pt"
                             },
                             children: (0, wo.jsxs)("table", {
                                 style: {
                                     width: "100%"
                                 },
-                                children: [(0, wo.jsx)(Ms, {
+                                children: [(0, wo.jsx)(Ns, {
                                     columns: r,
                                     sort: M,
                                     list: null === o || void 0 === o || null === (n = o.data) || void 0 === n ? void 0 : n.list,
                                     update: function(e, t) {
                                         j("".concat(e, ".").concat(t))
                                     },
                                     bottomline: !0,
@@ -70596,22 +70596,22 @@
                                                 size: "small",
                                                 text: "Status: ".concat(e.status)
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: nt(nt({}, g), {}, {
                                                 whiteSpace: "nowrap"
                                             }),
-                                            children: [e.updated ? Ns.Format(e.updated) : Ns.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                            children: [e.updated ? ks.Format(e.updated) : ks.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                 children: e.updated ? uo.Format(e.updated) : uo.Format(e.created)
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: nt(nt({}, g), {}, {
                                                 whiteSpace: "nowrap"
                                             }),
-                                            children: [Ns.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
+                                            children: [ks.Format(e.created), " ", (0, wo.jsx)("br", {}), (0, wo.jsx)("small", {
                                                 children: uo.Format(e.created)
                                             })]
                                         }), (0, wo.jsxs)("td", {
                                             style: nt(nt({}, g), {}, {
                                                 whiteSpace: "nowrap"
                                             }),
                                             children: ["\xa0\xa0", (0, wo.jsx)("button", {
@@ -70732,15 +70732,15 @@
                                         path: "/api/react/:environ/gac/:environCompare",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
                                             children: (0, wo.jsx)(sf, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/aws/s3",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
-                                            children: (0, wo.jsx)(js, {})
+                                            children: (0, wo.jsx)(Is, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
                                         path: "/api/react/:environ/aws/infrastructure",
                                         element: (0, wo.jsx)(wa.AuthorizationRequired, {
                                             children: (0, wo.jsx)(Of, {})
                                         })
                                     }), (0, wo.jsx)(Oe, {
```

### Comparing `foursight_core-4.3.0.2b4/foursight_core/route_prefixes.py` & `foursight_core-4.3.0.2b5/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/routes.py` & `foursight_core-4.3.0.2b5/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/run_result.py` & `foursight_core-4.3.0.2b5/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/s3_connection.py` & `foursight_core-4.3.0.2b5/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/schedule_decorator.py` & `foursight_core-4.3.0.2b5/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/sqs_utils.py` & `foursight_core-4.3.0.2b5/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/stage.py` & `foursight_core-4.3.0.2b5/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/base.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/header.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/history.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/info.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/unused.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/user.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/users.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/view_checks.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/foursight_core/templates/view_groups.html` & `foursight_core-4.3.0.2b5/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.3.0.2b4/pyproject.toml` & `foursight_core-4.3.0.2b5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.3.0.2b4"  # TODO: To become 4.4.0
+version = "4.3.0.2b5"  # TODO: To become 4.4.0
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
```

### Comparing `foursight_core-4.3.0.2b4/PKG-INFO` & `foursight_core-4.3.0.2b5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.3.0.2b4
+Version: 4.3.0.2b5
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

