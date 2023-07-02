# Comparing `tmp/port_ocean-0.1.0.dev3.tar.gz` & `tmp/port_ocean-0.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev3.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0.dev4.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev3.tar` & `port_ocean-0.1.0.dev4.tar`

### file list

```diff
@@ -1,67 +1,73 @@
--rw-r--r--   0        0        0     3218 2023-06-29 12:30:35.401267 port_ocean-0.1.0.dev3/README.md
--rw-r--r--   0        0        0      440 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     3385 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       54 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0      598 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1718 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      406 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0      392 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1184 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1334 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      766 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0    10983 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0      593 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2592 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/config/base.py
--rw-r--r--   0        0        0     1035 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3825 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     1896 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/context/event.py
--rw-r--r--   0        0        0     4017 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/base.py
--rw-r--r--   0        0        0      300 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0      690 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     2521 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      452 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1432 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      914 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1173 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/get_required_entities.py
--rw-r--r--   0        0        0     1043 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     4656 2023-06-29 12:30:35.453268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1495 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     3593 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2393 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     7023 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      448 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/base.py
--rw-r--r--   0        0        0     2616 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/factory.py
--rw-r--r--   0        0        0      817 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/http.py
--rw-r--r--   0        0        0     3229 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/kafka.py
--rw-r--r--   0        0        0      909 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/settings.py
--rw-r--r--   0        0        0      563 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/types.py
--rw-r--r--   0        0        0     1957 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/core/utils.py
--rw-r--r--   0        0        0      166 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/errors.py
--rw-r--r--   0        0        0      534 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2064 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4269 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/port_ocean/port_ocean.py
--rw-r--r--   0        0        0     1938 2023-06-29 12:30:35.457268 port_ocean-0.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     4247 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     4337 2023-07-02 12:33:49.649332 port_ocean-0.1.0.dev4/README.md
+-rw-r--r--   0        0        0      440 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     3380 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       54 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0      449 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1718 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      406 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0      392 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1184 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      766 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0    11337 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0      593 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1035 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     3821 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3234 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4012 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/base.py
+-rw-r--r--   0        0        0      300 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/__init__.py
+-rw-r--r--   0        0        0      690 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/base.py
+-rw-r--r--   0        0        0     2629 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/jq_manipulation.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1432 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/__init__.py
+-rw-r--r--   0        0        0      914 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/base.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/__init__.py
+-rw-r--r--   0        0        0     1258 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/get_required_entities.py
+-rw-r--r--   0        0        0     1043 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     5115 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/transport.py
+-rw-r--r--   0        0        0     1495 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     3734 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2556 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0     7748 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/models.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/base.py
+-rw-r--r--   0        0        0     2840 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/factory.py
+-rw-r--r--   0        0        0      898 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/http.py
+-rw-r--r--   0        0        0     3303 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/kafka.py
+-rw-r--r--   0        0        0      909 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/settings.py
+-rw-r--r--   0        0        0      563 2023-07-02 12:33:49.697333 port_ocean-0.1.0.dev4/port_ocean/core/types.py
+-rw-r--r--   0        0        0     2044 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/core/utils.py
+-rw-r--r--   0        0        0      166 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/errors.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/api/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/api/base.py
+-rw-r--r--   0        0        0      461 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      626 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2429 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4246 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/ocean.py
+-rw-r--r--   0        0        0      765 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/port_ocean/utils.py
+-rw-r--r--   0        0        0     1938 2023-07-02 12:33:49.701333 port_ocean-0.1.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev4/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev3/README.md` & `port_ocean-0.1.0.dev4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 <img align="right" width="100" height="74" src="https://user-images.githubusercontent.com/8277210/183290025-d7b24277-dfb4-4ce1-bece-7fe0ecd5efd4.svg" />
 
-# Integration Framework
+# Ocean
+[![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
-Integration Framework is a solution developed by Port to address the challenges faced while integrating various third-party systems with our developer portal product. This framework provides a standardized approach for implementing integrations, simplifying the process and allowing platform engineers to focus on the core functionality of the third-party system.
+Ocean is a solution developed by Port to address the challenges faced while integrating various third-party systems with our developer portal product. This framework provides a standardized approach for implementing integrations, simplifying the process and allowing platform engineers to focus on the core functionality of the third-party system.
+
+## Installation
+`pip install port-ocean[cli]` or `poetry add port-ocean[cli]`
+
+## Run Integration
+1. source the integration venv `. .venv/bin/activate`
+2. `ocean sail ./path/to/integration`
+
+## Local Development (Framework)
+1. Clone the repository
+2. Install dependencies: `make install` or `make install/all` for installing integrations dependencies as well
+3. source the integration venv `. .venv/bin/activate`
+
+
+## Local Development (Integration)
+1. Clone the repository
+2. For new integration run `make new` and follow the instructions
+3. Install dependencies: `cd DESIRED_INTEGRATION_FOLDER && make install`
+4. source the integration venv `. .venv/bin/activate`
+5. Run integration: `make run`
  
 ## Export Architecture
 ![image](./assets/IntegrationFrameworkExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/IntergationFrameworkRealTimeUpdatesArchitecture.svg)
 
 ## Self Service Architecture
 ![image](./assets/IntegrationFrameworkSelfServiceArchitecture.svg)
 
 ## Folder Structure
 The Integration Framework follows a specific folder structure within the mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
-integration-framework/
-├── framework/
-│ ├── main.py
-│ └── requirements.txt
+port-ocean/
+├── port_ocean (framework)/
+│ ├── ocean.py
+│ ├── core/
 | └── ...
 └── integrations/
-├────integration_name/
-│ ├──── main.py
-│ └──── requirements.txt
+│  ├───integration_name/
+│  ├──── main.py
+│  ├──── pyproject.toml
+│  └──── Dockerfile
 ├── ...
 └── ...
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
@@ -40,28 +62,34 @@
 ![image](./assets/IntegrationFrameworkLifecycleOfIntegration.svg)
 
 ## Configuration
 The Integration Framework utilizes a `config.yaml` file for configuration. This file specifies the integrations to be used within an array. Each integration has a unique identifier and type, which are used during initialization to update Port accordingly.
 
 Example `config.yaml`:
 ```yaml
