# Comparing `tmp/port_ocean-0.1.4.dev3.tar.gz` & `tmp/port_ocean-0.1.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.4.dev3.tar", max compression
+gzip compressed data, was "port_ocean-0.1.4.dev4.tar", max compression
```

## Comparing `port_ocean-0.1.4.dev3.tar` & `port_ocean-0.1.4.dev4.tar`

### file list

```diff
@@ -1,101 +1,99 @@
--rw-r--r--   0        0        0    11357 2023-08-06 16:03:03.662717 port_ocean-0.1.4.dev3/LICENSE
--rw-r--r--   0        0        0     4639 2023-08-06 16:03:03.662717 port_ocean-0.1.4.dev3/README.md
--rw-r--r--   0        0        0      270 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/__init__.py
--rw-r--r--   0        0        0      328 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0       57 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cli.py
--rw-r--r--   0        0        0      278 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/__init__.py
--rw-r--r--   0        0        0     1134 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/list_integrations.py
--rw-r--r--   0        0        0     1057 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/main.py
--rw-r--r--   0        0        0     1816 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/new.py
--rw-r--r--   0        0        0     2306 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/pull.py
--rw-r--r--   0        0        0     1534 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/sail.py
--rw-r--r--   0        0        0      536 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/commands/version.py
--rw-r--r--   0        0        0      429 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       42 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2698 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0       12 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
--rw-r--r--   0        0        0      388 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
--rw-r--r--   0        0        0      292 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      449 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1680 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      655 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0       12 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
--rw-r--r--   0        0        0      898 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
--rw-r--r--   0        0        0       65 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
--rw-r--r--   0        0        0     1669 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1941 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0       54 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/cli/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2563 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2309 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     2928 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/blueprints.py
--rw-r--r--   0        0        0     5623 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3909 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      781 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     4011 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/config/base.py
--rw-r--r--   0        0        0     1816 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/config/dynamic.py
--rw-r--r--   0        0        0     1231 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/config/settings.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     4147 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3201 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/context/event.py
--rw-r--r--   0        0        0     4283 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/base.py
--rw-r--r--   0        0        0      607 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/__init__.py
--rw-r--r--   0        0        0      891 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/base.py
--rw-r--r--   0        0        0     3474 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/factory.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/http/__init__.py
--rw-r--r--   0        0        0     2511 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/http/event_listener.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/kafka/__init__.py
--rw-r--r--   0        0        0     6351 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/kafka/event_listener.py
--rw-r--r--   0        0        0     3264 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/polling/event_listener.py
--rw-r--r--   0        0        0     2799 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/event_listener/polling/utils.py
--rw-r--r--   0        0        0      716 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/__init__.py
--rw-r--r--   0        0        0      869 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/base.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/__init__.py
--rw-r--r--   0        0        0     7977 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/applier.py
--rw-r--r--   0        0        0     1751 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
--rw-r--r--   0        0        0     1035 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     1392 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entity_processor/__init__.py
--rw-r--r--   0        0        0      955 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entity_processor/base.py
--rw-r--r--   0        0        0     2685 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      396 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1810 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     3162 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      698 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2569 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0    11843 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0     1747 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/utils.py
--rw-r--r--   0        0        0      909 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/models.py
--rw-r--r--   0        0        0      781 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/ocean_types.py
--rw-r--r--   0        0        0     1957 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      532 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      407 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/exceptions/port_defaults.py
--rw-r--r--   0        0        0     1107 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2475 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/middlewares.py
--rw-r--r--   0        0        0     2263 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/ocean.py
--rw-r--r--   0        0        0     7161 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/port_defaults.py
--rw-r--r--   0        0        0        0 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/py.typed
--rw-r--r--   0        0        0     2834 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/run.py
--rw-r--r--   0        0        0     1007 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/port_ocean/utils.py
--rw-r--r--   0        0        0     3462 2023-08-06 16:03:03.678717 port_ocean-0.1.4.dev3/pyproject.toml
--rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 port_ocean-0.1.4.dev3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 07:41:59.987208 port_ocean-0.1.4.dev4/LICENSE
+-rw-r--r--   0        0        0     4639 2023-08-07 07:41:59.987208 port_ocean-0.1.4.dev4/README.md
+-rw-r--r--   0        0        0      270 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/__init__.py
+-rw-r--r--   0        0        0      328 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0       57 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0      278 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1134 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/list_integrations.py
+-rw-r--r--   0        0        0     1057 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/main.py
+-rw-r--r--   0        0        0     1816 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/new.py
+-rw-r--r--   0        0        0     2306 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/pull.py
+-rw-r--r--   0        0        0     1534 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/sail.py
+-rw-r--r--   0        0        0      536 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/commands/version.py
+-rw-r--r--   0        0        0      429 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0       12 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/resources/.gitignore
+-rw-r--r--   0        0        0      388 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.port/spec.yaml
+-rw-r--r--   0        0        0      292 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      449 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1680 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      655 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       12 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/changelog/.gitignore
+-rw-r--r--   0        0        0      898 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml
+-rw-r--r--   0        0        0       65 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1941 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0       54 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/cli/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2563 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2309 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     2928 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/blueprints.py
+-rw-r--r--   0        0        0     5623 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3909 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      781 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     4011 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1816 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/config/dynamic.py
+-rw-r--r--   0        0        0     1231 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/config/settings.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     4147 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3710 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4283 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/base.py
+-rw-r--r--   0        0        0      607 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/__init__.py
+-rw-r--r--   0        0        0      580 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/base.py
+-rw-r--r--   0        0        0     2555 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/factory.py
+-rw-r--r--   0        0        0     1165 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/http/event_listener.py
+-rw-r--r--   0        0        0     3349 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/kafka/event_listener.py
+-rw-r--r--   0        0        0     1867 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/polling/event_listener.py
+-rw-r--r--   0        0        0     2799 2023-08-07 07:41:59.999208 port_ocean-0.1.4.dev4/port_ocean/core/event_listener/polling/utils.py
+-rw-r--r--   0        0        0      716 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/__init__.py
+-rw-r--r--   0        0        0      869 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/__init__.py
+-rw-r--r--   0        0        0     7977 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/applier.py
+-rw-r--r--   0        0        0     1751 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py
+-rw-r--r--   0        0        0     1115 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     1392 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entity_processor/__init__.py
+-rw-r--r--   0        0        0      955 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entity_processor/base.py
+-rw-r--r--   0        0        0     2685 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      396 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1810 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1912 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      698 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2569 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0    12314 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0     1747 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/utils.py
+-rw-r--r--   0        0        0      642 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/models.py
+-rw-r--r--   0        0        0      781 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/ocean_types.py
+-rw-r--r--   0        0        0     1957 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      532 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      407 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/exceptions/port_defaults.py
+-rw-r--r--   0        0        0     1107 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     2263 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/ocean.py
+-rw-r--r--   0        0        0     7161 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/port_defaults.py
+-rw-r--r--   0        0        0        0 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/py.typed
+-rw-r--r--   0        0        0     2834 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/run.py
+-rw-r--r--   0        0        0     1007 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/port_ocean/utils.py
+-rw-r--r--   0        0        0     3462 2023-08-07 07:42:00.003208 port_ocean-0.1.4.dev4/pyproject.toml
+-rw-r--r--   0        0        0     6361 1970-01-01 00:00:00.000000 port_ocean-0.1.4.dev4/PKG-INFO
```

### Comparing `port_ocean-0.1.4.dev3/LICENSE` & `port_ocean-0.1.4.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/README.md` & `port_ocean-0.1.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/commands/list_integrations.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/commands/list_integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/commands/main.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/commands/new.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/commands/pull.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/commands/pull.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/commands/sail.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/commands/sail.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/commands/version.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md` & `port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml` & `port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/config.yaml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py` & `port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.4.dev4/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/authentication.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/client.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/client.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/blueprints.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/blueprints.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/mixins/integrations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/types.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/clients/port/utils.py` & `port_ocean-0.1.4.dev4/port_ocean/clients/port/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/config/base.py` & `port_ocean-0.1.4.dev4/port_ocean/config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/config/dynamic.py` & `port_ocean-0.1.4.dev4/port_ocean/config/dynamic.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/config/settings.py` & `port_ocean-0.1.4.dev4/port_ocean/config/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.4.dev4/port_ocean/consumers/kafka_consumer.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/context/event.py` & `port_ocean-0.1.4.dev4/port_ocean/context/event.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 from loguru import logger
 from werkzeug.local import LocalStack, LocalProxy
 
 from port_ocean.exceptions.context import EventContextNotFoundError
 from port_ocean.utils import get_time
 
 if TYPE_CHECKING:
-    from port_ocean.core.handlers.port_app_config.models import PortAppConfig
+    from port_ocean.core.handlers.port_app_config.models import (
+        PortAppConfig,
+        ResourceConfig,
+    )
 
 TriggerType = Literal["manual", "machine", "request"]
 
 
 class EventType:
     START = "start"
     RESYNC = "resync"
     HTTP_REQUEST = "http_request"
 
 
 @dataclass
 class EventContext:
     event_type: str
     trigger_type: TriggerType = "machine"
+    resource_config: Optional["ResourceConfig"] = None
     attributes: dict[str, Any] = field(default_factory=dict)
     _port_app_config: Optional["PortAppConfig"] = None
     _parent_event: Optional["EventContext"] = None
     _event_id: str = field(default_factory=lambda: str(uuid4()))
 
     @property
     def id(self) -> str:
@@ -72,34 +76,42 @@
 event: EventContext = LocalProxy(lambda: _get_event_context())  # type: ignore
 
 
 @asynccontextmanager
 async def event_context(
     event_type: str,
     trigger_type: TriggerType = "manual",
+    resource_config: Optional["ResourceConfig"] = None,
     attributes: dict[str, Any] | None = None,
 ) -> AsyncIterator[EventContext]:
     attributes = attributes or {}
 
     parent = _event_context_stack.top
 
     _event_context_stack.push(
         EventContext(
             event_type,
             trigger_type=trigger_type,
+            resource_config=resource_config,
             attributes=attributes,
             _parent_event=parent,
+            # inherit port app config from parent event so it can be used in nested events
+            _port_app_config=parent.port_app_config if parent else None,
         )
     )
 
     start_time = get_time(seconds_precision=False)
     with logger.contextualize(
         event_trigger_type=event.trigger_type,
         event_kind=event.event_type,
         event_id=event.id,
+        event_parent_id=event.parent_id,
+        event_resource_kind=event.resource_config.kind
+        if event.resource_config
+        else None,
     ):
         logger.info("Event started")
         try:
             yield event
         except:
             success = False
             raise
