# Comparing `tmp/bk-plugin-framework-2.0.3.tar.gz` & `tmp/bk-plugin-framework-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk-plugin-framework-2.0.3.tar", max compression
+gzip compressed data, was "bk-plugin-framework-2.0.4.tar", max compression
```

## Comparing `bk-plugin-framework-2.0.3.tar` & `bk-plugin-framework-2.0.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/__init__.py
--rw-r--r--   0        0        0      753 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/__version__.py
--rw-r--r--   0        0        0      846 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/constants.py
--rw-r--r--   0        0        0     2752 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/envs.py
--rw-r--r--   0        0        0     2439 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/hub/__init__.py
--rw-r--r--   0        0        0      941 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/kit/__init__.py
--rw-r--r--   0        0        0     2130 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/kit/api.py
--rw-r--r--   0        0        0      938 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/kit/authentication.py
--rw-r--r--   0        0        0     1496 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/kit/decorators.py
--rw-r--r--   0        0        0     7433 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/kit/plugin.py
--rw-r--r--   0        0        0     4262 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/metrics.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/__init__.py
--rw-r--r--   0        0        0      811 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/__init__.py
--rw-r--r--   0        0        0     4248 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/api.py
--rw-r--r--   0        0        0      923 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/apps.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/celery/__init__.py
--rw-r--r--   0        0        0      915 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/celery/queues.py
--rw-r--r--   0        0        0     3669 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/celery/tasks.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/migrations/__init__.py
--rw-r--r--   0        0        0    13138 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/executor.py
--rw-r--r--   0        0        0      807 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/__init__.py
--rw-r--r--   0        0        0      986 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/admin.py
--rw-r--r--   0        0        0      846 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/apps.py
--rw-r--r--   0        0        0     1354 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/log.py
--rw-r--r--   0        0        0     1574 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/migrations/__init__.py
--rw-r--r--   0        0        0     1422 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/models.py
--rw-r--r--   0        0        0      811 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/__init__.py
--rw-r--r--   0        0        0     1022 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/admin.py
--rw-r--r--   0        0        0      948 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/apps.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/beat.py
--rw-r--r--   0        0        0     1011 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/queues.py
--rw-r--r--   0        0        0     2560 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/tasks.py
--rw-r--r--   0        0        0     1649 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py
--rw-r--r--   0        0        0      407 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0002_schedule_finish_at.py
--rw-r--r--   0        0        0      552 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py
--rw-r--r--   0        0        0      430 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0004_schedule_scheduling.py
--rw-r--r--   0        0        0      458 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0005_schedule_err.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/__init__.py
--rw-r--r--   0        0        0     2324 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/models.py
--rw-r--r--   0        0        0     1372 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/utils.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/__init__.py
--rw-r--r--   0        0        0      817 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/__init__.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/admin.py
--rw-r--r--   0        0        0     1006 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/__init__.py
--rw-r--r--   0        0        0     2504 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/callback.py
--rw-r--r--   0        0        0     3613 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/detail.py
--rw-r--r--   0        0        0     4299 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/invoke.py
--rw-r--r--   0        0        0     2078 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/logs.py
--rw-r--r--   0        0        0     3391 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/meta.py
--rw-r--r--   0        0        0     5977 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py
--rw-r--r--   0        0        0     3961 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/schedule.py
--rw-r--r--   0        0        0      997 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py
--rw-r--r--   0        0        0     1046 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/apps.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/__init__.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/__init__.py
--rw-r--r--   0        0        0      462 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-definition.yml
--rw-r--r--   0        0        0     2414 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml
--rw-r--r--   0        0        0      401 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-strategy-cors.yml
--rw-r--r--   0        0        0     2308 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py
--rw-r--r--   0        0        0     1093 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/middlewares.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/migrations/__init__.py
--rw-r--r--   0        0        0     1766 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/urls.py
--rw-r--r--   0        0        0        0 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/__init__.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/management/commands/__init__.py
--rw-r--r--   0        0        0     1753 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/migrations/__init__.py
--rw-r--r--   0        0        0      997 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/views.py
--rw-r--r--   0        0        0      730 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/utils/__init__.py
--rw-r--r--   0        0        0      981 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/utils/local.py
--rw-r--r--   0        0        0      928 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/utils/log.py
--rw-r--r--   0        0        0     1957 2023-07-03 08:53:05.313684 bk-plugin-framework-2.0.3/bk_plugin_framework/utils/module_load.py
--rw-r--r--   0        0        0      724 2023-07-03 08:53:05.317682 bk-plugin-framework-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1820 2023-07-03 08:53:25.672029 bk-plugin-framework-2.0.3/setup.py
--rw-r--r--   0        0        0      666 2023-07-03 08:53:25.672395 bk-plugin-framework-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.763147 bk-plugin-framework-2.0.4/bk_plugin_framework/__init__.py
+-rw-r--r--   0        0        0      753 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/__version__.py
+-rw-r--r--   0        0        0      846 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/constants.py
+-rw-r--r--   0        0        0     2752 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/envs.py
+-rw-r--r--   0        0        0     2439 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/hub/__init__.py
+-rw-r--r--   0        0        0      941 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/kit/__init__.py
+-rw-r--r--   0        0        0     2130 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/kit/api.py
+-rw-r--r--   0        0        0      938 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/kit/authentication.py
+-rw-r--r--   0        0        0     1496 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/kit/decorators.py
+-rw-r--r--   0        0        0     7433 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/kit/plugin.py
+-rw-r--r--   0        0        0     4262 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/metrics.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/__init__.py
+-rw-r--r--   0        0        0      811 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/__init__.py
+-rw-r--r--   0        0        0     4248 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/api.py
+-rw-r--r--   0        0        0      923 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/apps.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/celery/__init__.py
+-rw-r--r--   0        0        0      915 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/celery/queues.py
+-rw-r--r--   0        0        0     3669 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/celery/tasks.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/migrations/__init__.py
+-rw-r--r--   0        0        0    13138 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/executor.py
+-rw-r--r--   0        0        0      807 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/__init__.py
+-rw-r--r--   0        0        0      986 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/admin.py
+-rw-r--r--   0        0        0      846 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/apps.py
+-rw-r--r--   0        0        0     1354 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/log.py
+-rw-r--r--   0        0        0     1574 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/migrations/__init__.py
+-rw-r--r--   0        0        0     1422 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/models.py
+-rw-r--r--   0        0        0      811 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/__init__.py
+-rw-r--r--   0        0        0     1022 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/admin.py
+-rw-r--r--   0        0        0      948 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/apps.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/__init__.py
+-rw-r--r--   0        0        0     1051 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/beat.py
+-rw-r--r--   0        0        0     1011 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/queues.py
+-rw-r--r--   0        0        0     2560 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/tasks.py
+-rw-r--r--   0        0        0     1649 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py
+-rw-r--r--   0        0        0      407 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0002_schedule_finish_at.py
+-rw-r--r--   0        0        0      552 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py
+-rw-r--r--   0        0        0      430 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0004_schedule_scheduling.py
+-rw-r--r--   0        0        0      458 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0005_schedule_err.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/__init__.py
+-rw-r--r--   0        0        0     2324 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/models.py
+-rw-r--r--   0        0        0     1372 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/utils.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/__init__.py
+-rw-r--r--   0        0        0      817 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/__init__.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/admin.py
+-rw-r--r--   0        0        0     1006 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/__init__.py
+-rw-r--r--   0        0        0     2504 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/callback.py
+-rw-r--r--   0        0        0     3613 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/detail.py
+-rw-r--r--   0        0        0     4299 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/invoke.py
+-rw-r--r--   0        0        0     2078 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/logs.py
+-rw-r--r--   0        0        0     3391 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/meta.py
+-rw-r--r--   0        0        0     5977 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py
+-rw-r--r--   0        0        0     3961 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/schedule.py
+-rw-r--r--   0        0        0      997 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py
+-rw-r--r--   0        0        0     1046 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/apps.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/__init__.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/__init__.py
+-rw-r--r--   0        0        0      462 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/data/api-definition.yml
+-rw-r--r--   0        0        0     2414 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml
+-rw-r--r--   0        0        0      401 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/data/api-strategy-cors.yml
+-rw-r--r--   0        0        0     2308 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py
+-rw-r--r--   0        0        0     1093 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/middlewares.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/migrations/__init__.py
+-rw-r--r--   0        0        0     1766 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/urls.py
+-rw-r--r--   0        0        0        0 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/__init__.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/management/commands/__init__.py
+-rw-r--r--   0        0        0     1753 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/migrations/__init__.py
+-rw-r--r--   0        0        0      997 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/views.py
+-rw-r--r--   0        0        0      730 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/utils/__init__.py
+-rw-r--r--   0        0        0      981 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/utils/local.py
+-rw-r--r--   0        0        0      928 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/utils/log.py
+-rw-r--r--   0        0        0     1957 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/bk_plugin_framework/utils/module_load.py
+-rw-r--r--   0        0        0      724 2023-08-07 02:22:46.767147 bk-plugin-framework-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1820 2023-08-07 02:23:00.761133 bk-plugin-framework-2.0.4/setup.py
+-rw-r--r--   0        0        0      666 2023-08-07 02:23:00.761427 bk-plugin-framework-2.0.4/PKG-INFO
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/__version__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 You may obtain a copy of the License at
 http://opensource.org/licenses/MIT
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 """
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/constants.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/constants.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/envs.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/envs.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import base64
 import hashlib
 import logging
 
 from pydantic import BaseSettings
 from django.conf import settings as default_settings
 
-logger = logging.getLogger("bk-plugin")
+logger = logging.getLogger("bk_plugin")
 
 
 def compute_settings(settings: BaseSettings) -> dict:
     """
     对需要计算的环境变量进行计算
     :param settings:
     :return:
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/hub/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/kit/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/kit/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/kit/api.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/kit/api.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/kit/authentication.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/kit/authentication.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/kit/decorators.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/kit/decorators.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/kit/plugin.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/kit/plugin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/metrics.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/metrics.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/api.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from celery import current_app
 from cryptography.fernet import Fernet
 
 from bk_plugin_framework.envs import settings
 from bk_plugin_framework.runtime.schedule.models import Schedule
 from bk_plugin_framework.constants import State
 