+# This is an example configuration file for the integration service.
+# Please copy this file to config.yaml file in the integration folder and edit it to your needs.
+
 port:
   clientId: PORT_CLIENT_ID # Can be loaded via environment variable: PORT_CLIENT_ID
   clientSecret: PORT_CLIENT_SECRET # Can be loaded via environment variable: PORT_CLIENT_SECRET
   baseUrl: https://api.getport.io/v1
-triggerChannel: 
+# The trigger channel to use for the integration service.
+triggerChannel:
   type: KAFKA
-integrations:
+  brokers: "localhost:9092"
+  kafkaSecurityEnabled: false
+integration:
   # The name of the integration.
-  - identifier: "my_kafka_integration"
-    # The type of the integration.
-    type: "kafka"
-    # The configuration of the integration.
-    config:
-      bootstrap_servers: "localhost:9092"
+  identifier: "my_integration"
+  # The type of the integration.
+  type: "Git"
+  config:
+    my_git_token: "random"
+    some_other_integration_config: "Very important information"
 ```
 
 ## Contributing
 We welcome contributions to the Integration Framework project. If you have any suggestions, bug reports, or would like to contribute new features, please follow our guidelines outlined in the `CONTRIBUTING.md` file.
 
 ## License
 The Integration Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the `LICENSE` file for more details.
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/cli/commands.py` & `port_ocean-0.1.0.dev4/port_ocean/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # Ocean root command
     pass
 
 
 @cli_start.command()
 @click.argument("path", default="")
 def sail(path: str) -> None:
-    from port_ocean.port_ocean import run
+    from port_ocean.ocean import run
 
     print_logo()
 
     print("Setting sail... ⛵️⚓️⛵️⚓️ All hands on deck! ⚓️")
     run(path)
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/cli/download_git_folder.py` & `port_ocean-0.1.0.dev4/port_ocean/cli/download_git_folder.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0.dev4/port_ocean/cli/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/clients/port/client.py` & `port_ocean-0.1.0.dev4/port_ocean/clients/port/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from port_ocean.clients.port.types import (
     KafkaCreds,
     RequestOptions,
     UserAgentType,
 )
 from port_ocean.core.models import Entity, Blueprint
+from port_ocean.exceptions.clients import KafkaCredentialsNotFound
 
 
 class TokenResponse(BaseModel):
     access_token: str = Field(alias="accessToken")
     expires_in: int = Field(alias="expiresIn")
     token_type: str = Field(alias="tokenType")
     _retrieved_time: datetime = PrivateAttr(datetime.now())
@@ -112,24 +113,30 @@
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
                 f"error: {response.text}"
             )
         response.raise_for_status()
 
     async def delete_entity(
-        self, entity: Entity, user_agent_type: UserAgentType | None = None
+        self,
+        entity: Entity,
+        request_options: RequestOptions,
+        user_agent_type: UserAgentType | None = None,
     ) -> None:
         logger.info(
             f"Delete entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         async with httpx.AsyncClient() as client:
             response = await client.delete(
                 f"{self.api_url}/blueprints/{entity.blueprint}/entities/{entity.identifier}",
                 headers=await self._headers(user_agent_type),
-                params={"delete_dependents": "true"},
+                params={
+                    "delete_dependents": request_options["delete_dependent_entities"]
+                    or False
+                },
             )
 
         if not response.status_code < 400:
             logger.error(
                 f"Error deleting "
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
@@ -146,15 +153,15 @@
         if not response.status_code < 400:
             logger.error(f"Error getting kafka credentials, error: {response.text}")
             response.raise_for_status()
 
         credentials = response.json()["credentials"]
 
         if credentials is None:
-            raise Exception("No kafka credentials found")
+            raise KafkaCredentialsNotFound("No kafka credentials found")
 
         return credentials
 
     async def get_org_id(self) -> str:
         logger.info("Fetching organization id")
 
         async with httpx.AsyncClient() as client:
@@ -192,43 +199,42 @@
                     "property": "$datasource",
                     "operator": "=",
                     "value": self._user_agent(user_agent_type),
                 },
             ],
         }
 
+        logger.info(f"Searching entities with query {query}")
         async with httpx.AsyncClient() as client:
             search_req = await client.post(
                 f"{self.api_url}/entities/search",
                 json=query,
                 headers=await self._headers(),
                 params={
                     "exclude_calculated_properties": "true",
                     "include": ["blueprint", "identifier"],
                 },
             )
-            search_req.raise_for_status()
-            return [
-                Entity.parse_obj(result) for result in search_req.json()["entities"]
-            ]
+        search_req.raise_for_status()
+        return [Entity.parse_obj(result) for result in search_req.json()["entities"]]
 
     async def search_dependent_entities(self, entity: Entity) -> list[Entity]:
         body = {
             "combinator": "and",
             "rules": [
                 {
                     "operator": "relatedTo",
                     "blueprint": entity.blueprint,
                     "value": entity.identifier,
                     "direction": "downstream",
                 }
             ],
         }
 
-        logger.info(f"Search dependent entity with body {body}")
+        logger.info(f"Searching dependent entity with body {body}")
         async with httpx.AsyncClient() as client:
             response = await client.post(
                 f"{self.api_url}/entities/search",
                 headers=await self._headers(),
                 json=body,
             )
         response.raise_for_status()
@@ -273,14 +279,15 @@
         async with httpx.AsyncClient() as client:
             installation = await client.patch(
                 f"{self.api_url}/integration/{_id}",
                 headers=headers,
                 json=json,
             )
             if installation.status_code == 404:
+                logger.info(f"Integration with id: {_id} not found, creating it")
                 installation = await client.post(
                     f"{self.api_url}/integration", headers=headers, json=json
                 )
 
         if installation.status_code >= 400:
             logger.error(
                 f"Error initiating integration with id: {_id}, error: {installation.text}"
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/clients/port/types.py` & `port_ocean-0.1.0.dev4/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/config/base.py` & `port_ocean-0.1.0.dev4/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/config/integration.py` & `port_ocean-0.1.0.dev4/port_ocean/config/integration.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0.dev4/port_ocean/consumers/kafka_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         message = json.loads(raw_msg.value().decode())
         topic = raw_msg.topic()
 
         async def try_wrapper() -> None:
             try:
                 await self.msg_process(message, topic)
             except Exception as e:
-                logger.exception(f"Failed to process message: {str(e)}")
+                logger.error(f"Failed to process message: {str(e)}")
 
         asyncio.run(try_wrapper())
 
     def start(self) -> None:
         try:
             logger.info("Start consumer...")
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/context/ocean.py` & `port_ocean-0.1.0.dev4/port_ocean/context/ocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     START_EVENT_LISTENER,
     RawEntityDiff,
 )
 from port_ocean.errors import PortOceanContextNotFoundError
 
 if TYPE_CHECKING:
     from port_ocean.core.integrations.base import BaseIntegration
-    from port_ocean.port_ocean import Ocean
+    from port_ocean.ocean import Ocean
 
 
 @dataclass
 class PortOceanContext:
     app: "Ocean"
 
     @property
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/base.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/manipulation/jq_manipulation.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/manipulation/jq_manipulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import lru_cache
 from typing import Any
 
 import pyjq as jq  # type: ignore
-
 from port_ocean.core.handlers.manipulation.base import BaseManipulation
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff
+from port_ocean.exceptions.base import ManipulationHandlerException
 
 
 class JQManipulation(BaseManipulation):
     @lru_cache
     def _compile(self, pattern: str) -> Any:
         return jq.compile(pattern)
 
@@ -22,15 +22,17 @@
 
     def _search_as_bool(self, data: dict[str, Any], pattern: str) -> bool:
         value = self._compile(pattern).first(data)
 
         if isinstance(value, bool):
             return value
 
-        raise Exception(f"Expected boolean value, got {type(value)} instead")
+        raise ManipulationHandlerException(
+            f"Expected boolean value, got {type(value)} instead"
+        )
 
     def _search_as_object(
         self, data: dict[str, Any], obj: dict[str, Any]
     ) -> dict[str, Any | None]:
         result: dict[str, Any | None] = {}
         for key, value in obj.items():
             try:
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/base.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/transport.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 )
 from port_ocean.core.handlers.transport.port.validate_entity_relations import (
     validate_entity_relations,
 )
 from port_ocean.core.models import Entity
 from port_ocean.core.types import EntityDiff
 from port_ocean.core.utils import is_same_entity, get_unique, get_port_diff
+from port_ocean.exceptions.base import RelationValidationException
 
 
 class HttpPortTransport(BaseTransport):
     async def _validate_delete_dependent_entities(self, entities: list[Entity]) -> None:
         logger.info("Validated deleted entities")
         if not event.port_app_config.delete_dependent_entities:
             deps = await asyncio.gather(
@@ -33,89 +34,93 @@
                     entity
                     for entity in chain.from_iterable(deps)
                     if not any([is_same_entity(item, entity) for item in entities])
                 ]
             )
 
             if new_dependent:
-                raise Exception(
+                raise RelationValidationException(
                     f"Must enable delete_dependent_entities flag or delete also dependent entities:"
                     f" {[(dep.blueprint, dep.identifier) for dep in new_dependent]}"
                 )
 
     async def _validate_entity_diff(self, diff: EntityPortDiff) -> None:
         config = event.port_app_config
         await self._validate_delete_dependent_entities(diff.deleted)
         modified_or_created_entities = diff.modified + diff.created
-        logger.info("Validating modified or created entities")
 
-        await asyncio.gather(
-            *[
-                self.context.port_client.validate_entity_payload(
-                    entity,
-                    {
-                        "merge": config.enable_merge_entity,
-                        "create_missing_related_entities": config.create_missing_related_entities,
-                    },
-                )
-                for entity in modified_or_created_entities
-            ]
-        )
+        if modified_or_created_entities:
+            logger.info("Validating modified or created entities")
+
+            await asyncio.gather(
+                *[
+                    self.context.port_client.validate_entity_payload(
+                        entity,
+                        {
+                            "merge": config.enable_merge_entity,
+                            "create_missing_related_entities": config.create_missing_related_entities,
+                        },
+                    )
+                    for entity in modified_or_created_entities
+                ]
+            )
+        logger.info("Validating no relation blocks the operation")
         await validate_entity_relations(diff, self.context.port_client)
 
     async def update_diff(
         self,
         entities: EntityDiff,
         user_agent_type: UserAgentType | None = None,
     ) -> None:
         diff = get_port_diff(entities["before"], entities["after"])
 
         logger.info(
-            f"Registering entity diff (created: {len(diff.created)}, deleted: {len(diff.deleted)}, modified: {len(diff.modified)})"
+            f"Updating entity diff (created: {len(diff.created)}, deleted: {len(diff.deleted)}, modified: {len(diff.modified)})"
         )
         await self._validate_entity_diff(diff)
 
         user_agent_type = user_agent_type or self.DEFAULT_USER_AGENT_TYPE
         await self.delete(diff.deleted, user_agent_type)
+        logger.info("Upserting new entities")
         await self.upsert(diff.created, user_agent_type)
+        logger.info("Upserting modified entities")
         await self.upsert(diff.modified, user_agent_type)
 
     async def upsert(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
+        logger.info(f"Upserting {len(entities)} entities")
         ordered_created_entities = reversed(order_by_entities_dependencies(entities))
         for entity in ordered_created_entities:
             await self.context.port_client.upsert_entity(
                 entity,
                 event.port_app_config.get_port_request_options(),
                 user_agent_type,
             )
 
     async def delete(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
+        logger.info(f"Deleting {len(entities)} entities")
         ordered_deleted_entities = order_by_entities_dependencies(entities)
 
-        await asyncio.gather(
-            *[
-                self.context.port_client.delete_entity(entity, user_agent_type)
-                for entity in ordered_deleted_entities
-            ]
-        )
+        for entity in ordered_deleted_entities:
+            await self.context.port_client.delete_entity(
+                entity,
+                event.port_app_config.get_port_request_options(),
+                user_agent_type,
+            )
 
     async def delete_non_existing(
         self, excluded_entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
+        logger.info("Deleting entities that should no longer exists")
         entities_at_port = await self.context.port_client.search_entities(
             user_agent_type
         )
-        diff = get_port_diff(entities_at_port, excluded_entities)
-        await self._validate_entity_diff(diff)
-
-        ordered_deleted_entities = order_by_entities_dependencies(diff.deleted)
 
-        await asyncio.gather(
-            *[
-                self.context.port_client.delete_entity(entity, user_agent_type)
-                for entity in ordered_deleted_entities
-            ]
+        logger.info(
+            "Checking the diff between the state in the integration to the state in port"
         )
+        diff = get_port_diff(entities_at_port, excluded_entities)
+        await self._validate_entity_diff(diff)
+        await self.delete(diff.deleted, user_agent_type)
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0.dev4/port_ocean/core/handlers/transport/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0.dev4/port_ocean/core/integrations/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 import asyncio
 from typing import (
     Any,
 )
 
 from loguru import logger
+
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.context.event import (
     event_context,
     TriggerType,
 )
 from port_ocean.context.ocean import PortOceanContext
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.sync import SyncRawMixin, SyncMixin
 from port_ocean.core.models import Entity
 from port_ocean.core.trigger_channel.factory import (
     TriggerChannelFactory,
 )
+from port_ocean.exceptions.base import IntegrationAlreadyStartedException
 
 
 class BaseIntegration(SyncRawMixin, SyncMixin):
     def __init__(self, context: PortOceanContext):
         SyncRawMixin.__init__(self)
         SyncMixin.__init__(self)
         self.started = False
         self.context = context
         self.trigger_channel = TriggerChannelFactory(
             context,
             self.context.config.integration.identifier,
             {"on_action": self.trigger_action, "on_resync": self.sync_all},
         )
 
-    async def _sync_new_in_batches(
+    async def _register_in_batches(
         self, resource_config: ResourceConfig, user_agent_type: UserAgentType
     ) -> list[Entity]:
         resource, results = await self._get_resource_raw_results(resource_config)
 
         tasks = []
 
         batch_size = self.context.config.batch_work_size or len(results) or 1
         for batch in [
             results[i : i + batch_size] for i in range(0, len(results), batch_size)
         ]:
+            logger.info(f"Creating task for registering batch of {len(batch)} entities")
             tasks.append(self._register_resource_raw(resource, batch, user_agent_type))
         entities = await asyncio.gather(*tasks)
         return sum(entities, [])
 
     async def start(self) -> None:
         logger.info("Starting integration")
         if self.started:
-            raise Exception("Integration already started")
+            raise IntegrationAlreadyStartedException("Integration already started")
 
         if (
             not self.event_strategy["resync"]
             and self.__class__._on_resync == BaseIntegration._on_resync
         ):
             raise NotImplementedError("on_resync is not implemented")
 
@@ -87,17 +90,15 @@
         logger.info("Resync was triggered")
 
         async with event_context("resync", trigger_type=trigger_type):
             app_config = await self.port_app_config_handler.get_port_app_config()
 
             created_entities = await asyncio.gather(
                 *(
-                    self._sync_new_in_batches(resource, user_agent_type)
+                    self._register_in_batches(resource, user_agent_type)
                     for resource in app_config.resources
                 )
             )
 
             await self.transport.delete_non_existing(
                 sum(created_entities, []), user_agent_type
             )
-
-            logger.info("Resync was finished")
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Callable
 
 from loguru import logger
-
 from port_ocean.context.ocean import PortOceanContext, ocean
 from port_ocean.core.handlers import BaseManipulation, BasePortAppConfig, BaseTransport
 from port_ocean.core.handlers.manipulation.jq_manipulation import JQManipulation
 from port_ocean.core.handlers.port_app_config.api import APIPortAppConfig
 from port_ocean.core.handlers.transport.port.transport import HttpPortTransport
+from port_ocean.exceptions.base import IntegrationNotStartedException
 
 
 class HandlerMixin:
     ManipulationHandlerClass: Callable[
         [PortOceanContext], BaseManipulation
     ] = JQManipulation
 
@@ -26,27 +26,27 @@
         self._manipulation: BaseManipulation | None = None
         self._port_app_config_handler: BasePortAppConfig | None = None
         self._transport: BaseTransport | None = None
 
     @property
     def manipulation(self) -> BaseManipulation:
         if not self._manipulation:
-            raise Exception("Integration not started")
+            raise IntegrationNotStartedException("Manipulation class not initialized")
         return self._manipulation
 
     @property
     def port_app_config_handler(self) -> BasePortAppConfig:
         if self._port_app_config_handler is None:
-            raise Exception("Integration not started")
+            raise IntegrationNotStartedException("PortAppConfig class not initialized")
         return self._port_app_config_handler
 
     @property
     def transport(self) -> BaseTransport:
         if not self._transport:
-            raise Exception("Integration not started")
+            raise IntegrationNotStartedException("Transport class not initialized")
         return self._transport
 
     async def _init_manipulation_instance(self) -> BaseManipulation:
         self._manipulation = self.ManipulationHandlerClass(ocean)
         return self._manipulation
 
     async def _init_port_app_config_handler_instance(
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0.dev4/port_ocean/core/integrations/mixins/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.events import EventsMixin
 from port_ocean.core.integrations.mixins.handler import HandlerMixin
 from port_ocean.core.models import Entity
-from port_ocean.core.types import RawEntityDiff, EntityDiff
+from port_ocean.core.types import RawEntityDiff, EntityDiff, RESYNC_EVENT_LISTENER
 from port_ocean.core.utils import validate_result, zip_and_sum
+from port_ocean.exceptions.base import RawObjectValidationException
+from port_ocean.utils import get_function_location
 
 
 class SyncMixin(HandlerMixin, EventsMixin):
     def __init__(self) -> None:
         HandlerMixin.__init__(self)
         EventsMixin.__init__(self)
 
@@ -58,30 +60,45 @@
         return await asyncio.gather(
             *[
                 self.manipulation.parse_items(mapping, results)
                 for mapping, results in raw_diff
             ]
         )
 
+    async def _validate_raw_data_wrapper(
+        self, fn: RESYNC_EVENT_LISTENER, kind: str
+    ) -> Any:
+        results = await fn(kind)
+        try:
+            return validate_result(results)
+        except RawObjectValidationException as error:
+            raise RawObjectValidationException(
+                f"Failed to validate raw data for returned data from {get_function_location(fn)}, error: {error}"
+            ) from error
+
     async def _get_resource_raw_results(
         self, resource_config: ResourceConfig
     ) -> tuple[ResourceConfig, list[dict[Any, Any]]]:
-        logger.info(f"Resyncing {resource_config.kind}")
+        logger.info(f"Fetching {resource_config.kind} resync results")
         tasks: list[Awaitable[list[dict[Any, Any]]]] = []
         with logger.contextualize(kind=resource_config.kind):
             if self.__class__._on_resync != SyncRawMixin._on_resync:
                 tasks.append(self._on_resync(resource_config.kind))
 
             fns = [
                 *self.event_strategy["resync"][resource_config.kind],
                 *self.event_strategy["resync"][None],
             ]
 
-            for wrapper in fns:
-                tasks.append(wrapper(resource_config.kind))
+            for resync_function in fns:
+                tasks.append(
+                    self._validate_raw_data_wrapper(
+                        resync_function, resource_config.kind
+                    )
+                )
 
             logger.info(f"Found {len(tasks)} resync tasks for {resource_config.kind}")
             results: list[dict[Any, Any]] = list(
                 chain.from_iterable(
                     [
                         validate_result(task_result)
                         for task_result in await asyncio.gather(*tasks)
@@ -178,15 +195,15 @@
 
     async def update_raw_diff(
         self,
         kind: str,
         raw_desired_state: RawEntityDiff,
         user_agent_type: UserAgentType,
     ) -> None:
-        logger.info(f"Registering state for {kind}")
+        logger.info(f"Updating state for {kind}")
         config = await self.port_app_config_handler.get_port_app_config()
         resource_mappings = [
             resource for resource in config.resources if resource.kind == kind
         ]
 
         with logger.contextualize(kind=kind):
             logger.info(f"Found {len(resource_mappings)} resources for {kind}")
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/models.py` & `port_ocean-0.1.0.dev4/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/factory.py` & `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Callable, Any, Awaitable
 
+from loguru import logger
+
 from port_ocean.context.ocean import PortOceanContext
 from port_ocean.core.base import BaseWithContext
 from port_ocean.core.trigger_channel.base import (
     BaseTriggerChannel,
     TriggerChannelEvents,
 )
 from port_ocean.core.trigger_channel.http import (
@@ -12,14 +14,15 @@
 from port_ocean.core.trigger_channel.kafka import (
     KafkaTriggerChannel,
 )
 from port_ocean.core.trigger_channel.settings import (
     HttpTriggerChannelSettings,
     KafkaTriggerChannelSettings,
 )
+from port_ocean.exceptions.base import UnsupportedTriggerChannelException
 
 
 class TriggerChannelFactory(BaseWithContext):
     def __init__(
         self,
         context: PortOceanContext,
         installation_id: str,
@@ -47,14 +50,15 @@
         wrapped_events: TriggerChannelEvents = {
             "on_resync": self.on_event(self.events["on_resync"]),
             "on_action": self.on_event(self.events["on_action"]),
         }
         config = self.context.config.trigger_channel
         _type = config.type.lower()
         assert_message = "Invalid trigger channel config, expected KafkaTriggerChannelSettings and got {0}"
+        logger.info(f"Found trigger channel type: {_type}")
 
         match _type:
             case "kafka":
                 assert isinstance(
                     config, KafkaTriggerChannelSettings
                 ), assert_message.format(type(config))
                 org_id = await self.context.port_client.get_org_id()
@@ -67,10 +71,12 @@
             case "webhook":
                 assert isinstance(
                     config, HttpTriggerChannelSettings
                 ), assert_message.format(type(config))
                 self._trigger_channel = HttpTriggerChannel(wrapped_events, config)
 
             case _:
-                raise Exception(f"Trigger channel {_type} not supported")
+                raise UnsupportedTriggerChannelException(
+                    f"Trigger channel {_type} not supported"
+                )
 
         await self._trigger_channel.start()
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/http.py` & `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/http.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from fastapi import APIRouter
+from loguru import logger
 
 from port_ocean.context.ocean import ocean
 from port_ocean.core.trigger_channel.base import (
     BaseTriggerChannel,
     TriggerChannelEvents,
 )
 from port_ocean.core.trigger_channel.settings import HttpTriggerChannelSettings
@@ -14,14 +15,15 @@
         events: TriggerChannelEvents,
         trigger_channel_config: HttpTriggerChannelSettings,
     ):
         super().__init__(events)
         self.trigger_channel_config = trigger_channel_config
 
     async def start(self) -> None:
+        logger.info("Setting up HTTP trigger channel")
         target_channel_router = APIRouter()
 
         @target_channel_router.post("/resync")
         async def resync() -> None:
             await self.events["on_resync"]({})
 
         ocean.app.fast_api_app.include_router(target_channel_router)
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/kafka.py` & `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/kafka.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import threading
 from typing import Any, Callable
 
+from loguru import logger
+
 from port_ocean.consumers.kafka_consumer import KafkaConsumer, KafkaConsumerConfig
 from port_ocean.context.ocean import (
     PortOceanContext,
     initialize_port_ocean_context,
     ocean,
 )
 from port_ocean.core.trigger_channel.base import (
@@ -82,11 +84,12 @@
 
     async def start(self) -> None:
         consumer = KafkaConsumer(
             msg_process=self._handle_message,
             org_id=self.org_id,
             config=await self._get_kafka_creds(),
         )
+        logger.info("Starting Kafka consumer")
         threading.Thread(
             name="ocean_kafka_consumer",
             target=self.wrapped_start(ocean, consumer.start),
         ).start()
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/trigger_channel/settings.py` & `port_ocean-0.1.0.dev4/port_ocean/core/trigger_channel/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/types.py` & `port_ocean-0.1.0.dev4/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev3/port_ocean/core/utils.py` & `port_ocean-0.1.0.dev4/port_ocean/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Iterable, Any, TypeVar
 
 from port_ocean.core.handlers.manipulation.base import EntityPortDiff
 from port_ocean.core.models import Entity
+from port_ocean.exceptions.base import RawObjectValidationException
 
 
 def is_valid_diff_item(item: Any) -> bool:
     return isinstance(item, list) and all([isinstance(i, dict) for i in item] or [True])
 
 
 def validate_result(result: Any) -> list[dict[Any, Any]]:
     if isinstance(result, list):
         if is_valid_diff_item(result):
             return result
-    raise Exception(f"Expected dict, got {type(result)} instead")
+    raise RawObjectValidationException(f"Expected dict, got {type(result)} instead")
 
 
 def is_same_entity(firs_entity: Entity, second_entity: Entity) -> bool:
     return (
         firs_entity.identifier == second_entity.identifier
         and firs_entity.blueprint == second_entity.blueprint
     )
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/logger_setup.py` & `port_ocean-0.1.0.dev4/port_ocean/logger_setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
 
 from loguru import logger
 
 from port_ocean.config.integration import LoggerConfiguration
 
-settings = LoggerConfiguration()
 
-LoggerFormat = (
-    "<green>{time:YY-MM-DD HH:mm:ss.SSS}</green> | "
-    "<level>{level: <8}</level> | "
-    "<level>{message}</level> | {extra}"
-)
+def setup_logger() -> None:
+    settings = LoggerConfiguration()
+    logger_format = (
+        "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
+        "<level>{level: <8}</level> | "
+        "<level>{message}</level> | {extra}"
+    )
 
-logger.remove()
-logger.add(
-    sys.stderr,
-    level=settings.level.upper(),
-    format=LoggerFormat,
-    serialize=settings.serialize,
-    enqueue=True,  # process logs in background
-    diagnose=False,  # hide variable values in log backtrace
-)
+    logger.remove()
+    logger.add(
+        sys.stderr,
+        level=settings.level.upper(),
+        format=logger_format,
+        serialize=settings.serialize,
+        enqueue=True,  # process logs in background
+        diagnose=False,  # hide variable values in log backtrace
+    )
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/middlewares.py` & `port_ocean-0.1.0.dev4/port_ocean/middlewares.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,46 @@
-from time import time
 from typing import Callable, Awaitable
-from uuid import uuid4
 
 from fastapi import Request, Response
-
 from loguru import logger
 
 from .context.event import event_context
 from .context.ocean import ocean
+from .exceptions.api.base import BaseAPIException, InternalServerException
+from .utils import get_time, get_uuid
 
 
-def get_time(seconds_precision: bool = True) -> float:
-    """Return current time as Unix/Epoch timestamp, in seconds.
-    :param seconds_precision: if True, return with seconds precision as integer (default).
-                              If False, return with milliseconds precision as floating point number of seconds.
-    """
-    return time() if not seconds_precision else int(time())
+async def _handle_silently(
+    call_next: Callable[[Request], Awaitable[Response]], request: Request
+) -> Response:
+    response: Response
+    try:
+        if request.url.path.startswith("/integration"):
+            async with event_context("", trigger_type="request"):
+                await ocean.integration.port_app_config_handler.get_port_app_config()
+                response = await call_next(request)
+        else:
+            response = await call_next(request)
 
+    except BaseAPIException as ex:
+        response = ex.response()
+        if response.status_code < 500:
+            logger.bind(exception=str(ex)).info(
+                "Request did not succeed due to client-side error"
+            )
+        else:
+            logger.opt(exception=True).warning(
+                "Request did not succeed due to server-side error"
+            )
+
+    except Exception:
+        logger.opt(exception=True).error("Request failed due to unexpected error")
+        response = InternalServerException().response()
 
-def get_uuid() -> str:
-    """Return a UUID4 as string"""
-    return str(uuid4())
+    return response
 
 
 async def request_handler(
     request: Request, call_next: Callable[[Request], Awaitable[Response]]
 ) -> Response:
     """Middleware used by FastAPI to process each request, featuring:
 
@@ -33,22 +49,15 @@
       or treat (and log) unexpected exceptions.
     """
     start_time = get_time(seconds_precision=False)
     request_id = get_uuid()
 
     with logger.contextualize(request_id=request_id):
         logger.bind(url=str(request.url), method=request.method).info("Request started")
-        response: Response
-
-        if request.url.path.startswith("integration"):
-            async with event_context(""):
-                await ocean.integration.port_app_config_handler.get_port_app_config()
-                response = await call_next(request)
-        else:
-            response = await call_next(request)
+        response = await _handle_silently(call_next, request)
 
         end_time = get_time(seconds_precision=False)
         time_elapsed = round(end_time - start_time, 5)
         response.headers["X-Request-ID"] = request_id
         response.headers["X-Process-Time"] = str(time_elapsed)
         logger.bind(
             time_elapsed=time_elapsed, response_status=response.status_code
```