```

### Comparing `port_ocean-0.1.4.dev3/port_ocean/context/ocean.py` & `port_ocean-0.1.4.dev4/port_ocean/context/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/event_listener/__init__.py` & `port_ocean-0.1.4.dev4/port_ocean/core/event_listener/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/event_listener/base.py` & `port_ocean-0.1.4.dev4/port_ocean/core/event_listener/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from abc import abstractmethod
 from typing import TypedDict, Callable, Any, Awaitable
 
 from pydantic import BaseModel, Extra
 
 
 class EventListenerEvents(TypedDict):
-    """
-    A dictionary containing event types and their corresponding event handlers.
-    """
     on_resync: Callable[[dict[Any, Any]], Awaitable[None]]
 
 
 class BaseEventListener:
     def __init__(
         self,
         events: EventListenerEvents,
@@ -23,12 +20,8 @@
         pass
 
 
 class EventListenerSettings(BaseModel, extra=Extra.allow):
     type: str
 
     def to_request(self) -> dict[str, Any]:
-        """
-        Converts the Settings object to a dictionary representation (request format).
-        This method is used when configuring the event listener settings for the Polling event listener.
-        """
         return {"type": self.type}
```

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/event_listener/factory.py` & `port_ocean-0.1.4.dev4/port_ocean/core/event_listener/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,42 +16,25 @@
     BaseEventListener,
     EventListenerEvents,
 )
 from port_ocean.exceptions.core import UnsupportedEventListenerTypeException
 
 
 class EventListenerFactory(BaseWithContext):
-    """
-    This class is responsible for creating different types of event listeners based on the provided configuration.
-    The factory takes a PortOceanContext, installation_id, and events dictionary as parameters.
-
-    Parameters:
-        context (PortOceanContext): The PortOceanContext object containing information about the current application context.
-        installation_id (str): The identifier of the installation associated with the event listener.
-        events (EventListenerEvents): A dictionary containing event types and their corresponding event handlers.
-
-    """
     def __init__(
         self,
         context: PortOceanContext,
         installation_id: str,
         events: EventListenerEvents,
     ):
         super().__init__(context)
         self.installation_id = installation_id
         self.events = events
 
     async def create_event_listener(self) -> BaseEventListener:
-        """
-        Creates and returns a specific event listener based on the provided configuration.
-        The event listener is wrapped with the events provided in the factory's initialization.
-        
-        Raises:
-            UnsupportedEventListenerTypeException: If the event listener type is not supported.
-        """
         wrapped_events: EventListenerEvents = {"on_resync": self.events["on_resync"]}
         event_listener: BaseEventListener
         config = self.context.config.event_listener
         _type = config.type.lower()
         assert_message = "Invalid event listener config, expected KafkaEventListenerSettings and got {0}"
         logger.info(f"Found event listener type: {_type}")
```

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/event_listener/polling/event_listener.py` & `port_ocean-0.1.4.dev4/port_ocean/core/event_listener/polling/event_listener.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,55 +8,33 @@
     EventListenerEvents,
     EventListenerSettings,
 )
 from port_ocean.core.event_listener.polling.utils import repeat_every
 
 
 class PollingEventListenerSettings(EventListenerSettings):