-logger = logging.getLogger("bk-plugin")
+logger = logging.getLogger("bk_plugin")
 
 
 class CallbackPreparation(object):
     def __init__(self, callback_id: str, callback_url: str):
         self.id = callback_id
         self.url = callback_url
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/apps.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/celery/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/celery/queues.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/celery/queues.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/celery/tasks.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/callback/migrations/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/callback/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/executor.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/executor.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/admin.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/admin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/apps.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/log.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/log.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/loghub/models.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/loghub/models.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/admin.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/admin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/apps.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/beat.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/beat.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/queues.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/queues.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/celery/tasks.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/0003_auto_20210830_1945.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/migrations/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/models.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/models.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/runtime/schedule/utils.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/runtime/schedule/utils.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/admin.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/admin.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/callback.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from rest_framework.response import Response
 from django.utils.decorators import method_decorator
 from blueapps.account.decorators import login_exempt
 from apigw_manager.apigw.decorators import apigw_require
 
 from bk_plugin_framework.runtime.callback.api import parse_callback_token, callback
 
-logger = logging.getLogger("bk-plugin")
+logger = logging.getLogger("bk_plugin")
 
 
 @method_decorator(login_exempt, name="dispatch")
 @method_decorator(apigw_require, name="dispatch")
 class PluginCallback(APIView):
     authentication_classes = []  # csrf exempt
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/detail.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/detail.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/invoke.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/invoke.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from apigw_manager.apigw.decorators import apigw_require
 
 
 from bk_plugin_framework.hub import VersionHub
 from bk_plugin_framework.runtime.executor import BKPluginExecutor
 from bk_plugin_framework.services.bpf_service.api.serializers import StandardResponseSerializer
 