### Comparing `port_ocean-0.1.0.dev3/port_ocean/port_ocean.py` & `port_ocean-0.1.0.dev4/port_ocean/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from inspect import getmembers, isclass
 from types import ModuleType
 from typing import Type, Callable
 
 import uvicorn
 from fastapi import FastAPI, APIRouter
 from loguru import logger
+from pydantic import BaseSettings
+from starlette.types import Scope, Receive, Send
 
 from port_ocean.clients.port.client import PortClient
 from port_ocean.config.integration import IntegrationConfiguration
 from port_ocean.context.ocean import (
     PortOceanContext,
     ocean,
     initialize_port_ocean_context,
 )
 from port_ocean.core.integrations.base import BaseIntegration
+from port_ocean.logger_setup import setup_logger
 from port_ocean.middlewares import request_handler
-from pydantic import BaseSettings
-from starlette.types import Scope, Receive, Send
 
 
 def _get_base_integration_class_from_module(
     module: ModuleType,
 ) -> Type[BaseIntegration]:
     for name, obj in getmembers(module):
         if (
@@ -52,17 +53,14 @@
 
 
 def _include_target_channel_router(app: FastAPI, _ocean: PortOceanContext) -> None:
     target_channel_router = APIRouter()
 
     @target_channel_router.post("/resync")
     async def resync() -> None:
-        if _ocean.integration is None:
-            raise Exception("Integration not set")
-
         await _ocean.integration.sync_all()
 
     app.include_router(target_channel_router)
 
 
 class Ocean:
     def __init__(
@@ -106,14 +104,15 @@
                 logger.error(f"Failed to start integration with error: {e}")
                 sys.exit("Server stopped")
 
         await self.fast_api_app(scope, receive, send)
 
 
 def run(path: str) -> None:
+    setup_logger()
     sys.path.append(".")
     try:
         integration_path = f"{path}/integration.py" if path else "integration.py"
         module = _load_module(integration_path)
         integration_class = _get_base_integration_class_from_module(module)
     except Exception:
         integration_class = None
```

### Comparing `port_ocean-0.1.0.dev3/pyproject.toml` & `port_ocean-0.1.0.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.dev3"
+version = "0.1.0.dev4"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
     { include = "port_ocean", from = "." }
 ]
```

### Comparing `port_ocean-0.1.0.dev3/PKG-INFO` & `port_ocean-0.1.0.dev4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev3
+Version: 0.1.0.dev4
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
@@ -23,40 +23,62 @@
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Requires-Dist: werkzeug (>=2.3.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 <img align="right" width="100" height="74" src="https://user-images.githubusercontent.com/8277210/183290025-d7b24277-dfb4-4ce1-bece-7fe0ecd5efd4.svg" />
 
-# Integration Framework
+# Ocean
+[![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
-Integration Framework is a solution developed by Port to address the challenges faced while integrating various third-party systems with our developer portal product. This framework provides a standardized approach for implementing integrations, simplifying the process and allowing platform engineers to focus on the core functionality of the third-party system.
+Ocean is a solution developed by Port to address the challenges faced while integrating various third-party systems with our developer portal product. This framework provides a standardized approach for implementing integrations, simplifying the process and allowing platform engineers to focus on the core functionality of the third-party system.
+
+## Installation
+`pip install port-ocean[cli]` or `poetry add port-ocean[cli]`
+
+## Run Integration
+1. source the integration venv `. .venv/bin/activate`
+2. `ocean sail ./path/to/integration`
+
+## Local Development (Framework)
+1. Clone the repository
+2. Install dependencies: `make install` or `make install/all` for installing integrations dependencies as well
+3. source the integration venv `. .venv/bin/activate`
+
+
+## Local Development (Integration)
+1. Clone the repository
+2. For new integration run `make new` and follow the instructions
+3. Install dependencies: `cd DESIRED_INTEGRATION_FOLDER && make install`
+4. source the integration venv `. .venv/bin/activate`
+5. Run integration: `make run`
  
 ## Export Architecture
 ![image](./assets/IntegrationFrameworkExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/IntergationFrameworkRealTimeUpdatesArchitecture.svg)
 
 ## Self Service Architecture
 ![image](./assets/IntegrationFrameworkSelfServiceArchitecture.svg)
 
 ## Folder Structure
 The Integration Framework follows a specific folder structure within the mono repository. This structure ensures proper organization and easy identification of integration modules. The suggested folder structure is as follows:
 
 ```
-integration-framework/
-├── framework/
-│ ├── main.py
-│ └── requirements.txt
+port-ocean/
+├── port_ocean (framework)/
+│ ├── ocean.py
+│ ├── core/
 | └── ...
 └── integrations/
-├────integration_name/
-│ ├──── main.py
-│ └──── requirements.txt
+│  ├───integration_name/
+│  ├──── main.py
+│  ├──── pyproject.toml
+│  └──── Dockerfile
 ├── ...
 └── ...
 ```
 
 - The `framework` folder contains the core logic for managing the integration lifecycle.
 - Each integration is represented by a separate folder inside the `integrations` directory.
 - Inside each integration folder, you'll find a `main.py` file that implements the core functionality of the integration for the specific third-party system.
@@ -67,28 +89,34 @@
 ![image](./assets/IntegrationFrameworkLifecycleOfIntegration.svg)
 
 ## Configuration
 The Integration Framework utilizes a `config.yaml` file for configuration. This file specifies the integrations to be used within an array. Each integration has a unique identifier and type, which are used during initialization to update Port accordingly.
 
 Example `config.yaml`:
 ```yaml
+# This is an example configuration file for the integration service.
+# Please copy this file to config.yaml file in the integration folder and edit it to your needs.
+
 port:
   clientId: PORT_CLIENT_ID # Can be loaded via environment variable: PORT_CLIENT_ID
   clientSecret: PORT_CLIENT_SECRET # Can be loaded via environment variable: PORT_CLIENT_SECRET
   baseUrl: https://api.getport.io/v1
-triggerChannel: 
+# The trigger channel to use for the integration service.
+triggerChannel:
   type: KAFKA
-integrations:
+  brokers: "localhost:9092"
+  kafkaSecurityEnabled: false
+integration:
   # The name of the integration.
-  - identifier: "my_kafka_integration"
-    # The type of the integration.
-    type: "kafka"
-    # The configuration of the integration.
-    config:
-      bootstrap_servers: "localhost:9092"
+  identifier: "my_integration"
+  # The type of the integration.
+  type: "Git"
+  config:
+    my_git_token: "random"
+    some_other_integration_config: "Very important information"
 ```
 
 ## Contributing
 We welcome contributions to the Integration Framework project. If you have any suggestions, bug reports, or would like to contribute new features, please follow our guidelines outlined in the `CONTRIBUTING.md` file.
 
 ## License
 The Integration Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the `LICENSE` file for more details.
```

