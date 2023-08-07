# Comparing `tmp/vdk-core-0.3.948436673.tar.gz` & `tmp/vdk-core-0.3.957833289.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-core-0.3.948436673.tar", last modified: Fri Jul 28 09:42:30 2023, max compression
+gzip compressed data, was "vdk-core-0.3.957833289.tar", last modified: Mon Aug  7 08:54:52 2023, max compression
```

## Comparing `vdk-core-0.3.948436673.tar` & `vdk-core-0.3.957833289.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-28 09:42:06.000000 vdk-core-0.3.948436673/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2460 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1542 2023-07-28 09:42:06.000000 vdk-core-0.3.948436673/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-28 09:42:30.828073 vdk-core-0.3.948436673/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-28 09:42:06.000000 vdk-core-0.3.948436673/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.812073 vdk-core-0.3.948436673/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.808073 vdk-core-0.3.948436673/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.812073 vdk-core-0.3.948436673/src/vdk/api/
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)    19040 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/job_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.812073 vdk-core-0.3.948436673/src/vdk/api/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/plugin/connection_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     7784 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/plugin/core_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/plugin/hook_markers.py
--rw-rw-rw-   0 root         (0) root         (0)    27782 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/plugin/plugin_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/plugin/plugin_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/api/plugin/plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.812073 vdk-core-0.3.948436673/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/
--rw-rw-rw-   0 root         (0) root         (0)     6060 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/config_help.py
--rw-rw-rw-   0 root         (0) root         (0)     9610 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/job_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11191 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4661 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/impl/
--rw-rw-rw-   0 root         (0) root         (0)     6464 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/impl/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
--rw-rw-rw-   0 root         (0) root         (0)    10048 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/pep249/
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/debug/
--rw-rw-rw-   0 root         (0) root         (0)     6082 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/debug/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.816073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/
--rw-rw-rw-   0 root         (0) root         (0)    29371 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4069 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13247 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/internal_hookspecs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.820073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8208 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.820073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/base_secrets_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/cached_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     3517 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/datajobs_service_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/inmemsecrets.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secrets_api_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2287 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secrets_config.py
--rw-rw-rw-   0 root         (0) root         (0)     7835 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secrets_router.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secretsnotavailable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.820073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    10658 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/notification_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7985 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/
--rw-rw-rw-   0 root         (0) root         (0)     9148 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/cli_run.py
--rw-rw-rw-   0 root         (0) root         (0)    13573 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_environment.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_results.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     7130 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/file_based_step.py
--rw-rw-rw-   0 root         (0) root         (0)     4252 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/job_context.py
--rw-rw-rw-   0 root         (0) root         (0)     7571 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/job_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4856 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/run_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
--rw-rw-rw-   0 root         (0) root         (0)     7959 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3806 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/templates/template_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/file_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3119 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/new_version_check.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)     6471 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/cli_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/core/
--rw-rw-rw-   0 root         (0) root         (0)     9586 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/core/context.py
--rw-rw-rw-   0 root         (0) root         (0)    21237 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/core/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5683 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/core/statestore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     5200 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/plugin/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/plugin/plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk/internal/util/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/util/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-07-28 09:42:07.000000 vdk-core-0.3.948436673/src/vdk/internal/util/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-28 09:42:28.000000 vdk-core-0.3.948436673/src/vdk/internal/vdk_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:30.824073 vdk-core-0.3.948436673/src/vdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4857 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:30.000000 vdk-core-0.3.948436673/src/vdk_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-07-28 09:42:28.000000 vdk-core-0.3.948436673/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-08-07 08:54:52.067839 vdk-core-0.3.957833289/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.051839 vdk-core-0.3.957833289/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.047839 vdk-core-0.3.957833289/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.051839 vdk-core-0.3.957833289/src/vdk/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    19040 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/job_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.051839 vdk-core-0.3.957833289/src/vdk/api/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/plugin/connection_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/plugin/core_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/plugin/hook_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)    27782 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/plugin/plugin_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/plugin/plugin_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/api/plugin/plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.051839 vdk-core-0.3.957833289/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.051839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     6060 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.051839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/config_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     9717 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/job_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11191 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.055839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.055839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/impl/
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/impl/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10048 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.055839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/pep249/
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.055839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/debug/
+-rw-rw-rw-   0 root         (0) root         (0)     6082 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/debug/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.055839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)    29371 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/internal_hookspecs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.055839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8208 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.059839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/base_secrets_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/cached_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/datajobs_service_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/inmemsecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secrets_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2287 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secrets_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7835 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secrets_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secretsnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.059839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    10658 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/notification_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7985 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.059839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/
+-rw-rw-rw-   0 root         (0) root         (0)     9148 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/cli_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    13573 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_results.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     7130 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/file_based_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/job_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/job_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4856 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/run_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7959 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/templates/template_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/file_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3119 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/new_version_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6471 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/cli_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/core/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    21237 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/core/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/core/statestore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk/internal/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/plugin/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/plugin/plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk/internal/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/util/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-08-07 08:54:24.000000 vdk-core-0.3.957833289/src/vdk/internal/util/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-08-07 08:54:49.000000 vdk-core-0.3.957833289/src/vdk/internal/vdk_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 08:54:52.063839 vdk-core-0.3.957833289/src/vdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-08-07 08:54:51.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4857 2023-08-07 08:54:52.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:54:51.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-08-07 08:54:51.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 08:54:51.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-08-07 08:54:51.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-07 08:54:51.000000 vdk-core-0.3.957833289/src/vdk_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-08-07 08:54:49.000000 vdk-core-0.3.957833289/version.txt
```

### Comparing `vdk-core-0.3.948436673/PKG-INFO` & `vdk-core-0.3.957833289/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.948436673
+Version: 0.3.957833289
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.948436673/README.md` & `vdk-core-0.3.957833289/README.md`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/setup.cfg` & `vdk-core-0.3.957833289/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/data_job.py` & `vdk-core-0.3.957833289/src/vdk/api/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/job_input.py` & `vdk-core-0.3.957833289/src/vdk/api/job_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/plugin/connection_hook_spec.py` & `vdk-core-0.3.957833289/src/vdk/api/plugin/connection_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/plugin/core_hook_spec.py` & `vdk-core-0.3.957833289/src/vdk/api/plugin/core_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/plugin/hook_markers.py` & `vdk-core-0.3.957833289/src/vdk/api/plugin/hook_markers.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/plugin/plugin_input.py` & `vdk-core-0.3.957833289/src/vdk/api/plugin/plugin_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/plugin/plugin_registry.py` & `vdk-core-0.3.957833289/src/vdk/api/plugin/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/api/plugin/plugin_utils.py` & `vdk-core-0.3.957833289/src/vdk/api/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/builtin_hook_impl.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/builtin_hook_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/config_help.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/config_help.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/job_config.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/job_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,32 +38,37 @@
 
 class JobConfig:
     """
     User facing configuration of a Data Job.
     For more see the user wiki
     """
 
-    def __init__(self, data_job_path: Union[pathlib.Path, str]):
+    def __init__(
+        self, data_job_path: Union[pathlib.Path, str], should_fail_missing_config=False
+    ):
         self._config_ini = configparser.ConfigParser()
         self._config_file = os.path.join(data_job_path, "config.ini")
+        self._should_fail_missing_config = should_fail_missing_config
 
         if not os.path.isfile(self._config_file):
-            # TODO: Figure out a way to properly handle cases where there is no config.ini present
-            log.info("Missing config.ini file.")
-            # raise VdkConfigurationError(
-            #     ErrorMessage(
-            #         summary="Error while loading config.ini file",
-            #         what="Cannot extract job Configuration",
-            #         why=f"Configuration file config.ini is missing in data job path: {data_job_path}",
-            #         consequences="Cannot deploy and configure the data job without config.ini file.",
-            #         countermeasures="config.ini must be in the root of the data job folder. "
-            #         "Make sure the file is created "
-            #         "or double check the data job path is passed correctly.",
-            #     )
-            # )
+            if should_fail_missing_config:
+                raise VdkConfigurationError(
+                    ErrorMessage(
+                        summary="Error while loading config.ini file",
+                        what="Cannot extract job Configuration",
+                        why=f"Configuration file config.ini is missing in data job path: {data_job_path}",
+                        consequences="Cannot deploy and configure the data job without config.ini file.",
+                        countermeasures="config.ini must be in the root of the data job folder. "
+                        "Make sure the file is created "
+                        "or double check the data job path is passed correctly.",
+                    )
+                )
+            else:
+                log.info("Missing config.ini file.")
+
         self._read_config_ini_file(
             config_parser=self._config_ini, configuration_file_path=self._config_file
         )
 
     def get_team(self) -> str:
         """
         Specified which is the team that owns the data job.
```

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/log_config.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/config/vdk_config.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/config/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/connection_hooks.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/connection_hooks.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/connection_plugin.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/connection_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/execution_cursor.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/execution_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/impl/router.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/impl/router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/managed_cursor.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/managed_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/debug/debug.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/debug/debug.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/internal_hookspecs.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/internal_hookspecs.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/properties_config.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/properties_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/properties_router.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/properties_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/base_secrets_impl.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/base_secrets_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/cached_secrets.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/cached_secrets.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/datajobs_service_secrets.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/datajobs_service_secrets.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/inmemsecrets.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/inmemsecrets.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secrets_api_plugin.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secrets_api_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secrets_config.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secrets_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secrets_router.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secrets_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/job_secrets/secretsnotavailable.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/job_secrets/secretsnotavailable.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/notification.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/notification.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/notification_base.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/notification_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/notification/notification_configuration.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/notification/notification_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/cli_run.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/cli_run.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/data_job.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_environment.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_environment.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_results.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_results.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_state.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_state.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/execution_tracking.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/execution_tracking.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/file_based_step.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/file_based_step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/job_context.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/job_context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/job_input.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/job_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/standalone_data_job.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/standalone_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/run/step.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/run/step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/templates/template_impl.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/templates/template_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/file_util.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/file_util.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/writer.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/writer.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/new_version_check.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/new_version_check.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/builtin_plugins/version/version.py` & `vdk-core-0.3.957833289/src/vdk/internal/builtin_plugins/version/version.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/cli_entry.py` & `vdk-core-0.3.957833289/src/vdk/internal/cli_entry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/core/config.py` & `vdk-core-0.3.957833289/src/vdk/internal/core/config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/core/context.py` & `vdk-core-0.3.957833289/src/vdk/internal/core/context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/core/errors.py` & `vdk-core-0.3.957833289/src/vdk/internal/core/errors.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/core/statestore.py` & `vdk-core-0.3.957833289/src/vdk/internal/core/statestore.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/plugin/plugin.py` & `vdk-core-0.3.957833289/src/vdk/internal/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/util/decorators.py` & `vdk-core-0.3.957833289/src/vdk/internal/util/decorators.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk/internal/util/utils.py` & `vdk-core-0.3.957833289/src/vdk/internal/util/utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.948436673/src/vdk_core.egg-info/PKG-INFO` & `vdk-core-0.3.957833289/src/vdk_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.948436673
+Version: 0.3.957833289
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.948436673/src/vdk_core.egg-info/SOURCES.txt` & `vdk-core-0.3.957833289/src/vdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