-logger = logging.getLogger("bk-plugin")
+logger = logging.getLogger("bk_plugin")
 
 
 class InvokeParamsSerializer(serializers.Serializer):
     inputs = serializers.DictField(help_text="插件调用参数", required=True)
     context = serializers.DictField(help_text="插件执行上下文", required=True)
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/logs.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/logs.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/meta.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/meta.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/plugin_api_dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from drf_yasg.utils import swagger_auto_schema
 
 from blueapps.account.decorators import login_exempt
 from apigw_manager.apigw.decorators import apigw_require
 
 from bk_plugin_framework.services.bpf_service.api.serializers import StandardResponseSerializer
 
-logger = logging.getLogger("bk-plugin")
+logger = logging.getLogger("bk_plugin")
 
 CUSTOM_REQUEST_HEADER_REGEX = re.compile("HTTP_BK_PLUGIN_*")
 
 
 class PluginAPIDispatchParamsSerializer(serializers.Serializer):
     url = serializers.CharField(help_text="数据接口 URL", required=True)
     method = serializers.CharField(help_text="调用方法", required=True)
```

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/schedule.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/schedule.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/apps.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/apps.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/data/api-resources.yml`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/management/commands/sync_plugin_apigw.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/middlewares.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/middlewares.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/migrations/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/bpf_service/urls.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/bpf_service/urls.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/management/commands/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/management/commands/rundebugserver.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/migrations/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/services/debug_panel/views.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/services/debug_panel/views.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/utils/__init__.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/utils/local.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/utils/local.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/utils/log.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/utils/log.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/bk_plugin_framework/utils/module_load.py` & `bk-plugin-framework-2.0.4/bk_plugin_framework/utils/module_load.py`

 * *Files identical despite different names*

### Comparing `bk-plugin-framework-2.0.3/pyproject.toml` & `bk-plugin-framework-2.0.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bk-plugin-framework"
-version = "2.0.3"
+version = "2.0.4"
 description = "bk plugin python framework"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.6.1,<4.0"
 pydantic = "^1.0"
```

### Comparing `bk-plugin-framework-2.0.3/setup.py` & `bk-plugin-framework-2.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ['apigw-manager[extra]>=1.0.6,<1.2.0',
  'bk-plugin-runtime==2.0.2',
  'pydantic>=1.0,<2.0',
  'werkzeug>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bk-plugin-framework',
-    'version': '2.0.3',
+    'version': '2.0.4',
     'description': 'bk plugin python framework',
     'long_description': None,
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bk-plugin-framework-2.0.3/PKG-INFO` & `bk-plugin-framework-2.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bk-plugin-framework
-Version: 2.0.3
+Version: 2.0.4
 Summary: bk plugin python framework
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