-    """
-    Attributes:
-        type (Literal["POLLING"]): A literal indicating the type of the event listener, which is set to "POLLING" for this class.
-        resync_on_start (bool): A flag indicating whether to trigger a resync event on the start of the polling event listener.
-                                If True, the "on_resync" event will be triggered immediately when the polling listener starts.
-        interval (int): The interval in seconds at which the polling event listener checks for changes in the integration.
-                        The default interval is set to 60 seconds.
-    """
     type: Literal["POLLING"]
     resync_on_start: bool = True
     interval: int = 60
 
     def to_request(self) -> dict[str, Any]:
         return {}
 
 
 class PollingEventListener(BaseEventListener):
-    """
-    Polling event listener that checks for changes in the integration every `interval` seconds.
-
-    The `PollingEventListener` periodically checks for changes in the integration and triggers the "on_resync" event if changes are detected.
-
-    Parameters:
-        events (EventListenerEvents): A dictionary containing event types and their corresponding event handlers.
-        event_listener_config (PollingEventListenerSettings): Configuration settings for the Polling event listener.
-    """
     def __init__(
         self,
         events: EventListenerEvents,
         event_listener_config: PollingEventListenerSettings,
     ):
         super().__init__(events)
         self.event_listener_config = event_listener_config
         self._last_updated_at = None
 
     async def start(self) -> None:
-        """
-        Starts the polling event listener.
-        It registers the "on_resync" event to be called every `interval` seconds specified in the `event_listener_config`.
-        The `on_resync` event is triggered if the integration has changed since the last update.
-        """
         logger.info(
             f"Setting up Polling event listener with interval: {self.event_listener_config.interval}"
         )
 
         @repeat_every(seconds=self.event_listener_config.interval)
         async def resync() -> None:
             logger.info(
```

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/event_listener/polling/utils.py` & `port_ocean-0.1.4.dev4/port_ocean/core/event_listener/polling/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/__init__.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/base.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/applier.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/applier.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/get_related_entities.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/order_by_entities_dependencies.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,20 +15,22 @@
     entities_map = {}
 
     for entity in entities:
         nodes[node(entity)] = set()
         entities_map[node(entity)] = entity
 
     for entity in entities:
-        relation_target_ids: list[str] = [
-            identifier
-            for relation in entity.relations.values()
-            if relation is not None
-            for identifier in relation
-        ]
+        relation_target_ids: list[str] = sum(
+            [
+                identifiers if isinstance(identifiers, list) else [identifiers]
+                for identifiers in entity.relations.values()
+                if identifiers is not None
+            ],
+            [],
+        )
         related_entities = [
             related for related in entities if related.identifier in relation_target_ids
         ]
 
         for related_entity in related_entities:
             nodes[node(entity)].add(node(related_entity))
```

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entities_state_applier/port/validate_entity_relations.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entity_processor/base.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entity_processor/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/entity_processor/jq_entity_processor.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/entity_processor/jq_entity_processor.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.4.dev4/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/sync.py`

 * *Files 5% similar despite different names*

```diff
@@ -308,19 +308,27 @@
         async with event_context(EventType.RESYNC, trigger_type=trigger_type):
             app_config = await self.port_app_config_handler.get_port_app_config()
 
             entities_at_port = await ocean.port_client.search_entities(user_agent_type)
 
             creation_results: list[tuple[list[Entity], list[Exception]]] = []
             for resource in app_config.resources:
-                creation_results.append(
-                    await self._register_in_batches(
-                        resource, user_agent_type, ocean.config.batch_work_size
+                # create event context per resource kind, so resync method could have access to the resource config
+                # as we might have multiple resources with the same kind name
+                async with event_context(
+                    EventType.RESYNC,
+                    trigger_type=trigger_type,
+                    resource_config=resource,
+                    attributes={"resource_kind": resource.kind},
+                ):
+                    creation_results.append(
+                        await self._register_in_batches(
+                            resource, user_agent_type, ocean.config.batch_work_size
+                        )
                     )
-                )
             flat_created_entities, errors = zip_and_sum(creation_results) or [[], []]
 
             if errors:
                 message = f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state"
                 error_group = ExceptionGroup(
                     f"Resync failed with {len(errors)}. Skipping delete phase due to incomplete state",
                     errors,
```

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/integrations/mixins/utils.py` & `port_ocean-0.1.4.dev4/port_ocean/core/integrations/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/ocean_types.py` & `port_ocean-0.1.4.dev4/port_ocean/core/ocean_types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/core/utils.py` & `port_ocean-0.1.4.dev4/port_ocean/core/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/exceptions/core.py` & `port_ocean-0.1.4.dev4/port_ocean/exceptions/core.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/logger_setup.py` & `port_ocean-0.1.4.dev4/port_ocean/logger_setup.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/middlewares.py` & `port_ocean-0.1.4.dev4/port_ocean/middlewares.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/ocean.py` & `port_ocean-0.1.4.dev4/port_ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/port_defaults.py` & `port_ocean-0.1.4.dev4/port_ocean/port_defaults.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/run.py` & `port_ocean-0.1.4.dev4/port_ocean/run.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/port_ocean/utils.py` & `port_ocean-0.1.4.dev4/port_ocean/utils.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.4.dev3/pyproject.toml` & `port_ocean-0.1.4.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.4dev3"
+version = "0.1.4dev4"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 homepage = "https://app.getport.io"
 repository = "https://github.com/port-labs/Port-Ocean"
 
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
```

### Comparing `port_ocean-0.1.4.dev3/PKG-INFO` & `port_ocean-0.1.4.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.4.dev3
+Version: 0.1.4.dev4
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Home-page: https://app.getport.io
 Keywords: ocean,port-ocean,port
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Framework :: FastAPI
```

