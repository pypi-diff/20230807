# Comparing `tmp/mercury-2.3.1.tar.gz` & `tmp/mercury-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-2.3.1.tar", last modified: Mon Jun  5 11:39:20 2023, max compression
+gzip compressed data, was "mercury-2.3.2.tar", last modified: Mon Aug  7 09:59:44 2023, max compression
```

## Comparing `mercury-2.3.1.tar` & `mercury-2.3.2.tar`

### file list

```diff
@@ -1,212 +1,220 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.588888 mercury-2.3.1/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.3.1/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6016 2023-06-05 11:39:20.588888 mercury-2.3.1/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4326 2023-05-22 10:58:50.000000 mercury-2.3.1/README.md
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.556888 mercury-2.3.1/mercury/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-06-05 11:37:37.000000 mercury-2.3.1/mercury/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.556888 mercury-2.3.1/mercury/apps/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.560888 mercury-2.3.1/mercury/apps/accounts/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.1/mercury/apps/accounts/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.3.1/mercury/apps/accounts/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.3.1/mercury/apps/accounts/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.3.1/mercury/apps/accounts/fields.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.560888 mercury-2.3.1/mercury/apps/accounts/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/accounts/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.1/mercury/apps/accounts/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.3.1/mercury/apps/accounts/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.3.1/mercury/apps/accounts/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.3.1/mercury/apps/accounts/tasks.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.560888 mercury-2.3.1/mercury/apps/accounts/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.3.1/mercury/apps/accounts/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/accounts/tests/test_accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.3.1/mercury/apps/accounts/tests/test_invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/accounts/tests/test_secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-03-31 10:52:58.000000 mercury-2.3.1/mercury/apps/accounts/tests/test_sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/accounts/tests/test_subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2023-04-25 12:36:08.000000 mercury-2.3.1/mercury/apps/accounts/urls.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.560888 mercury-2.3.1/mercury/apps/accounts/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.3.1/mercury/apps/accounts/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.3.1/mercury/apps/accounts/views/accounts.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.3.1/mercury/apps/accounts/views/invitations.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.3.1/mercury/apps/accounts/views/permissions.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.3.1/mercury/apps/accounts/views/secrets.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6578 2023-05-16 15:07:21.000000 mercury-2.3.1/mercury/apps/accounts/views/sites.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/accounts/views/subscription.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      436 2023-03-24 08:45:58.000000 mercury-2.3.1/mercury/apps/accounts/views/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.560888 mercury-2.3.1/mercury/apps/nb/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/nb/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/nb/exporter.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4086 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/nb/nbrun.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.560888 mercury-2.3.1/mercury/apps/nb/tests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.3.1/mercury/apps/nb/tests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/nb/tests/test_nbrun.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.3.1/mercury/apps/nb/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/nb/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.564888 mercury-2.3.1/mercury/apps/nbworker/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/nbworker/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1950 2023-04-27 15:29:23.000000 mercury-2.3.1/mercury/apps/nbworker/__main__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17411 2023-04-12 08:48:16.000000 mercury-2.3.1/mercury/apps/nbworker/nb.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7485 2023-04-06 14:49:56.000000 mercury-2.3.1/mercury/apps/nbworker/rest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4864 2023-03-17 08:55:41.000000 mercury-2.3.1/mercury/apps/nbworker/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/nbworker/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2927 2023-04-20 13:08:01.000000 mercury-2.3.1/mercury/apps/nbworker/ws.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.568888 mercury-2.3.1/mercury/apps/notebooks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/notebooks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/notebooks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/notebooks/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.568888 mercury-2.3.1/mercury/apps/notebooks/management/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/notebooks/management/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.568888 mercury-2.3.1/mercury/apps/notebooks/management/commands/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/notebooks/management/commands/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.3.1/mercury/apps/notebooks/management/commands/add.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.3.1/mercury/apps/notebooks/management/commands/delete.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.3.1/mercury/apps/notebooks/management/commands/list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/notebooks/management/commands/watch.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.568888 mercury-2.3.1/mercury/apps/notebooks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/notebooks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/notebooks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.3.1/mercury/apps/notebooks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.3.1/mercury/apps/notebooks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.3.1/mercury/apps/notebooks/slides_themes.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11852 2023-05-22 13:27:15.000000 mercury-2.3.1/mercury/apps/notebooks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.3.1/mercury/apps/notebooks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.3.1/mercury/apps/notebooks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2023-04-27 15:18:53.000000 mercury-2.3.1/mercury/apps/notebooks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.568888 mercury-2.3.1/mercury/apps/storage/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/storage/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/storage/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/storage/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.568888 mercury-2.3.1/mercury/apps/storage/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/storage/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.3.1/mercury/apps/storage/migrations/0002_useruploadedfile.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/storage/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/storage/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.3.1/mercury/apps/storage/s3utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.3.1/mercury/apps/storage/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    11397 2023-05-22 12:14:16.000000 mercury-2.3.1/mercury/apps/storage/storage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.3.1/mercury/apps/storage/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2132 2023-03-29 09:56:45.000000 mercury-2.3.1/mercury/apps/storage/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.3.1/mercury/apps/storage/utils.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.572888 mercury-2.3.1/mercury/apps/storage/views/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.3.1/mercury/apps/storage/views/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-03-31 11:42:07.000000 mercury-2.3.1/mercury/apps/storage/views/dashboardfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.3.1/mercury/apps/storage/views/notebookfiles.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.3.1/mercury/apps/storage/views/workerfiles.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.572888 mercury-2.3.1/mercury/apps/tasks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/tasks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/tasks/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/tasks/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.3.1/mercury/apps/tasks/clean_service.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4021 2023-05-30 11:26:15.000000 mercury-2.3.1/mercury/apps/tasks/export_pdf.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/tasks/export_png.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.572888 mercury-2.3.1/mercury/apps/tasks/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/tasks/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/apps/tasks/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.3.1/mercury/apps/tasks/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/tasks/notify.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.3.1/mercury/apps/tasks/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.3.1/mercury/apps/tasks/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1335 2023-05-23 13:34:07.000000 mercury-2.3.1/mercury/apps/tasks/tasks_export.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/tasks/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1431 2023-04-25 12:37:36.000000 mercury-2.3.1/mercury/apps/tasks/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8714 2023-05-23 13:27:23.000000 mercury-2.3.1/mercury/apps/tasks/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.576888 mercury-2.3.1/mercury/apps/workers/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/workers/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/workers/admin.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/workers/apps.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.576888 mercury-2.3.1/mercury/apps/workers/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/workers/migrations/0001_initial.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/workers/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      798 2023-03-29 09:06:05.000000 mercury-2.3.1/mercury/apps/workers/models.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/workers/serializers.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/workers/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1076 2023-04-25 12:37:59.000000 mercury-2.3.1/mercury/apps/workers/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3913 2023-05-30 12:14:57.000000 mercury-2.3.1/mercury/apps/workers/views.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.576888 mercury-2.3.1/mercury/apps/ws/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/ws/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/ws/apps.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6162 2023-04-20 13:43:38.000000 mercury-2.3.1/mercury/apps/ws/client.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/ws/middleware.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.576888 mercury-2.3.1/mercury/apps/ws/migrations/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/apps/ws/migrations/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.3.1/mercury/apps/ws/routing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2495 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/ws/tasks.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-03-01 11:07:38.000000 mercury-2.3.1/mercury/apps/ws/tests.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5106 2023-04-06 13:49:54.000000 mercury-2.3.1/mercury/apps/ws/utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1754 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/apps/ws/worker.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.3.1/mercury/demo.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.576888 mercury-2.3.1/mercury/frontend-dist/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/asset-manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/favicon-old.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/favicon.ico
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/index.html
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/jupyter-additional.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/jupyter-syntax.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   580392 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/jupyter-theme-light.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/manifest.json
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/mercury_black_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/mercury_logo.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-06-05 11:39:03.000000 mercury-2.3.1/mercury/frontend-dist/robots.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.556888 mercury-2.3.1/mercury/frontend-dist/static/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.580888 mercury-2.3.1/mercury/frontend-dist/static/css/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3021 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5576 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.584888 mercury-2.3.1/mercury/frontend-dist/static/js/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/2.206848a5.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/2.206848a5.chunk.js.LICENSE.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)  4972965 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/2.206848a5.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    87736 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/main.9c1f23c5.chunk.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   267938 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/main.9c1f23c5.chunk.js.map
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.584888 mercury-2.3.1/mercury/frontend-dist/static/media/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
--rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/manage.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9259 2023-05-23 11:37:47.000000 mercury-2.3.1/mercury/mercury.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2023-04-25 12:41:47.000000 mercury-2.3.1/mercury/requirements.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.588888 mercury-2.3.1/mercury/server/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.3.1/mercury/server/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.3.1/mercury/server/asgi.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2771 2023-03-24 08:43:00.000000 mercury-2.3.1/mercury/server/celery.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.3.1/mercury/server/settings.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.3.1/mercury/server/urls.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.3.1/mercury/server/views.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.3.1/mercury/server/wsgi.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.588888 mercury-2.3.1/mercury/widgets/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.1/mercury/widgets/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2029 2023-05-23 08:29:51.000000 mercury-2.3.1/mercury/widgets/app.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.3.1/mercury/widgets/button.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.3.1/mercury/widgets/chat.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2140 2023-05-23 08:29:43.000000 mercury-2.3.1/mercury/widgets/checkbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.3.1/mercury/widgets/confetti.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.3.1/mercury/widgets/file.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.3.1/mercury/widgets/json.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6894 2023-04-07 10:30:37.000000 mercury-2.3.1/mercury/widgets/manager.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.3.1/mercury/widgets/md.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2703 2023-05-23 08:29:29.000000 mercury-2.3.1/mercury/widgets/multiselect.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.3.1/mercury/widgets/note.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3143 2023-05-29 10:16:14.000000 mercury-2.3.1/mercury/widgets/numberbox.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3029 2023-05-23 08:29:18.000000 mercury-2.3.1/mercury/widgets/numeric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.3.1/mercury/widgets/outputdir.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3038 2023-05-23 08:29:05.000000 mercury-2.3.1/mercury/widgets/range.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2416 2023-05-23 08:28:57.000000 mercury-2.3.1/mercury/widgets/select.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2962 2023-05-23 08:28:46.000000 mercury-2.3.1/mercury/widgets/slider.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.3.1/mercury/widgets/stop.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2052 2023-05-23 08:26:54.000000 mercury-2.3.1/mercury/widgets/text.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-05 11:39:20.556888 mercury-2.3.1/mercury.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6016 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6314 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury.egg-info/entry_points.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      489 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-06-05 11:39:20.000000 mercury-2.3.1/mercury.egg-info/top_level.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.3.1/pyproject.toml
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-06-05 11:39:20.588888 mercury-2.3.1/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2023-06-05 11:37:42.000000 mercury-2.3.1/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.787108 mercury-2.3.2/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      149 2022-04-19 12:37:24.000000 mercury-2.3.2/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10232 2023-08-07 09:59:44.787108 mercury-2.3.2/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8038 2023-06-19 11:13:10.000000 mercury-2.3.2/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       54 2023-08-07 09:58:34.000000 mercury-2.3.2/mercury/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/accounts/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.2/mercury/apps/accounts/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      459 2023-03-17 11:37:23.000000 mercury-2.3.2/mercury/apps/accounts/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2023-03-01 11:11:00.000000 mercury-2.3.2/mercury/apps/accounts/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      801 2023-03-01 11:11:00.000000 mercury-2.3.2/mercury/apps/accounts/fields.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/accounts/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9132 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-01 11:11:00.000000 mercury-2.3.2/mercury/apps/accounts/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4715 2023-03-28 08:49:03.000000 mercury-2.3.2/mercury/apps/accounts/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2086 2023-04-06 13:33:42.000000 mercury-2.3.2/mercury/apps/accounts/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2937 2023-03-27 12:26:01.000000 mercury-2.3.2/mercury/apps/accounts/tasks.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/accounts/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-16 13:27:44.000000 mercury-2.3.2/mercury/apps/accounts/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7289 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/accounts/tests/test_accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5543 2023-03-31 10:36:11.000000 mercury-2.3.2/mercury/apps/accounts/tests/test_invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6078 2023-04-06 13:49:54.000000 mercury-2.3.2/mercury/apps/accounts/tests/test_secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11402 2023-06-22 08:59:21.000000 mercury-2.3.2/mercury/apps/accounts/tests/test_sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3426 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/accounts/tests/test_subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2645 2023-04-25 12:36:08.000000 mercury-2.3.2/mercury/apps/accounts/urls.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/accounts/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-17 08:20:29.000000 mercury-2.3.2/mercury/apps/accounts/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2006 2023-03-27 08:34:35.000000 mercury-2.3.2/mercury/apps/accounts/views/accounts.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4308 2023-03-31 10:36:11.000000 mercury-2.3.2/mercury/apps/accounts/views/invitations.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      789 2023-03-24 08:45:58.000000 mercury-2.3.2/mercury/apps/accounts/views/permissions.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2922 2023-04-06 14:49:43.000000 mercury-2.3.2/mercury/apps/accounts/views/secrets.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7505 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/accounts/views/sites.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4152 2023-07-05 10:28:41.000000 mercury-2.3.2/mercury/apps/accounts/views/subscription.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      854 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/accounts/views/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/nb/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/nb/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5845 2023-04-06 13:49:54.000000 mercury-2.3.2/mercury/apps/nb/exporter.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4522 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/nb/nbrun.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/nb/tests/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-04-05 08:19:32.000000 mercury-2.3.2/mercury/apps/nb/tests/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1252 2023-07-18 10:35:22.000000 mercury-2.3.2/mercury/apps/nb/tests/test_nbrun.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1265 2023-03-17 12:41:34.000000 mercury-2.3.2/mercury/apps/nb/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      403 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/nb/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/nbworker/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/nbworker/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1698 2023-06-28 11:54:57.000000 mercury-2.3.2/mercury/apps/nbworker/__main__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17517 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/nbworker/nb.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8896 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/nbworker/rest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4898 2023-06-28 11:59:58.000000 mercury-2.3.2/mercury/apps/nbworker/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/nbworker/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2862 2023-06-28 11:55:41.000000 mercury-2.3.2/mercury/apps/nbworker/ws.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/notebooks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/notebooks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      277 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/notebooks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      155 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/notebooks/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/notebooks/management/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/notebooks/management/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/notebooks/management/commands/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/notebooks/management/commands/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1279 2022-03-09 11:06:47.000000 mercury-2.3.2/mercury/apps/notebooks/management/commands/add.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      864 2022-03-09 11:06:47.000000 mercury-2.3.2/mercury/apps/notebooks/management/commands/delete.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2022-03-09 11:06:47.000000 mercury-2.3.2/mercury/apps/notebooks/management/commands/list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3702 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/notebooks/management/commands/watch.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/apps/notebooks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2300 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/notebooks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/notebooks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1067 2023-03-27 08:29:11.000000 mercury-2.3.2/mercury/apps/notebooks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      617 2023-03-17 11:38:01.000000 mercury-2.3.2/mercury/apps/notebooks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4093 2022-05-18 10:19:32.000000 mercury-2.3.2/mercury/apps/notebooks/slides_themes.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11853 2023-06-22 08:55:52.000000 mercury-2.3.2/mercury/apps/notebooks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-03-01 11:11:00.000000 mercury-2.3.2/mercury/apps/notebooks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      582 2023-04-25 12:40:05.000000 mercury-2.3.2/mercury/apps/notebooks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3798 2023-04-27 15:18:53.000000 mercury-2.3.2/mercury/apps/notebooks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/storage/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/storage/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/storage/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/storage/apps.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/storage/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2949 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/storage/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1404 2023-03-31 09:54:03.000000 mercury-2.3.2/mercury/apps/storage/migrations/0002_useruploadedfile.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/storage/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1787 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/storage/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3540 2023-03-31 09:54:03.000000 mercury-2.3.2/mercury/apps/storage/s3utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-03-31 14:19:15.000000 mercury-2.3.2/mercury/apps/storage/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11436 2023-06-28 11:57:30.000000 mercury-2.3.2/mercury/apps/storage/storage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3158 2023-03-17 08:55:41.000000 mercury-2.3.2/mercury/apps/storage/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2483 2023-08-01 14:10:06.000000 mercury-2.3.2/mercury/apps/storage/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      445 2023-03-31 09:54:03.000000 mercury-2.3.2/mercury/apps/storage/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/storage/views/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-31 12:45:08.000000 mercury-2.3.2/mercury/apps/storage/views/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6182 2023-07-22 09:24:04.000000 mercury-2.3.2/mercury/apps/storage/views/dashboardfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4935 2023-03-31 11:42:07.000000 mercury-2.3.2/mercury/apps/storage/views/notebookfiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3495 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/storage/views/stylefiles.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3737 2023-03-31 11:42:07.000000 mercury-2.3.2/mercury/apps/storage/views/workerfiles.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/tasks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/tasks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/tasks/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      153 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/tasks/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      412 2022-03-09 11:06:47.000000 mercury-2.3.2/mercury/apps/tasks/clean_service.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4018 2023-06-22 08:55:52.000000 mercury-2.3.2/mercury/apps/tasks/export_pdf.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3805 2023-04-06 13:49:54.000000 mercury-2.3.2/mercury/apps/tasks/export_png.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/tasks/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1328 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/apps/tasks/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      762 2022-05-18 10:19:32.000000 mercury-2.3.2/mercury/apps/tasks/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3659 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/tasks/notify.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      433 2022-03-09 11:06:47.000000 mercury-2.3.2/mercury/apps/tasks/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15223 2023-02-23 14:52:12.000000 mercury-2.3.2/mercury/apps/tasks/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1335 2023-05-23 13:34:07.000000 mercury-2.3.2/mercury/apps/tasks/tasks_export.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      571 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/tasks/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1431 2023-04-25 12:37:36.000000 mercury-2.3.2/mercury/apps/tasks/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8714 2023-05-23 13:27:23.000000 mercury-2.3.2/mercury/apps/tasks/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/workers/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/workers/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       63 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/workers/admin.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      151 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/workers/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      532 2023-07-18 10:35:22.000000 mercury-2.3.2/mercury/apps/workers/constants.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/workers/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1286 2023-03-29 09:06:05.000000 mercury-2.3.2/mercury/apps/workers/migrations/0001_initial.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2023-06-20 12:58:36.000000 mercury-2.3.2/mercury/apps/workers/migrations/0002_machine.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2842 2023-06-22 09:33:58.000000 mercury-2.3.2/mercury/apps/workers/migrations/0003_worker_run_by_workersession.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/workers/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1832 2023-06-28 12:00:54.000000 mercury-2.3.2/mercury/apps/workers/models.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      296 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/workers/serializers.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6163 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/workers/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1360 2023-08-02 15:55:58.000000 mercury-2.3.2/mercury/apps/workers/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      469 2023-06-28 11:58:17.000000 mercury-2.3.2/mercury/apps/workers/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6912 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/apps/workers/views.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/ws/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/ws/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      141 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/ws/apps.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6248 2023-06-26 08:29:00.000000 mercury-2.3.2/mercury/apps/ws/client.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      947 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/apps/ws/middleware.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/apps/ws/migrations/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/apps/ws/migrations/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      386 2023-02-28 13:59:46.000000 mercury-2.3.2/mercury/apps/ws/routing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2654 2023-06-28 12:03:38.000000 mercury-2.3.2/mercury/apps/ws/tasks.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      137 2023-06-21 07:54:00.000000 mercury-2.3.2/mercury/apps/ws/tests.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5658 2023-07-18 10:35:22.000000 mercury-2.3.2/mercury/apps/ws/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2343 2023-06-28 12:04:52.000000 mercury-2.3.2/mercury/apps/ws/worker.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7191 2023-03-31 14:11:10.000000 mercury-2.3.2/mercury/demo.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.779108 mercury-2.3.2/mercury/frontend-dist/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1158 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/asset-manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15406 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/favicon-old.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15086 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/favicon.ico
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3086 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/index.html
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    17406 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/jupyter-additional.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4539 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/jupyter-syntax.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   580392 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/jupyter-theme-light.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      324 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/manifest.json
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6237 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/mercury_black_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6997 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/mercury_logo.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       67 2023-08-07 09:59:29.000000 mercury-2.3.2/mercury/frontend-dist/robots.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury/frontend-dist/static/
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.783108 mercury-2.3.2/mercury/frontend-dist/static/css/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   229115 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   612316 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3071 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5632 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.787108 mercury-2.3.2/mercury/frontend-dist/static/js/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  1311795 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/2.20c8cb43.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3383 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/2.20c8cb43.chunk.js.LICENSE.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)  4972965 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/2.20c8cb43.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    89648 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/main.55ba4c52.chunk.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   274882 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/main.55ba4c52.chunk.js.map
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1557 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8276 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/js/runtime-main.248907bc.js.map
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.787108 mercury-2.3.2/mercury/frontend-dist/static/media/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165548 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/media/fontawesome-webfont.1e59d233.ttf
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    77160 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/media/fontawesome-webfont.20fd1704.woff2
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   165742 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/media/fontawesome-webfont.8b43027f.eot
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   444379 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/media/fontawesome-webfont.c1e38fd9.svg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    98024 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury/frontend-dist/static/media/fontawesome-webfont.f691f37e.woff
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      684 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/manage.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9485 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      545 2023-04-25 12:41:47.000000 mercury-2.3.2/mercury/requirements.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.787108 mercury-2.3.2/mercury/server/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       68 2022-03-09 11:04:20.000000 mercury-2.3.2/mercury/server/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      837 2023-03-14 07:49:44.000000 mercury-2.3.2/mercury/server/asgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3230 2023-06-22 11:55:26.000000 mercury-2.3.2/mercury/server/celery.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9844 2023-04-05 13:16:51.000000 mercury-2.3.2/mercury/server/settings.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1575 2023-04-25 12:38:18.000000 mercury-2.3.2/mercury/server/urls.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1645 2023-03-01 12:07:40.000000 mercury-2.3.2/mercury/server/views.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      405 2022-05-18 11:03:41.000000 mercury-2.3.2/mercury/server/wsgi.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2461 2023-06-21 11:57:21.000000 mercury-2.3.2/mercury/start_instance.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.787108 mercury-2.3.2/mercury/widgets/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-02-13 14:05:12.000000 mercury-2.3.2/mercury/widgets/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2150 2023-07-18 10:35:22.000000 mercury-2.3.2/mercury/widgets/app.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2294 2023-04-07 10:30:37.000000 mercury-2.3.2/mercury/widgets/button.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      826 2023-04-07 10:43:02.000000 mercury-2.3.2/mercury/widgets/chat.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2140 2023-05-23 08:29:43.000000 mercury-2.3.2/mercury/widgets/checkbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      408 2023-04-07 10:32:14.000000 mercury-2.3.2/mercury/widgets/confetti.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3393 2023-04-07 10:30:37.000000 mercury-2.3.2/mercury/widgets/file.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      850 2023-07-14 09:38:16.000000 mercury-2.3.2/mercury/widgets/in_mercury.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4828 2023-02-21 07:28:26.000000 mercury-2.3.2/mercury/widgets/json.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6988 2023-07-17 12:16:57.000000 mercury-2.3.2/mercury/widgets/manager.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      104 2023-02-21 07:28:26.000000 mercury-2.3.2/mercury/widgets/md.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2703 2023-05-23 08:29:29.000000 mercury-2.3.2/mercury/widgets/multiselect.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1219 2023-02-21 07:48:36.000000 mercury-2.3.2/mercury/widgets/note.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3143 2023-05-29 10:16:14.000000 mercury-2.3.2/mercury/widgets/numberbox.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3029 2023-05-23 08:29:18.000000 mercury-2.3.2/mercury/widgets/numeric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1255 2023-02-21 07:48:36.000000 mercury-2.3.2/mercury/widgets/outputdir.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3360 2023-07-17 12:20:30.000000 mercury-2.3.2/mercury/widgets/range.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2416 2023-05-23 08:28:57.000000 mercury-2.3.2/mercury/widgets/select.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3475 2023-07-17 12:20:06.000000 mercury-2.3.2/mercury/widgets/slider.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      222 2023-02-21 07:28:26.000000 mercury-2.3.2/mercury/widgets/stop.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2052 2023-05-23 08:26:54.000000 mercury-2.3.2/mercury/widgets/text.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      815 2023-08-07 09:22:06.000000 mercury-2.3.2/mercury/widgets/user.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-08-07 09:59:44.775108 mercury-2.3.2/mercury.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10232 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6615 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       50 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury.egg-info/entry_points.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      489 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        8 2023-08-07 09:59:44.000000 mercury-2.3.2/mercury.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      106 2022-03-09 11:04:20.000000 mercury-2.3.2/pyproject.toml
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-08-07 09:59:44.787108 mercury-2.3.2/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1386 2023-08-07 09:58:18.000000 mercury-2.3.2/setup.py
```

### Comparing `mercury-2.3.1/PKG-INFO` & `mercury-2.3.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,191 @@
-Metadata-Version: 2.1
-Name: mercury
-Version: 2.3.1
-Summary: Turn Jupyter Notebook to Web App and share with non-technical users
-Home-page: https://github.com/mljar/mercury
-Author: MLJAR Sp. z o.o.
-Maintainer: MLJAR Sp. z o.o.
-Maintainer-email: contact@mljar.com
-License: UNKNOWN
-Description: 
-        
-        <p align="center">
-          <img 
-            alt="Mercury convert Jupyter Notebook to Web App"
-            src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/mercury-og.png" width="100%" />  
-        </p>
-        
-        [![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
-        [![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
-        [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
-        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
-        
-        # Build Web Apps in Jupyter Notebook
-        
-        Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
-        
-        You can build with Mercury:
-        - Turn your notebook into beautiful [Web Apps](https://runmercury.com/tutorials/web-app-python-jupyter-notebook/),
-        - Create interactive [Presentations](https://runmercury.com/tutorials/presentation-python-jupyter-notebook/) with widgets, you can recompute slides during the show,
-        - Share notebooks as static [Websites](https://runmercury.com/tutorials/website-python-jupyter-notebook/),
-        
-        - Build data-rich [Dashboards](https://runmercury.com/tutorials/dashboard-python-jupyter-notebook/) with widgets,
-        - Create [Reports](https://runmercury.com/tutorials/report-python-jupyter-notebook/) with PDF exports, automatic scheduling, and email notifications (coming soon),
-        - Serve Python notebooks as [REST API](https://runmercury.com/tutorials/rest-api-python-jupyter-notebook/) endpoints (coming soon).
-        
-        Mercury features:
-        - add widgets with Python code - no frontend experience needed!
-        - hide or show notebook's code,
-        - export executed notebook to PDF or HTML,
-        - share muplitple notebooks - no limits!
-        - embed notebook on any website,
-        - easy file upload and download from the notebook,
-        - add authentication to notebooks (coming soon),
-        - schedule automatic notebook execution (coming soon).
-        
-        ## Example
-        
-        Simple code example that creates a widget and displays its value. You can interact with a widget in the Jupyter Notebook. Its value will be updated. However, to see the update in other cells you need to **manually execute** them.
-        
-        Import package:
-        ```python
-        import mercury as mr
-        ```
-        
-        Create a [`Text`](https://runmercury.com/docs/input-widgets/text/) widget:
-        ```python
-        name = mr.Text(value="Piotr", label="What is your name?")
-        ```
-        
-        Print widget value:
-        ```python
-        print(f"Hello {name.value}")
-        ```
-        
-        #### Code in Jupyter Notebook
-        
-        <p align="center">
-        <kbd>
-        <img 
-            alt="Web App from Notebook"
-            src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/hello-world-notebook-ola.png"  />  
-        </kbd>
-        </p>
-        
-        #### Mercury App
-        
-        Use Mercury to run notebook as web application. **Cells are automatically re-executed** after widget change. Mercury re-executes only cells with widget definition and below it. In the example, cells 2 and 3 are re-executed after widget update. 
-        
-        <p align="center">
-        <kbd>
-        <img 
-            alt="Web App from Notebook"
-            src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/hello-world-app-ola.gif"  />  
-           </kbd>
-        </p>
-        
-        
-        ## Documentation
-        
-        📚 Read more about Mercury on [RunMercury.com](https://RunMercury.com).
-        
-        ## Installation
-        
-        *Compatible with Python 3.7 and higher.*
-        
-        Install with `pip`:
-        
-        ```
-        pip install mercury
-        ```
-        
-        Install with `conda`:
-        
-        ```
-        conda install -c conda-forge mercury
-        ```
-        
-        
-        ## Demo
-        
-        Run Mercury with demo notebooks.
-        
-        ```
-        mercury run demo
-        ```
-        
-        Please check [127.0.0.1:8000](http://127.0.0.1:8000) to see demo notebooks.
-        
-        
-        ## Mercury with your notebooks
-        
-        To run Mercury with your notebook, please execute the following:
-        
-        ```
-        mercury run
-        ```
-        
-        The command should be run in the same directory as notebooks. You can change code in Jupyter Notebook, and Mercury will **instantly** update web app.
-        
-        
-        ## Mercury License
-        
-        Mercury is released with AGPL v3 license.
-        
-        Looking for dedicated support, a commercial-friendly license, and more features? The Mercury Pro is for you. Please see the details at [our website](https://mljar.com/pricing).
-        
-        
-        
-Platform: UNKNOWN
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+
+
+<p align="center">
+  <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/main.png#gh-light-mode-only" width="100%" />  
+</p>
+<p align="center">
+  <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/main_black.png#gh-dark-mode-only" width="100%" />  
+</p>
+
+[![Tests](https://github.com/mljar/mercury/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mercury/actions/workflows/run-tests.yml)
+[![PyPI version](https://badge.fury.io/py/mercury.svg)](https://badge.fury.io/py/mercury)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mercury.svg)](https://pypi.python.org/pypi/mercury/)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-mercury/badges/license.svg)](https://anaconda.org/conda-forge/mljar-mercury)
+
+# Build Web Apps in Jupyter Notebook
+
+Mercury allows you to add interactive widgets in Python notebooks, so you can share notebooks as web applications. Forget about rewriting notebooks to web frameworks just to share your results. Mercury offers a set of widgets with simple re-execution of cells.
+
+You can build with Mercury:
+- Turn your notebook into beautiful [Web Apps](https://runmercury.com/tutorials/web-app-python-jupyter-notebook/),
+- Create interactive [Presentations](https://runmercury.com/tutorials/presentation-python-jupyter-notebook/) with widgets, you can recompute slides during the show,
+- Share notebooks as static [Websites](https://runmercury.com/tutorials/website-python-jupyter-notebook/),
+
+- Build data-rich [Dashboards](https://runmercury.com/tutorials/dashboard-python-jupyter-notebook/) with widgets,
+- Create [Reports](https://runmercury.com/tutorials/report-python-jupyter-notebook/) with PDF exports, automatic scheduling, and email notifications (coming soon),
+- Serve Python notebooks as [REST API](https://runmercury.com/tutorials/rest-api-python-jupyter-notebook/) endpoints (coming soon).
+
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/What_to_build.png#gh-light-mode-only" width="100%" />  
+</p>
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/What_to_build_black.png#gh-dark-mode-only" width="100%" />  
+</p>
+
+Mercury features:
+- add widgets with Python code - no frontend experience needed!
+- hide or show the notebook's code,
+- export executed notebook to PDF or HTML,
+- share multiple notebooks - no limits!
+- embed notebook on any website,
+- easy file upload and download from the notebook,
+- add authentication to notebooks (coming soon),
+- schedule automatic notebook execution (coming soon).
+
+## Widgets
+
+Mercury provides multiple widgets. There are 3 types of widgets:
+- [Input widgets](https://runmercury.com/docs/input-widgets/) are components that will appear in the sidebar when running the notebook in Mercury. They can be used to provide user input or trigger action in the notebook.
+- [Output widgets](https://runmercury.com/docs/output-widgets/) help present notebook results to the user and control execution flow.
+- [Custom Widgets](https://runmercury.com/docs/custom-widgets/) - you can use many custom widgets, for example, PyDeck, and Pivot Tables.
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets3.png#gh-light-mode-only" width="100%" />  
+</p>
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/widgets_black.png#gh-dark-mode-only" width="100%" />  
+</p>
+## Integrations
+ 
+Mercury works with virtually every Python package!
+Among the most important are machine learning libraries such as Scikit-Learn, Pandas, and Seaborn or visualization libraries: Plotly, matplotlib, Vega-Altair, and Ipyvizzu.
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Integrations.png#gh-light-mode-only" width="100%" />  
+</p>
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Integrations_black.png#gh-dark-mode-only" width="100%" />  
+</p>
+
+## Example
+
+Simple code example that creates a widget and displays its value. You can interact with a widget in the Jupyter Notebook. Its value will be updated. However, to see the update in other cells you need to **manually execute** them.
+
+Import package:
+```python
+import mercury as mr
+```
+
+Create a [`Text`](https://runmercury.com/docs/input-widgets/text/) widget:
+```python
+name = mr.Text(value="Piotr", label="What is your name?")
+```
+
+Print widget value:
+```python
+print(f"Hello {name.value}")
+```
+
+#### Code in Jupyter Notebook
+
+<p align="center">
+<kbd>
+<img 
+    alt="Web App from Notebook"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/hello-world-notebook-ola.png"  />  
+</kbd>
+</p>
+
+#### Mercury App
+
+Use Mercury to run notebook as web application. **Cells are automatically re-executed** after widget change. Mercury re-executes only cells with widget definition and below it. In the example, cells 2 and 3 are re-executed after widget update. 
+
+<p align="center">
+<kbd>
+<img 
+    alt="Web App from Notebook"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/hello-world-app-ola.gif"  />  
+   </kbd>
+</p>
+
+
+## Documentation
+
+📚 Read more about Mercury on [RunMercury.com](https://RunMercury.com).
+
+## Installation
+
+*Compatible with Python 3.7 and higher.*
+
+Install with `pip`:
+
+```
+pip install mercury
+```
+
+Install with `conda`:
+
+```
+conda install -c conda-forge mercury
+```
+
+
+## Demo
+
+Run Mercury with demo notebooks.
+
+```
+mercury run demo
+```
+
+Please check [127.0.0.1:8000](http://127.0.0.1:8000) to see demo notebooks.
+
+## Deployment
+
+You have several options to deploy the notebook. You can use the self-hosted option where you use [docker-compose](https://runmercury.com/docs/docker-compose/) on a VPS machine or use ngrok. There's also a possibility to use [Hugging Face Spaces](https://runmercury.com/docs/hugging-face/).
+
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/jupyter-notebook-hugging-face.gif" width="100%" />  
+</p>
+
+Another option is a Self-hosted commercial where you get access to the deployment dashboard where you manage notebooks and user access. In addition, you have access to user analytics; you can freely customize the style of your application. You benefit from private forks and email support.
+
+The third option is to use [Mercury Cloud](https://runmercury.com/docs/cloud/). It's the easiest way to share notebooks online. You will be able to create a website with a few clicks.
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Deployment.png#gh-light-mode-only" width="100%" />  
+</p>
+ <img 
+    alt="Mercury convert Jupyter Notebook to Web App"
+    src="https://raw.githubusercontent.com/mljar/visual-identity/main/mercury/readme/Deployment_black.png#gh-dark-mode-only" width="100%" />  
+</p>
+
+
+## Mercury with your notebooks
+
+To run Mercury with your notebook, please execute the following:
+
+```
+mercury run
+```
+
+The command should be run in the same directory as notebooks. You can change code in Jupyter Notebook, and Mercury will **instantly** update web app.
+
+
+
+## Mercury License
+
+Mercury is released with AGPL v3 license.
+
+Looking for dedicated support, a commercial-friendly license, and more features? The Mercury Pro is for you. Please see the details at [our website](https://runmercury.com/pricing/).
+
+
```

### Comparing `mercury-2.3.1/mercury/apps/accounts/fields.py` & `mercury-2.3.2/mercury/apps/accounts/fields.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/migrations/0001_initial.py` & `mercury-2.3.2/mercury/apps/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/models.py` & `mercury-2.3.2/mercury/apps/accounts/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/serializers.py` & `mercury-2.3.2/mercury/apps/accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/tasks.py` & `mercury-2.3.2/mercury/apps/accounts/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/tests/test_accounts.py` & `mercury-2.3.2/mercury/apps/accounts/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/tests/test_invitations.py` & `mercury-2.3.2/mercury/apps/accounts/tests/test_invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/tests/test_secrets.py` & `mercury-2.3.2/mercury/apps/accounts/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/tests/test_sites.py` & `mercury-2.3.2/mercury/apps/accounts/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/tests/test_subscription.py` & `mercury-2.3.2/mercury/apps/accounts/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/urls.py` & `mercury-2.3.2/mercury/apps/accounts/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/views/accounts.py` & `mercury-2.3.2/mercury/apps/accounts/views/accounts.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/views/invitations.py` & `mercury-2.3.2/mercury/apps/accounts/views/invitations.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/views/permissions.py` & `mercury-2.3.2/mercury/apps/accounts/views/permissions.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/views/secrets.py` & `mercury-2.3.2/mercury/apps/accounts/views/secrets.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/accounts/views/sites.py` & `mercury-2.3.2/mercury/apps/accounts/views/sites.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,38 @@
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.serializers import ValidationError
 
 from apps.accounts.models import Membership, Site
 from apps.accounts.serializers import SiteSerializer
 from apps.accounts.tasks import task_init_site
-from apps.accounts.views.utils import get_slug, is_cloud_version
-from apps.accounts.views.permissions import HasEditRights
+from apps.accounts.views.utils import (
+    get_slug, 
+    is_cloud_version,
+    PLAN_KEY,
+    PLAN_STARTER,
+    PLAN_PRO,
+    PLAN_BUSINESS
+)
 
-PLAN_KEY = "plan"
-PLAN_STARTER = "starter"
-PLAN_PRO = "pro"
-PLAN_BUSINESS = "business"
+from apps.accounts.views.permissions import HasEditRights
 
 FORBIDDEN_SLUGS = [
     "mercury",
     "dashboard",
     "report",
     "mljar",
     "cloud",
     "api",
     "python",
     "backend",
     "frontend",
     "www",
     "app",
+    "blog",
 ]
 
 
 def get_plan(user):
     info = json.loads(user.profile.info)
     user_plan = info.get(PLAN_KEY, PLAN_STARTER)
     if user_plan not in [PLAN_STARTER, PLAN_PRO, PLAN_BUSINESS]:
@@ -71,15 +75,17 @@
 
     def create(self, request, *args, **kwargs):
         # check number of allowed sites
         if Site.objects.filter(created_by=request.user).count() >= max_number_of_sites(
             request.user
         ):
             return Response(
-                {"msg": "Sites limit reached. Please change subsription plan"},
+                {
+                    "msg": "Sorry, you reached Sites limit. Please upgrade subscription plan"
+                },
                 status=status.HTTP_403_FORBIDDEN,
             )
         proposed_slug = get_slug(
             request.data.get("slug", ""), request.data.get("title", "")
         )
         if proposed_slug in FORBIDDEN_SLUGS:
             return Response(
@@ -88,14 +94,25 @@
             )
         if Site.objects.filter(slug=proposed_slug):
             return Response(
                 {"msg": "Please change site subdomain, current value is not unique"},
                 status=status.HTTP_403_FORBIDDEN,
             )
 
+        if is_cloud_version():
+            proposed_share = request.data.get("share", "")
+            user_plan = get_plan(self.request.user)
+            if user_plan == PLAN_STARTER and proposed_share == "PRIVATE":
+                return Response(
+                    {
+                        "msg": "Sorry, you can't create PRIVATE Site. Please uprgade subscription plan"
+                    },
+                    status=status.HTTP_403_FORBIDDEN,
+                )
+
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         self.perform_create(serializer)
         headers = self.get_success_headers(serializer.data)
         return Response(
             serializer.data, status=status.HTTP_201_CREATED, headers=headers
         )
@@ -117,14 +134,23 @@
         # lets check slug if we update it
         new_slug = self.request.data.get("slug")
 
         if new_slug is not None:
             new_slug = get_slug(new_slug, updated_instance.title)
             if new_slug in FORBIDDEN_SLUGS:
                 raise ValidationError(f"You cant use {new_slug} as a subdomain")
+
+            if is_cloud_version():
+                proposed_share = self.request.data.get("share", "")
+                user_plan = get_plan(self.request.user)
+                if user_plan == PLAN_STARTER and proposed_share == "PRIVATE":
+                    raise ValidationError(
+                        f"Sorry, you can't create PRIVATE Site. Please uprgade subscription plan"
+                    )
+
             updated_instance.slug = new_slug
             updated_instance.save()
 
     def destroy(self, request, *args, **kwargs):
         """Only owner can delete object"""
         try:
             instance = self.get_object()
```

### Comparing `mercury-2.3.1/mercury/apps/accounts/views/subscription.py` & `mercury-2.3.2/mercury/apps/accounts/views/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from rest_framework import permissions, status
 from rest_framework.response import Response
 from rest_framework.views import APIView
 from rest_framework.serializers import ValidationError
 
 from apps.accounts.serializers import UserSerializer
 
-MERCURY_CLOUD_PRO_ID = 820856
-MERCURY_CLOUD_BUSINESS_ID = 820858
+MERCURY_CLOUD_PRO_ID = 839780
+MERCURY_CLOUD_BUSINESS_ID = 839783
 
 PADDLE_VENDOR_ID = os.environ.get("PADDLE_VENDOR_ID")
 PADDLE_API_KEY = os.environ.get("PADDLE_API_KEY")
 
 
 class SubscriptionView(APIView):
     permission_classes = [permissions.IsAuthenticated]
```

### Comparing `mercury-2.3.1/mercury/apps/nb/exporter.py` & `mercury-2.3.2/mercury/apps/nb/exporter.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/nb/nbrun.py` & `mercury-2.3.2/mercury/apps/nb/nbrun.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,23 +20,31 @@
 class NbRun:
     def __init__(
         self,
         show_code=False,
         show_prompt=False,
         is_presentation=False,
         reveal_theme="white",
+        stop_on_error=False,
+        user_info=None
     ):
         self.exporter = Exporter(show_code, show_prompt, is_presentation, reveal_theme)
         self.shell = CaptureShell()
         try:
             self.shell.enable_matplotlib("inline")
         except Exception as e:
             pass
-        self.shell.run("from mercury import WidgetsManager")
-        self.shell.run("import os\nos.environ['RUN_MERCURY']='1'")
+        init_code = "from mercury import WidgetsManager\nimport os\nos.environ['RUN_MERCURY']='1'\n"
+        if user_info is not None:
+            init_code += f"os.environ['MERCURY_USER_INFO']='{user_info}'"
+        self.shell.run(init_code)
+        self.stop_on_error = stop_on_error
+
+    def set_stop_on_error(self, new_stop_on_error):
+        self.stop_on_error = new_stop_on_error
 
     def set_show_code(self, new_show_code):
         self.exporter.set_show_code(new_show_code)
 
     def set_show_code_and_prompt(self, new_show_code, new_show_prompt):
         self.exporter.set_show_prompt(new_show_prompt)
         self.exporter.set_show_code(new_show_code)
@@ -66,14 +74,17 @@
 
             try:
                 for output in cell.outputs:
                     if output.get(
                         "output_type", ""
                     ) == "error" and "StopExecution" in output.get("ename", ""):
                         return False
+                    if self.stop_on_error and output.get("output_type", "") == "error":
+                        return False
+
             except Exception as e:
                 pass
 
         return True
 
     def run_notebook(self, nb, start=0):
         #
```

### Comparing `mercury-2.3.1/mercury/apps/nb/tests.py` & `mercury-2.3.2/mercury/apps/nb/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/nbworker/__main__.py` & `mercury-2.3.2/mercury/apps/nbworker/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,28 @@
-import json
 import os
-import queue
 import signal
 import sys
-import threading
 import time
-import traceback
-from datetime import datetime, timedelta
-
-import websocket
-from django.utils.timezone import make_aware
+import logging
 
 CURRENT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 BACKEND_DIR = os.path.join(CURRENT_DIR, "..")
 sys.path.insert(0, BACKEND_DIR)
 
-os.environ.setdefault("DJANGO_SETTINGS_MODULE", "server.settings")
-import django
-
-django.setup()
-
-
-import logging
-
 LOG_LEVEL = (
     logging.ERROR if os.environ.get("MERCURY_VERBOSE", "0") == "0" else logging.DEBUG
 )
 
 logging.basicConfig(
     # filename="nbworker.log", filemode="w",
     format="NB %(asctime)s %(message)s",
     level=LOG_LEVEL,
 )
 log = logging.getLogger(__name__)
-logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
+logging.getLogger("matplotlib.font_manager").setLevel(logging.ERROR)
 
 from apps.nbworker.nb import NBWorker
 from apps.nbworker.rest import RESTClient
 from apps.nbworker.utils import stop_event
 
 if len(sys.argv) != 5:
     log.error("Wrong number of input parameters")
@@ -46,16 +31,19 @@
 notebook_id = int(sys.argv[1])
 session_id = sys.argv[2]
 worker_id = int(sys.argv[3])
 server_url = sys.argv[4]
 
 
 if os.environ.get("MERCURY_SERVER_URL") is None:
-    os.environ["MERCURY_SERVER_URL"] = server_url.replace("ws://", "http://").replace("wss://", "https://")
-    
+    os.environ["MERCURY_SERVER_URL"] = server_url.replace("ws://", "http://").replace(
+        "wss://", "https://"
+    )
+
+
 def signal_handler(signal, frame):
     global stop_event
     log.debug("\nBye bye!")
     stop_event.set()
     RESTClient.delete_worker_in_db(session_id, worker_id, notebook_id)
     sys.exit(1)
```

### Comparing `mercury-2.3.1/mercury/apps/nbworker/nb.py` & `mercury-2.3.2/mercury/apps/nbworker/nb.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from datetime import datetime
 
 from execnb.nbio import nb2dict, read_nb
 
 from apps.nb.nbrun import NbRun
 from apps.nbworker.utils import Purpose, stop_event
 from apps.nbworker.ws import WSClient
-from apps.workers.models import WorkerState
+from apps.workers.constants import WorkerState
 from apps.ws.utils import parse_params
+from apps.accounts.views.utils import get_idle_time, get_max_run_time
 from widgets.manager import WidgetsManager
 
 log = logging.getLogger(__name__)
 
 
 class NBWorker(WSClient):
     def __init__(self, ws_address, notebook_id, session_id, worker_id):
@@ -26,20 +27,16 @@
 
         self.prev_nb = None
         self.prev_widgets = {}
         self.prev_body = ""
         self.prev_update_time = None
         self.prev_md5 = None
         self.start_time = time.time()
-        self.max_idle_time = int(
-            os.environ.get("MAX_IDLE_TIME", 12 * 60 * 60)
-        )  # default idle after 12 hours
-        self.max_run_time = int(
-            os.environ.get("MAX_RUN_TIME", 24 * 60 * 60)
-        )  # default max run time is 24 hours
+        self.max_idle_time = get_idle_time(self.owner)
+        self.max_run_time = get_max_run_time(self.owner)
         self.last_execution_time = time.time()
         self.start_time = time.time()
 
         # monitor notebook file updates if running locally
         if "127.0.0.1" in ws_address:
             threading.Thread(target=self.nb_file_watch, daemon=True).start()
         threading.Thread(target=self.process_msgs, daemon=True).start()
@@ -312,14 +309,16 @@
         self.update_worker_state(WorkerState.Busy)
 
         self.nbrun = NbRun(
             show_code=self.show_code(),
             show_prompt=self.show_prompt(),
             is_presentation=self.is_presentation(),
             reveal_theme=self.reveal_theme(),
+            stop_on_error=self.stop_on_error(),
+            user_info=self.get_user_info(),
         )
 
         self.install_new_packages()
         self.provision_secrets()
 
         # we need to initialize the output dir always
         # even if there is no OutputDir in the notebook
@@ -376,14 +375,17 @@
 
         nb_params = json.loads(self.notebook.params)
 
         self.nbrun.set_show_code_and_prompt(
             nb_params.get("show-code", False), nb_params.get("show-prompt", True)
         )
         self.nbrun.set_is_presentation(nb_params.get("output", "app") == "slides")
+        self.nbrun.set_stop_on_error(
+            nb_params.get("stop_on_error", False)
+        )
 
         log.debug(params)
         log.debug(f"Exporter show_code {self.nbrun.exporter.show_code}")
 
         self.nb = copy.deepcopy(self.nb_original)
 
         if self.is_presentation():
```

### Comparing `mercury-2.3.1/mercury/apps/nbworker/rest.py` & `mercury-2.3.2/mercury/apps/nbworker/rest.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,44 +2,68 @@
 import logging
 import os
 import sys
 from types import SimpleNamespace
 
 import requests
 
-from apps.workers.models import Worker, WorkerState
+from apps.workers.constants import WorkerState
 from apps.ws.utils import machine_uuid
 
 log = logging.getLogger(__name__)
 
 
 class RESTClient:
     def __init__(self, notebook_id, session_id, worker_id):
         self.server_url = os.environ.get("MERCURY_SERVER_URL", "http://127.0.0.1:8000")
         self.notebook_id = notebook_id
         self.session_id = session_id
         self.worker_id = worker_id
         self.worker = None  # SimpleNamespace object
         self.state = WorkerState.Unknown
         self.notebook = None  # SimpleNamespace object
+        self.owner = None # SimpleNamespace object
+        self.user = None # SimpleNamespace object
         self.load_notebook()
+        self.load_owner_and_user()
 
     def load_notebook(self):
         try:
             log.debug(f"Load notebook id={self.notebook_id}")
             response = requests.get(
                 f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/nb"
             )
             if response.status_code != 200:
                 raise Exception("Cant load notebook")
             self.notebook = SimpleNamespace(**response.json())
         except Exception:
             log.exception("Exception when notebook load, quit")
             sys.exit(0)
 
+    def load_owner_and_user(self):
+        try:
+            log.debug("Load owner and user")
+            response = requests.get(
+                f"{self.server_url}/api/v1/worker/{self.session_id}/{self.worker_id}/{self.notebook_id}/owner-and-user"
+            )
+            if response.status_code != 200:
+                raise Exception("Cant load onwer and user information")
+            owner = response.json().get("owner", {})
+            user = response.json().get("user", {})
+            if owner: self.owner = SimpleNamespace(**owner)
+            if user: self.user = SimpleNamespace(**user)
+        except Exception:
+            log.exception("Exception when loading owner and user")
+
+    def get_user_info(self):
+        print(self.user)
+        if self.user is None:
+            return None
+        return json.dumps(self.user.__dict__)
+
     def update_notebook(self, new_params):
         log.debug(f"Executed params {json.dumps(new_params, indent=4)}")
 
         update_database = False
         if new_params.get("title", "") != "" and self.notebook.title != new_params.get(
             "title", ""
         ):
@@ -52,14 +76,15 @@
             "show-prompt",
             "continuous_update",
             "static_notebook",
             "description",
             "show_sidebar",
             "full_screen",
             "allow_download",
+            "stop_on_error",
         ]:
             if new_params.get(property) is not None and nb_params.get(
                 property
             ) != new_params.get(property):
                 nb_params[property] = new_params.get(property)
                 update_database = True
         # save widgets params
@@ -115,14 +140,25 @@
             log.exception("Exception when check if show promtp from notebook")
         return False
 
     def reveal_theme(self):
         # TODO: get reveal theme
         return "white"
 
+    def stop_on_error(self):
+        try:
+            stop_on_error = str(
+                json.loads(self.notebook.params).get("stop_on_error", "false")
+            ).lower()
+            log.debug(f"Check if stop_on_error ({stop_on_error})")
+            return stop_on_error == "true"
+        except Exception:
+            log.exception("Exception when check if stop_on_error")
+        return False
+
     def worker_state(self):
         return self.state
 
     def set_worker_state(self, new_state):
         try:
             log.debug(
                 f"Worker id={self.worker_id} set state {new_state} uuid {machine_uuid()}"
```

### Comparing `mercury-2.3.1/mercury/apps/nbworker/tests.py` & `mercury-2.3.2/mercury/apps/nbworker/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from apps.accounts.models import Site
 from apps.nbworker.rest import RESTClient
 from apps.notebooks.models import Notebook
 from apps.storage.models import UploadedFile
 from apps.storage.s3utils import S3
 from apps.storage.storage import StorageManager
-from apps.workers.models import Worker, WorkerState
+from apps.workers.models import Worker
+from apps.workers.constants import WorkerState
 
 # python manage.py test apps.nbworker -v 2
 
 
 class RESTClientTestCase(LiveServerTestCase):
     def setUp(self):
         self.user = User.objects.create_user(
```

### Comparing `mercury-2.3.1/mercury/apps/nbworker/utils.py` & `mercury-2.3.2/mercury/apps/nbworker/utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/nbworker/ws.py` & `mercury-2.3.2/mercury/apps/nbworker/ws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 import logging
-import time
 import sys
 from queue import Queue
 
 import websocket
 
 from apps.nbworker.rest import RESTClient
 from apps.nbworker.utils import Purpose, stop_event
-from apps.workers.models import WorkerState
 from apps.storage.storage import StorageManager
 
 log = logging.getLogger(__name__)
 
 
 class WSClient(RESTClient):
     def __init__(self, ws_address, notebook_id, session_id, worker_id):
@@ -45,15 +43,14 @@
             log.exception("Exception when WS connect")
 
     def on_open(self, ws):
         log.info("Open ws connection")
         self.queue.put(json.dumps({"purpose": Purpose.InitNotebook}))
         # just check if exists
         self.worker_exists()
-        
 
     def on_close(self, ws, close_status_code, close_msg):
         global stop_event
         stop_event.set()
         self.sm.delete_worker_output_dir()
         log.info(f"WS close connection, status={close_status_code}, msg={close_msg}")
```

### Comparing `mercury-2.3.1/mercury/apps/notebooks/management/commands/add.py` & `mercury-2.3.2/mercury/apps/notebooks/management/commands/add.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/management/commands/delete.py` & `mercury-2.3.2/mercury/apps/notebooks/management/commands/delete.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/management/commands/list.py` & `mercury-2.3.2/mercury/apps/notebooks/management/commands/list.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/management/commands/watch.py` & `mercury-2.3.2/mercury/apps/notebooks/management/commands/watch.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/migrations/0001_initial.py` & `mercury-2.3.2/mercury/apps/notebooks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/models.py` & `mercury-2.3.2/mercury/apps/notebooks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/serializers.py` & `mercury-2.3.2/mercury/apps/notebooks/serializers.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/slides_themes.py` & `mercury-2.3.2/mercury/apps/notebooks/slides_themes.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/tasks.py` & `mercury-2.3.2/mercury/apps/notebooks/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                     site = Site.objects.create(
                         title="Mercury",
                         slug="single-site",
                         share=Site.PUBLIC,
                         created_by=user,
                         status=SiteStatus.READY,
                         domain=os.environ.get("MERCURY_DOMAIN", "runmercury.com"),
-                        custom_domain=os.environ.get("MERCURY_CUSTOM_DOMAIN")
+                        custom_domain=os.environ.get("MERCURY_CUSTOM_DOMAIN"),
                     )
                 else:
                     site = Site.objects.get(slug="single-site")
 
             bucket_key_fname = ""
             if bucket_key is not None:
                 s3 = S3()
```

### Comparing `mercury-2.3.1/mercury/apps/notebooks/urls.py` & `mercury-2.3.2/mercury/apps/notebooks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/notebooks/views.py` & `mercury-2.3.2/mercury/apps/notebooks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/migrations/0001_initial.py` & `mercury-2.3.2/mercury/apps/storage/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/migrations/0002_useruploadedfile.py` & `mercury-2.3.2/mercury/apps/storage/migrations/0002_useruploadedfile.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/models.py` & `mercury-2.3.2/mercury/apps/storage/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/s3utils.py` & `mercury-2.3.2/mercury/apps/storage/s3utils.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/storage.py` & `mercury-2.3.2/mercury/apps/storage/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 import os
 import shutil
 import sys
 import uuid
 
 import requests
 from django.conf import settings
-from execnb.nbio import write_nb
-from django_drf_filepond.models import TemporaryUpload
 
 from apps.nbworker.utils import stop_event
-from apps.storage.models import UploadedFile
 from apps.storage.utils import get_worker_bucket_key
 from apps.tasks.export_pdf import to_pdf
 
 log = logging.getLogger(__name__)
 
 
 class StorageManager:
@@ -250,16 +247,22 @@
         return pdf_path, pdf_url
 
     def some_hash(self):
         h = uuid.uuid4().hex.replace("-", "")
         return h[:8]
 
     def get_user_uploaded_file(self, value):
+        log.debug("get user uploaded file " * 33)
         if settings.STORAGE == settings.STORAGE_MEDIA:
             log.debug(f"Get file {value[0]} from id={value[1]}")
+            import django
+
+            django.setup()
+            from django_drf_filepond.models import TemporaryUpload
+
             tu = TemporaryUpload.objects.get(upload_id=value[1])
             value[1] = tu.get_file_path()
             value[1] = value[1].replace("\\", "\\\\")
             log.debug(f"File path is {value[1]}")
         elif settings.STORAGE == settings.STORAGE_S3:
             # get link
```

### Comparing `mercury-2.3.1/mercury/apps/storage/tests.py` & `mercury-2.3.2/mercury/apps/storage/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/urls.py` & `mercury-2.3.2/mercury/apps/storage/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 )
 from apps.storage.views.notebookfiles import (
     NbPresignedUrlPut,
     NbFileUploaded,
     NbDeleteFile,
     WorkerGetNbFileUrl,
 )
+from apps.storage.views.stylefiles import (
+    StyleUrlPut,
+    StyleUrlGet
+)
+
 
 storage_urlpatterns = [
     re_path(
         "api/v1/storage-type",
         GetStorageType.as_view(),
     ),
     #
@@ -42,14 +47,25 @@
         FileUploaded.as_view(),
     ),
     re_path(
         "api/v1/delete-file",
         DeleteFile.as_view(),
     ),
     #
+    # style files
+    #
+    re_path(
+        "api/v1/style-put/(?P<site_id>.+)/(?P<filename>.+)/(?P<filesize>.+)",
+        StyleUrlPut.as_view(),
+    ),
+    re_path(
+        "api/v1/get-style/(?P<site_id>.+)/(?P<filename>.+)",
+        StyleUrlGet.as_view(),
+    ),
+    #
     # worker files
     #
     re_path(
         "api/v1/worker/presigned-url/(?P<action>.+)/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/(?P<output_dir>.+)/(?P<filename>.+)",
         WorkerPresignedUrl.as_view(),
     ),
     re_path(
```

### Comparing `mercury-2.3.1/mercury/apps/storage/views/dashboardfiles.py` & `mercury-2.3.2/mercury/apps/storage/views/dashboardfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/views/notebookfiles.py` & `mercury-2.3.2/mercury/apps/storage/views/notebookfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/storage/views/workerfiles.py` & `mercury-2.3.2/mercury/apps/storage/views/workerfiles.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/export_pdf.py` & `mercury-2.3.2/mercury/apps/tasks/export_pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from subprocess import PIPE, Popen
 
 pdf_export_available = True
 try:
     from pyppeteer import launch
 except Exception:
     pdf_export_available = False
-    
+
+
 async def html_to_pdf(html_file, pdf_file, pyppeteer_args=None):
     """Convert a HTML file to a PDF"""
     browser = await launch(
         handleSIGINT=False,
         handleSIGTERM=False,
         handleSIGHUP=False,
         headless=True,
```

### Comparing `mercury-2.3.1/mercury/apps/tasks/export_png.py` & `mercury-2.3.2/mercury/apps/tasks/export_png.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/migrations/0001_initial.py` & `mercury-2.3.2/mercury/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/models.py` & `mercury-2.3.2/mercury/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/notify.py` & `mercury-2.3.2/mercury/apps/tasks/notify.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/tasks.py` & `mercury-2.3.2/mercury/apps/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/tasks_export.py` & `mercury-2.3.2/mercury/apps/tasks/tasks_export.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/tests.py` & `mercury-2.3.2/mercury/apps/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/urls.py` & `mercury-2.3.2/mercury/apps/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/tasks/views.py` & `mercury-2.3.2/mercury/apps/tasks/views.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/workers/migrations/0001_initial.py` & `mercury-2.3.2/mercury/apps/workers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/workers/urls.py` & `mercury-2.3.2/mercury/apps/workers/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 from apps.workers.views import (
     DeleteWorker,
     GetWorker,
     IsWorkerStale,
     SetWorkerState,
     WorkerGetNb,
     WorkerUpdateNb,
+    MachineInfo,
+    WorkerGetOwnerAndUser,
 )
 
 workers_urlpatterns = [
     re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/nb",
         WorkerGetNb.as_view(),
     ),
     re_path(
+        "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/owner-and-user",
+        WorkerGetOwnerAndUser.as_view(),
+    ),
+    re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/update-nb",
         WorkerUpdateNb.as_view(),
     ),
     re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/worker",
         GetWorker.as_view(),
     ),
@@ -30,8 +36,12 @@
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/set-worker-state",
         SetWorkerState.as_view(),
     ),
     re_path(
         "api/v1/worker/(?P<session_id>.+)/(?P<worker_id>.+)/(?P<notebook_id>.+)/delete-worker",
         DeleteWorker.as_view(),
     ),
+    re_path(
+        "api/v1/machine-info",
+        MachineInfo.as_view(),
+    ),
 ]
```

### Comparing `mercury-2.3.1/mercury/apps/ws/client.py` & `mercury-2.3.2/mercury/apps/ws/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def connect(self):
         log.debug("Trying to connect client")
 
         self.notebook_id = int(self.scope["url_route"]["kwargs"]["notebook_id"])
         self.session_id = self.scope["url_route"]["kwargs"]["session_id"]
 
         self.user = self.scope["user"]
+
         nb = Notebook.objects.get(pk=self.notebook_id)
         if nb.hosted_on.share == Site.PRIVATE:
             if self.user.is_anonymous:
                 self.close()
             else:
                 member = Membership.objects.filter(user=self.user, host=nb.hosted_on)
                 owner = nb.hosted_on.created_by == self.user
@@ -126,14 +127,16 @@
         with transaction.atomic():
             log.debug("Create worker in db")
             worker = Worker(
                 session_id=self.session_id,
                 notebook_id=self.notebook_id,
                 state="Queued",
             )
+            if not self.user.is_anonymous:
+                worker.run_by = self.user
             worker.save()
             job_params = {
                 "notebook_id": self.notebook_id,
                 "session_id": self.session_id,
                 "worker_id": worker.id,
                 #
                 # ugly hack for docker deployment
```

### Comparing `mercury-2.3.1/mercury/apps/ws/middleware.py` & `mercury-2.3.2/mercury/apps/ws/middleware.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/apps/ws/tasks.py` & `mercury-2.3.2/mercury/apps/ws/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 from celery import shared_task
 from django.conf import settings
 
 from apps.workers.models import Worker
 from apps.ws.utils import machine_uuid
 
+from apps.workers.utils import get_running_machines, shuffle_machines, need_instance
+
+
 log = logging.getLogger(__name__)
 
 
 @shared_task(bind=True)
 def task_start_websocket_worker(self, job_params):
     log.debug(f"NbWorkers per machine: {settings.NBWORKERS_PER_MACHINE}")
 
-    workers_ip_list = os.environ.get("WORKERS_IP_LIST", "")
-
-    if workers_ip_list == "":
+    if os.environ.get("MACHINE_SPELL", "") == "":
         machine_id = machine_uuid()
         workers = Worker.objects.filter(machine_id=machine_id)
 
         log.debug(f"Workers count: {len(workers)} machine_id={ machine_id }")
 
         if len(workers) > settings.NBWORKERS_PER_MACHINE:
             log.debug("Defer task start ws worker")
@@ -37,16 +38,18 @@
                 str(job_params["session_id"]),
                 str(job_params["worker_id"]),
                 job_params["server_url"],
             ]
             log.debug("Start " + " ".join(command))
             worker = subprocess.Popen(command)
     else:
-        workers_ips = workers_ip_list.split(",")
-        print(workers_ips)
+        machines = get_running_machines()
+        machines = shuffle_machines(machines)
+
+        workers_ips = [m.ipv4 for m in machines]
 
         all_busy = True
 
         for worker_ip in workers_ips:
             try:
                 workers = Worker.objects.filter(machine_id=worker_ip)
 
@@ -64,8 +67,9 @@
                             all_busy = False
                             break
             except Exception as e:
                 pass
 
         if all_busy:
             log.debug("Defer task start ws worker")
+            need_instance(job_params["worker_id"])
             task_start_websocket_worker.s(job_params).apply_async(countdown=15)
```

### Comparing `mercury-2.3.1/mercury/apps/ws/utils.py` & `mercury-2.3.2/mercury/apps/ws/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,39 @@
 
 log = logging.getLogger(__name__)
 
 
 CLIENT_SITE = "client"
 WORKER_SITE = "worker"
 
-
+# global variable
 my_ip = None
 
 
 def machine_uuid():
     global my_ip
     if my_ip is not None:
         return my_ip
     if os.environ.get("USE_WORKER_IP") is not None:
-        response = requests.get("https://api.ipify.org?format=json")
-        my_ip = response.json().get("ip", platform.node())
-        return my_ip
-    return platform.node()
+        try:
+            # fast way to get IP
+            response = requests.get("http://checkip.amazonaws.com")
+            my_ip = response.content.decode("UTF-8").replace("\n", "")
+            return my_ip
+
+        except Exception as e:
+            pass
+
+        # alternative service
+        # response = requests.get("https://api.ipify.org?format=json")
+        # my_ip = response.json().get("ip", platform.node())
+        # return my_ip
+
+    my_ip = platform.node()
+    return my_ip
 
 
 def client_group(notebook_id, session_id):
     return f"{CLIENT_SITE}-{notebook_id}-{session_id}"
 
 
 def worker_group(notebook_id, session_id):
@@ -111,15 +123,20 @@
                     if view.get("notify") is not None:
                         params["notify"] = json.loads(view.get("notify"))
                     if view.get("continuous_update") is not None:
                         params["continuous_update"] = view.get("continuous_update")
                     if view.get("static_notebook") is not None:
                         params["static_notebook"] = view.get("static_notebook")
 
-                    for property in ["show_sidebar", "full_screen", "allow_download"]:
+                    for property in [
+                        "show_sidebar",
+                        "full_screen",
+                        "allow_download",
+                        "stop_on_error",
+                    ]:
                         if view.get(property) is not None:
                             params[property] = view.get(property)
 
                 else:
                     params["params"][widget_key] = WidgetsManager.frontend_format(view)
 
                 all_model_ids += [view.get("model_id", "")]
@@ -136,14 +153,16 @@
         params["static_notebook"] = not mercury_package_imported
     if params.get("show_sidebar") is None:
         params["show_sidebar"] = True
     if params.get("full_screen") is None:
         params["full_screen"] = True
     if params.get("allow_download") is None:
         params["allow_download"] = True
+    if params.get("stop_on_error") is None:
+        params["stop_on_error"] = False
 
     if no_outputs:
         params["version"] = "2"
         params["show-code"] = False
         params["show-prompt"] = False
         params["params"] = {}
         params["output"] = "app"
```

### Comparing `mercury-2.3.1/mercury/demo.py` & `mercury-2.3.2/mercury/demo.py`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/asset-manifest.json` & `mercury-2.3.2/mercury/frontend-dist/asset-manifest.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6727941176470589%*

 * *Differences: {"'entrypoints'": "{insert: [(2, 'static/js/2.20c8cb43.chunk.js'), (3, "*

 * *                  "'static/css/main.9848f1b3.chunk.css'), (4, "*

 * *                  "'static/js/main.55ba4c52.chunk.js')], delete: [4, 3, 2]}",*

 * * "'files'": "{'main.css': '/static/css/main.9848f1b3.chunk.css', 'main.js': "*

 * *            "'/static/js/main.55ba4c52.chunk.js', 'main.js.map': "*

 * *            "'/static/js/main.55ba4c52.chunk.js.map', 'static/js/2.20c8cb43.chunk.js': "*

 * *            "'/static/js/2.20c8cb43.chunk.js', 'static/js/2.20c […]*

```diff
@@ -1,24 +1,24 @@
 {
     "entrypoints": [
         "static/js/runtime-main.248907bc.js",
         "static/css/2.c6cf5ff9.chunk.css",
-        "static/js/2.206848a5.chunk.js",
-        "static/css/main.80c2d41b.chunk.css",
-        "static/js/main.9c1f23c5.chunk.js"
+        "static/js/2.20c8cb43.chunk.js",
+        "static/css/main.9848f1b3.chunk.css",
+        "static/js/main.55ba4c52.chunk.js"
     ],
     "files": {
         "index.html": "/index.html",
-        "main.css": "/static/css/main.80c2d41b.chunk.css",
-        "main.js": "/static/js/main.9c1f23c5.chunk.js",
-        "main.js.map": "/static/js/main.9c1f23c5.chunk.js.map",
+        "main.css": "/static/css/main.9848f1b3.chunk.css",
+        "main.js": "/static/js/main.55ba4c52.chunk.js",
+        "main.js.map": "/static/js/main.55ba4c52.chunk.js.map",
         "runtime-main.js": "/static/js/runtime-main.248907bc.js",
         "runtime-main.js.map": "/static/js/runtime-main.248907bc.js.map",
         "static/css/2.c6cf5ff9.chunk.css": "/static/css/2.c6cf5ff9.chunk.css",
         "static/css/2.c6cf5ff9.chunk.css.map": "/static/css/2.c6cf5ff9.chunk.css.map",
-        "static/css/main.80c2d41b.chunk.css.map": "/static/css/main.80c2d41b.chunk.css.map",
-        "static/js/2.206848a5.chunk.js": "/static/js/2.206848a5.chunk.js",
-        "static/js/2.206848a5.chunk.js.LICENSE.txt": "/static/js/2.206848a5.chunk.js.LICENSE.txt",
-        "static/js/2.206848a5.chunk.js.map": "/static/js/2.206848a5.chunk.js.map",
+        "static/css/main.9848f1b3.chunk.css.map": "/static/css/main.9848f1b3.chunk.css.map",
+        "static/js/2.20c8cb43.chunk.js": "/static/js/2.20c8cb43.chunk.js",
+        "static/js/2.20c8cb43.chunk.js.LICENSE.txt": "/static/js/2.20c8cb43.chunk.js.LICENSE.txt",
+        "static/js/2.20c8cb43.chunk.js.map": "/static/js/2.20c8cb43.chunk.js.map",
         "static/media/font-awesome.min.css": "/static/media/fontawesome-webfont.f691f37e.woff"
     }
 }
```

### Comparing `mercury-2.3.1/mercury/frontend-dist/favicon-old.ico` & `mercury-2.3.2/mercury/frontend-dist/favicon-old.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/favicon.ico` & `mercury-2.3.2/mercury/frontend-dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/index.html` & `mercury-2.3.2/mercury/frontend-dist/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.80c2d41b.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.206848a5.chunk.js"></script><script src="/static/js/main.9c1f23c5.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/static/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Mercury: Easily share your Python notebooks"/><link rel="manifest" href="/static/manifest.json"/><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script><link rel="stylesheet" href="/static/jupyter-syntax.css"/><link rel="stylesheet" href="/static/jupyter-additional.css"/><link rel="stylesheet" href="/static/jupyter-theme-light.css"/><title>Mercury - Turn Jupyter Notebook to Web App</title><script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"></script><script>init_mathjax=function(){window.MathJax&&(MathJax.Hub.Config({showProcessingMessages:!1,TeX:{equationNumbers:{autoNumber:"AMS",useLabelIds:!0}},tex2jax:{inlineMath:[["$","$"],["\\(","\\)"]],displayMath:[["$$","$$"],["\\[","\\]"]],processEscapes:!0,processEnvironments:!0},displayAlign:"center",CommonHTML:{linebreaks:{automatic:!0}}}),MathJax.Hub.Queue(["Typeset",MathJax.Hub]))},init_mathjax()</script><link href="/static/css/2.c6cf5ff9.chunk.css" rel="stylesheet"><link href="/static/css/main.9848f1b3.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function r(r){for(var n,f,l=r[0],i=r[1],a=r[2],c=0,s=[];c<l.length;c++)f=l[c],Object.prototype.hasOwnProperty.call(o,f)&&o[f]&&s.push(o[f][0]),o[f]=0;for(n in i)Object.prototype.hasOwnProperty.call(i,n)&&(e[n]=i[n]);for(p&&p(r);s.length;)s.shift()();return u.push.apply(u,a||[]),t()}function t(){for(var e,r=0;r<u.length;r++){for(var t=u[r],n=!0,l=1;l<t.length;l++){var i=t[l];0!==o[i]&&(n=!1)}n&&(u.splice(r--,1),e=f(f.s=t[0]))}return e}var n={},o={1:0},u=[];function f(r){if(n[r])return n[r].exports;var t=n[r]={i:r,l:!1,exports:{}};return e[r].call(t.exports,t,t.exports,f),t.l=!0,t.exports}f.m=e,f.c=n,f.d=function(e,r,t){f.o(e,r)||Object.defineProperty(e,r,{enumerable:!0,get:t})},f.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},f.t=function(e,r){if(1&r&&(e=f(e)),8&r)return e;if(4&r&&"object"==typeof e&&e&&e.__esModule)return e;var t=Object.create(null);if(f.r(t),Object.defineProperty(t,"default",{enumerable:!0,value:e}),2&r&&"string"!=typeof e)for(var n in e)f.d(t,n,function(r){return e[r]}.bind(null,n));return t},f.n=function(e){var r=e&&e.__esModule?function(){return e.default}:function(){return e};return f.d(r,"a",r),r},f.o=function(e,r){return Object.prototype.hasOwnProperty.call(e,r)},f.p="/";var l=this.webpackJsonpfrontend=this.webpackJsonpfrontend||[],i=l.push.bind(l);l.push=r,l=l.slice();for(var a=0;a<l.length;a++)r(l[a]);var p=i;t()}([])</script><script src="/static/js/2.20c8cb43.chunk.js"></script><script src="/static/js/main.55ba4c52.chunk.js"></script></body></html>
```

### Comparing `mercury-2.3.1/mercury/frontend-dist/jupyter-additional.css` & `mercury-2.3.2/mercury/frontend-dist/jupyter-additional.css`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/jupyter-syntax.css` & `mercury-2.3.2/mercury/frontend-dist/jupyter-syntax.css`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/jupyter-theme-light.css` & `mercury-2.3.2/mercury/frontend-dist/jupyter-theme-light.css`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/mercury_black_logo.svg` & `mercury-2.3.2/mercury/frontend-dist/mercury_black_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/mercury_logo.svg` & `mercury-2.3.2/mercury/frontend-dist/mercury_logo.svg`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css` & `mercury-2.3.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map` & `mercury-2.3.2/mercury/frontend-dist/static/css/2.c6cf5ff9.chunk.css.map`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css` & `mercury-2.3.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css`

 * *Files 3% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-.filepond--credits{display:none}.loading-bullet{color:#09c!important}.uneditable-input:focus,input[type=checkbox]:focus,input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus,textarea:focus{box-shadow:none;border:2px solid #2684ff}.uneditable-input:focus,div[role=slider]:focus{border:2px solid #2684ff!important}.form-check-input:checked{background-color:#2684ff!important}.thumbnailIframe{-ms-zoom:.5;zoom:.5;-moz-transform:scale(.5);-moz-transform-origin:0 0;-o-transform:scale(.5);-o-transform-origin:0 0;-webkit-transform:scale(.5);-webkit-transform-origin:0 0;transform:scale(.5);transform-origin:0 0}.sidebar{position:fixed;top:0;bottom:0;left:0;z-index:100;padding:48px 0 0;box-shadow:inset -1px 0 0 rgba(0,0,0,.1);border-left:1px solid #eee}.sidebar-sticky{position:relative;top:0;height:calc(100vh - 48px);padding-top:.5rem;overflow-x:hidden;overflow-y:auto}.sidebar .nav-link{font-weight:500;color:#333}.sidebar .nav-link .feather{margin-right:4px;color:#727272}.sidebar .nav-link.active{color:#2470dc}.sidebar .nav-link.active .feather,.sidebar .nav-link:hover .feather{color:inherit}.sidebar-heading{font-size:.75rem;text-transform:uppercase}.navbar-brand{padding-top:.75rem;padding-bottom:.75rem;font-size:1rem;background-color:rgba(0,0,0,.25);box-shadow:inset -1px 0 0 rgba(0,0,0,.25)}.navbar .navbar-toggler{top:.25rem;right:1rem}.div-signin{padding-top:60px;padding-bottom:40px}.form-signin{width:100%;max-width:330px;padding:15px;margin:0 auto}.form-signin .form-control{position:relative;box-sizing:border-box;height:auto;padding:10px;font-size:16px}.form-signin .form-control:focus{z-index:2}.form-signin input[type=email]{margin-bottom:-1px;border-bottom-right-radius:0;border-bottom-left-radius:0}.form-signin input[type=password]{margin-bottom:10px;border-top-left-radius:0;border-top-right-radius:0}.poweredby{position:absolute;top:5px;right:5px}.btn-primary{border-color:#2684ff!important;background-color:#2684ff!important}.btn-primary:hover{border-color:#217bf1!important;background-color:#217bf1!important}.btn-outline-primary{border-color:#2684ff!important;color:#2684ff!important}.btn-outline-primary:hover{border-color:#2684ff!important;color:#fff!important;background-color:#2684ff!important}.title-card{background-color:rgba(38,132,255,.04)}.title-card:hover{background-color:rgba(38,132,255,.08)}body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Roboto","Oxygen","Ubuntu","Cantarell","Fira Sans","Droid Sans","Helvetica Neue",sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,"Courier New",monospace}html{position:relative;min-height:100%}
-/*# sourceMappingURL=main.80c2d41b.chunk.css.map */
+.filepond--credits{display:none}.loading-bullet{color:#09c!important}.uneditable-input:focus,input[type=checkbox]:focus,input[type=color]:focus,input[type=date]:focus,input[type=datetime-local]:focus,input[type=datetime]:focus,input[type=email]:focus,input[type=month]:focus,input[type=number]:focus,input[type=password]:focus,input[type=search]:focus,input[type=tel]:focus,input[type=text]:focus,input[type=time]:focus,input[type=url]:focus,input[type=week]:focus,textarea:focus{box-shadow:none;border:2px solid #2684ff}.uneditable-input:focus,div[role=slider]:focus{border:2px solid #2684ff!important}.form-check-input:checked{background-color:#2684ff!important}.thumbnailIframe{-ms-zoom:.5;zoom:.5;-moz-transform:scale(.5);-moz-transform-origin:0 0;-o-transform:scale(.5);-o-transform-origin:0 0;-webkit-transform:scale(.5);-webkit-transform-origin:0 0;transform:scale(.5);transform-origin:0 0}.sidebar{position:fixed;top:0;bottom:0;left:0;z-index:100;padding:48px 0 0;box-shadow:inset -1px 0 0 rgba(0,0,0,.1);border-left:1px solid #eee}.sidebar-sticky{position:relative;top:0;height:calc(100vh - 48px);padding-top:.5rem;overflow-x:hidden;overflow-y:auto}.sidebar .nav-link{font-weight:500;color:#333}.sidebar .nav-link .feather{margin-right:4px;color:#727272}.sidebar .nav-link.active{color:#2470dc}.sidebar .nav-link.active .feather,.sidebar .nav-link:hover .feather{color:inherit}.sidebar-heading{font-size:.75rem;text-transform:uppercase}.navbar-brand{padding-top:.75rem;padding-bottom:.75rem;font-size:1rem;background-color:rgba(0,0,0,.25);box-shadow:inset -1px 0 0 rgba(0,0,0,.25)}.navbar .navbar-toggler{top:.25rem;right:1rem}.div-signin{padding-top:60px;padding-bottom:40px}.form-signin{width:100%;max-width:330px;padding:15px;margin:0 auto}.form-signin .form-control{position:relative;box-sizing:border-box;height:auto;padding:10px;font-size:16px}.form-signin .form-control:focus{z-index:2}.form-signin input[type=email]{margin-bottom:-1px;border-bottom-right-radius:0;border-bottom-left-radius:0}.form-signin input[type=password]{margin-bottom:10px;border-top-left-radius:0;border-top-right-radius:0}.poweredby{position:absolute;top:5px;right:5px}.btn-primary{border-color:#2684ff!important;background-color:#2684ff!important}.btn-primary:hover{border-color:#217bf1!important;background-color:#217bf1!important}.btn-outline-primary{border-color:#2684ff!important;color:#2684ff!important}.btn-outline-primary:hover{border-color:#2684ff!important;color:#fff!important;background-color:#2684ff!important}.title-card{background-color:rgba(38,132,255,.04)}.title-card:hover{background-color:rgba(38,132,255,.08)}body{margin:0;font-family:-apple-system,BlinkMacSystemFont,"Segoe UI","Roboto","Oxygen","Ubuntu","Cantarell","Fira Sans","Droid Sans","Helvetica Neue",sans-serif;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}code{font-family:source-code-pro,Menlo,Monaco,Consolas,"Courier New",monospace}html{position:relative;min-height:100%;-ms-scroll-chaining:none;overscroll-behavior:none}
+/*# sourceMappingURL=main.9848f1b3.chunk.css.map */
```

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/css/main.80c2d41b.chunk.css.map` & `mercury-2.3.2/mercury/frontend-dist/static/css/main.9848f1b3.chunk.css.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'file'": "'main.9848f1b3.chunk.css'",*

 * * "'mappings'": "'AAEA,mBACE,YACF,CAIA,gBACE,oBACF,CAGA,2ZAiBE,eAAgB,CAChB,wBACF,CAEA,+CAGE,kCACF,CAEA,0BACE,kCACF,CAEA,iBACE,WAAa,CACb,OAAS,CACT,wBAA0B,CAC1B,yBAA0B,CAC1B,sBAAwB,CACxB,uBAAwB,CACxB,2BAA6B,CAC7B,4BAA6B,CAC7B,mBAAqB,CACrB,oBACF,CAMA,SACE,cAAe,CACf,KAAM,CACN,QAAS,CACT,MAAO,CACP,WAAY,CACZ,gBAAiB,CACjB,wCAA6C,CAC7C,0BACF,CAQA,gBACE,iBAAkB,CAClB,KAAM,CACN,yBAA0B,CAC1B,iBAAmB,CACnB,iBAAkB,CAClB,eACF,CAEA,mBACE,eAAgB,CAChB,UACF,CAEA,4BACE,gBAAiB,CACjB,aACF,CAE […]*

```diff
@@ -1,14 +1,14 @@
 {
-    "file": "main.80c2d41b.chunk.css",
-    "mappings": "AAEA,mBACE,YACF,CAIA,gBACE,oBACF,CAGA,2ZAiBE,eAAgB,CAChB,wBACF,CAEA,+CAGE,kCACF,CAEA,0BACE,kCACF,CAEA,iBACE,WAAa,CACb,OAAS,CACT,wBAA0B,CAC1B,yBAA0B,CAC1B,sBAAwB,CACxB,uBAAwB,CACxB,2BAA6B,CAC7B,4BAA6B,CAC7B,mBAAqB,CACrB,oBACF,CAMA,SACE,cAAe,CACf,KAAM,CACN,QAAS,CACT,MAAO,CACP,WAAY,CACZ,gBAAiB,CACjB,wCAA6C,CAC7C,0BACF,CAQA,gBACE,iBAAkB,CAClB,KAAM,CACN,yBAA0B,CAC1B,iBAAmB,CACnB,iBAAkB,CAClB,eACF,CAEA,mBACE,eAAgB,CAChB,UACF,CAEA,4BACE,gBAAiB,CACjB,aACF,CAEA,0BACE,aACF,CAEA,qEAEE,aACF,CAEA,iBACE,gBAAkB,CAClB,wBACF,CAMA,cACE,kBAAoB,CACpB,qBAAuB,CACvB,cAAe,CACf,gCAAqC,CACrC,yCACF,CAEA,wBACE,UAAY,CACZ,UACF,CAMA,YACE,gBAAiB,CACjB,mBAEF,CAEA,aACE,UAAW,CACX,eAAgB,CAChB,YAAa,CACb,aACF,CAEA,2BACE,iBAAkB,CAClB,qBAAsB,CACtB,WAAY,CACZ,YAAa,CACb,cACF,CACA,iCACE,SACF,CACA,+BACE,kBAAmB,CACnB,4BAA6B,CAC7B,2BACF,CACA,kCACE,kBAAmB,CACnB,wBAAyB,CACzB,yBACF,CAEA,WACE,iBAAkB,CAElB,OAAQ,CACR,SAEF,CAEA,aACE,8BAAgC,CAChC,kCACF,CAEA,mBACE,8BAAgC,CAChC,kCACF,CAEA,qBACE,8BAAgC,CAChC,uBACF,CAEA,2BACE,8BAAgC,CAChC,oBAAuB,CACvB,kCACF,CAEA,YACE,qCACF,CAEA,kBACE,qCACF,CCzMA,KACE,QAAS,CACT,mJAEY,CACZ,kCAAmC,CACnC,iCACF,CAEA,KACE,yEAEF,CAEA,KACE,iBAAkB,CAClB,eACF",
+    "file": "main.9848f1b3.chunk.css",
+    "mappings": "AAEA,mBACE,YACF,CAIA,gBACE,oBACF,CAGA,2ZAiBE,eAAgB,CAChB,wBACF,CAEA,+CAGE,kCACF,CAEA,0BACE,kCACF,CAEA,iBACE,WAAa,CACb,OAAS,CACT,wBAA0B,CAC1B,yBAA0B,CAC1B,sBAAwB,CACxB,uBAAwB,CACxB,2BAA6B,CAC7B,4BAA6B,CAC7B,mBAAqB,CACrB,oBACF,CAMA,SACE,cAAe,CACf,KAAM,CACN,QAAS,CACT,MAAO,CACP,WAAY,CACZ,gBAAiB,CACjB,wCAA6C,CAC7C,0BACF,CAQA,gBACE,iBAAkB,CAClB,KAAM,CACN,yBAA0B,CAC1B,iBAAmB,CACnB,iBAAkB,CAClB,eACF,CAEA,mBACE,eAAgB,CAChB,UACF,CAEA,4BACE,gBAAiB,CACjB,aACF,CAEA,0BACE,aACF,CAEA,qEAEE,aACF,CAEA,iBACE,gBAAkB,CAClB,wBACF,CAMA,cACE,kBAAoB,CACpB,qBAAuB,CACvB,cAAe,CACf,gCAAqC,CACrC,yCACF,CAEA,wBACE,UAAY,CACZ,UACF,CAMA,YACE,gBAAiB,CACjB,mBAEF,CAEA,aACE,UAAW,CACX,eAAgB,CAChB,YAAa,CACb,aACF,CAEA,2BACE,iBAAkB,CAClB,qBAAsB,CACtB,WAAY,CACZ,YAAa,CACb,cACF,CACA,iCACE,SACF,CACA,+BACE,kBAAmB,CACnB,4BAA6B,CAC7B,2BACF,CACA,kCACE,kBAAmB,CACnB,wBAAyB,CACzB,yBACF,CAEA,WACE,iBAAkB,CAElB,OAAQ,CACR,SAEF,CAEA,aACE,8BAAgC,CAChC,kCACF,CAEA,mBACE,8BAAgC,CAChC,kCACF,CAEA,qBACE,8BAAgC,CAChC,uBACF,CAEA,2BACE,8BAAgC,CAChC,oBAAuB,CACvB,kCACF,CAEA,YACE,qCACF,CAEA,kBACE,qCACF,CCzMA,KACE,QAAS,CACT,mJAEY,CACZ,kCAAmC,CACnC,iCACF,CAEA,KACE,yEAEF,CAEA,KACE,iBAAkB,CAClB,eAAgB,CAChB,wBAAyB,CAAzB,wBACF",
     "names": [],
     "sources": [
         "webpack://src/views/App.css",
         "webpack://src/index.css"
     ],
     "sourcesContent": [
         "/* file upload widget */\n\n.filepond--credits {\n  display: none;\n}\n\n/* Loading Bullet in BlockUI */\n\n.loading-bullet {\n  color: #0099cc !important;\n}\n\n/* widgets */\ntextarea:focus,\ninput[type=\"text\"]:focus,\ninput[type=\"password\"]:focus,\ninput[type=\"datetime\"]:focus,\ninput[type=\"datetime-local\"]:focus,\ninput[type=\"date\"]:focus,\ninput[type=\"month\"]:focus,\ninput[type=\"time\"]:focus,\ninput[type=\"week\"]:focus,\ninput[type=\"number\"]:focus,\ninput[type=\"email\"]:focus,\ninput[type=\"url\"]:focus,\ninput[type=\"search\"]:focus,\ninput[type=\"tel\"]:focus,\ninput[type=\"color\"]:focus,\ninput[type=\"checkbox\"]:focus,\n.uneditable-input:focus {\n  box-shadow: none;\n  border: 2px solid #2684ff;\n}\n\ndiv[role=\"slider\"]:focus,\n.uneditable-input:focus {\n  /* box-shadow: none; */\n  border: 2px solid #2684ff !important;\n}\n\n.form-check-input:checked {\n  background-color: #2684ff !important;\n}\n\n.thumbnailIframe {\n  -ms-zoom: 0.5;\n  zoom: 0.5;\n  -moz-transform: scale(0.5);\n  -moz-transform-origin: 0 0;\n  -o-transform: scale(0.5);\n  -o-transform-origin: 0 0;\n  -webkit-transform: scale(0.5);\n  -webkit-transform-origin: 0 0;\n  transform: scale(0.5);\n  transform-origin: 0 0;\n}\n\n/*\n * Sidebar\n */\n\n.sidebar {\n  position: fixed;\n  top: 0;\n  bottom: 0;\n  left: 0;\n  z-index: 100; /* Behind the navbar */\n  padding: 48px 0 0; /* Height of navbar */\n  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.1);\n  border-left: 1px solid #eeeeee;\n}\n\n/* @media (max-width: 767.98px) {\n  .sidebar {\n    top: 0rem;\n  }\n} */\n\n.sidebar-sticky {\n  position: relative;\n  top: 0;\n  height: calc(100vh - 48px);\n  padding-top: 0.5rem;\n  overflow-x: hidden;\n  overflow-y: auto; /* Scrollable contents if viewport is shorter than content. */\n}\n\n.sidebar .nav-link {\n  font-weight: 500;\n  color: #333;\n}\n\n.sidebar .nav-link .feather {\n  margin-right: 4px;\n  color: #727272;\n}\n\n.sidebar .nav-link.active {\n  color: #2470dc;\n}\n\n.sidebar .nav-link:hover .feather,\n.sidebar .nav-link.active .feather {\n  color: inherit;\n}\n\n.sidebar-heading {\n  font-size: 0.75rem;\n  text-transform: uppercase;\n}\n\n/*\n * Navbar\n */\n\n.navbar-brand {\n  padding-top: 0.75rem;\n  padding-bottom: 0.75rem;\n  font-size: 1rem;\n  background-color: rgba(0, 0, 0, 0.25);\n  box-shadow: inset -1px 0 0 rgba(0, 0, 0, 0.25);\n}\n\n.navbar .navbar-toggler {\n  top: 0.25rem;\n  right: 1rem;\n}\n\n/*\n  Login\n*/\n\n.div-signin {\n  padding-top: 60px;\n  padding-bottom: 40px;\n  /* background-color: #f5f5f5; */\n}\n\n.form-signin {\n  width: 100%;\n  max-width: 330px;\n  padding: 15px;\n  margin: 0 auto;\n}\n\n.form-signin .form-control {\n  position: relative;\n  box-sizing: border-box;\n  height: auto;\n  padding: 10px;\n  font-size: 16px;\n}\n.form-signin .form-control:focus {\n  z-index: 2;\n}\n.form-signin input[type=\"email\"] {\n  margin-bottom: -1px;\n  border-bottom-right-radius: 0;\n  border-bottom-left-radius: 0;\n}\n.form-signin input[type=\"password\"] {\n  margin-bottom: 10px;\n  border-top-left-radius: 0;\n  border-top-right-radius: 0;\n}\n\n.poweredby {\n  position: absolute;\n  /* bottom: 10px; */\n  top: 5px;\n  right: 5px;\n  /* border: 1px solid #e5e5e5; */\n}\n\n.btn-primary {\n  border-color: #2684ff !important;\n  background-color: #2684ff !important;\n}\n\n.btn-primary:hover {\n  border-color: #217bf1 !important;\n  background-color: #217bf1 !important;\n}\n\n.btn-outline-primary {\n  border-color: #2684ff !important;\n  color: #2684ff !important;\n}\n\n.btn-outline-primary:hover {\n  border-color: #2684ff !important;\n  color: white !important;\n  background-color: #2684ff !important;\n}\n\n.title-card {\n  background-color: rgba(38, 132, 255, 0.04);\n}\n\n.title-card:hover {\n  background-color: rgba(38, 132, 255, 0.08);\n}\n",
-        "body {\n  margin: 0; \n  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',\n    'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',\n    sans-serif;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n}\n\ncode {\n  font-family: source-code-pro, Menlo, Monaco, Consolas, 'Courier New',\n    monospace;\n}\n\nhtml {\n  position: relative;\n  min-height: 100%;\n}\n\n"
+        "body {\n  margin: 0; \n  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',\n    'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',\n    sans-serif;\n  -webkit-font-smoothing: antialiased;\n  -moz-osx-font-smoothing: grayscale;\n}\n\ncode {\n  font-family: source-code-pro, Menlo, Monaco, Consolas, 'Courier New',\n    monospace;\n}\n\nhtml {\n  position: relative;\n  min-height: 100%;\n  overscroll-behavior: none;\n}\n\n"
     ],
     "version": 3
 }
```

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/js/2.206848a5.chunk.js` & `mercury-2.3.2/mercury/frontend-dist/static/js/2.20c8cb43.chunk.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 2.206848a5.chunk.js.LICENSE.txt */
+/*! For license information please see 2.20c8cb43.chunk.js.LICENSE.txt */
 (this.webpackJsonpfrontend = this.webpackJsonpfrontend || []).push([
     [2],
     [function(e, t, n) {
         "use strict";
         e.exports = n(194)
     }, function(e, t, n) {
         "use strict";
@@ -573,23 +573,23 @@
             return q
         })), n.d(t, "q", (function() {
             return U
         }));
         var r, i = n(6),
             o = n.n(i),
             a = n(13),
-            s = n(8),
-            u = n(24),
+            s = n(9),
+            u = n(25),
             l = n(19),
             c = n(41),
             f = n(42),
             d = n(89),
-            p = n(9),
+            p = n(8),
             h = n(67),
-            m = n(27),
+            m = n(28),
             g = n(15);
 
         function v() {
             return (v = Object.assign ? Object.assign.bind() : function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
@@ -2819,28 +2819,14 @@
             var n = "string" === typeof t ? C(t).search : t.search;
             if (e[e.length - 1].route.index && Ue(n || "")) return e[e.length - 1];
             var r = z(e);
             return r[r.length - 1]
         }
     }, function(e, t, n) {
         "use strict";
-
-        function r(e, t, n) {
-            return t in e ? Object.defineProperty(e, t, {
-                value: n,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : e[t] = n, e
-        }
-        n.d(t, "a", (function() {
-            return r
-        }))
-    }, function(e, t, n) {
-        "use strict";
         n.d(t, "a", (function() {
             return a
         }));
         var r = n(77);
         var i = n(45),
             o = n(78);
 
@@ -2865,14 +2851,28 @@
                     return n
                 }
             }(e, t) || Object(i.a)(e, t) || Object(o.a)()
         }
     }, function(e, t, n) {
         "use strict";
 
+        function r(e, t, n) {
+            return t in e ? Object.defineProperty(e, t, {
+                value: n,
+                enumerable: !0,
+                configurable: !0,
+                writable: !0
+            }) : e[t] = n, e
+        }
+        n.d(t, "a", (function() {
+            return r
+        }))
+    }, function(e, t, n) {
+        "use strict";
+
         function r() {
             return (r = Object.assign || function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
                     for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
                 }
                 return e
@@ -2918,18 +2918,18 @@
         })), n.d(t, "q", (function() {
             return N
         })), n.d(t, "r", (function() {
             return x
         }));
         var r = n(15),
             i = n(19),
-            o = n(24),
+            o = n(25),
             a = n(41),
             s = n(42),
-            u = n(9),
+            u = n(8),
             l = n(7),
             c = n(1);
 
         function f() {
             return (f = Object.assign ? Object.assign.bind() : function(e) {
                 for (var t = 1; t < arguments.length; t++) {
                     var n = arguments[t];
@@ -3468,15 +3468,15 @@
             return i
         }))
     }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return o
         }));
-        var r = n(8);
+        var r = n(9);
 
         function i(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
@@ -3588,16 +3588,16 @@
             return d
         })), n.d(t, "b", (function() {
             return h
         })), n.d(t, "c", (function() {
             return v
         }));
         n(15);
-        var r = n(9),
-            i = n(27),
+        var r = n(8),
+            i = n(28),
             o = n(1),
             a = n(11),
             s = n(7);
 
         function u() {
             return (u = Object.assign ? Object.assign.bind() : function(e) {
                 for (var t = 1; t < arguments.length; t++) {
@@ -5574,15 +5574,15 @@
 
         function r(e) {
             return e.replace(/[\t\n\r ]+/g, " ").replace(/^ | $/g, "").toLowerCase().toUpperCase()
         }
         n.d(t, "a", (function() {
             return r
         }))
-    }, function(e, t, n) {
+    }, , function(e, t, n) {
         "use strict";
 
         function r(e, t) {
             for (var n = 0; n < t.length; n++) {
                 var r = t[n];
                 r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
             }
@@ -6442,15 +6442,15 @@
                 var r = t[n];
                 r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
             }
         }
         e.exports = function(e, t, r) {
             return t && n(e.prototype, t), r && n(e, r), e
         }
-    }, , function(e, t, n) {
+    }, function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return i
         }));
         var r = n(63),
             i = function(e, t, n, i) {
                 "function" === typeof t && "function" !== typeof n && (i = n, n = t, t = null), Object(r.b)(e, t, (function(e, t) {
@@ -6740,16 +6740,16 @@
         }))
     }, function(e, t, n) {
         var r = n(262),
             i = n(121),
             o = n(35),
             a = n(36),
             s = n(72),
-            u = n(26),
-            l = n(28),
+            u = n(27),
+            l = n(29),
             c = {
                 exports: {}
             };
 
         function f(e) {
             return e instanceof Map ? e.clear = e.delete = e.set = function() {
                 throw new Error("map is read-only")
@@ -7855,16 +7855,16 @@
                     column: n.column || null,
                     offset: n.offset > -1 ? n.offset : null
                 }
             }
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = function() {
                 function e(t) {
                     r(this, e);
                     for (var n = {}, i = this._getOverriddenMethods(this, n), o = 0, a = Object.keys(i); o < a.length; o++) {
                         var s = a[o];
                         "function" === typeof i[s] && (n[s] = t[s], t[s] = i[s])
                     }
@@ -11120,16 +11120,16 @@
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(271),
             a = n(98),
             s = n(272),
             u = n(99),
             l = a.CODE_POINTS,
             c = a.CODE_POINT_SEQUENCES,
             f = {
@@ -12372,15 +12372,15 @@
                     break
                 }
             }
             return e.length > 0 && !n && (e[e.length - 1][1]._gfmAutolinkLiteralWalkedInto = !0), n
         }
         p[43] = d, p[45] = d, p[46] = d, p[95] = d, p[72] = [d, f], p[104] = [d, f], p[87] = [d, c], p[119] = [d, c];
         n(43);
-        var w = n(8),
+        var w = n(9),
             O = n(69),
             A = n(12),
             k = n(23),
             D = {
                 tokenize: function(e, t, n) {
                     var r = this;
                     return Object(A.a)(e, (function(e) {
@@ -13806,15 +13806,15 @@
         function N(e) {
             return e.line && e.column ? e : null
         }
 
         function x(e) {
             return "messages" in e
         }
-        var R = n(8),
+        var R = n(9),
             L = n(118),
             M = n(84),
             P = n.n(M),
             F = n(31),
             B = O,
             j = L.a,
             U = {}.hasOwnProperty,
@@ -14632,16 +14632,16 @@
             abandonedHeadElementChild: "abandoned-head-element-child",
             misplacedStartTagForHeadElement: "misplaced-start-tag-for-head-element",
             nestedNoscriptInHead: "nested-noscript-in-head",
             eofInElementThatCanContainOnlyText: "eof-in-element-that-can-contain-only-text"
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(35),
             a = n(36),
             s = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e, i) {
@@ -15215,16 +15215,16 @@
             o = n(96),
             a = n(267);
         e.exports = function(e, t) {
             return r(e) || i(e, t) || o(e, t) || a()
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(35),
             a = n(36),
             s = n(38),
             u = n(74),
             l = n(123),
             c = function(e) {
                 o(n, e);
@@ -15302,16 +15302,16 @@
                         })), n
                     }
                 }]), n
             }(s);
         e.exports = c
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(35),
             a = n(36),
             s = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e) {
@@ -21247,16 +21247,16 @@
                 return n.apply(null, [e].concat(t))
             }, "undefined" !== typeof console && "function" === typeof console.log && (t.printf = function() {
                 console.log(n.apply(null, arguments))
             })
         }()
     }, function(e, t, n) {
         "use strict";
-        var r, i, o, a, s, u, l, c, f, d, p, h, m, g, v, b, E, y, _, T, w, O, A, k, D, C, S = n(26),
-            I = n(28),
+        var r, i, o, a, s, u, l, c, f, d, p, h, m, g, v, b, E, y, _, T, w, O, A, k, D, C, S = n(27),
+            I = n(29),
             N = n(73),
             x = n(74),
             R = n(273),
             L = n(274),
             M = n(275),
             P = n(277),
             F = n(38),
@@ -41063,16 +41063,16 @@
     }, function(e, t) {
         e.exports = function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(98),
             a = n(99),
             s = o.CODE_POINTS,
             u = function() {
                 function e() {
                     r(this, e), this.html = null, this.pos = -1, this.lastGapPos = -1, this.lastCharPos = -1, this.gapStack = [], this.skipNextNewLine = !1, this.lastChunkWritten = !1, this.endOfChunkHit = !1, this.bufferWaterline = 65536
                 }
@@ -41129,16 +41129,16 @@
             }();
         e.exports = u
     }, function(e, t, n) {
         "use strict";
         e.exports = new Uint16Array([4, 52, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 106, 303, 412, 810, 1432, 1701, 1796, 1987, 2114, 2360, 2420, 2484, 3170, 3251, 4140, 4393, 4575, 4610, 5106, 5512, 5728, 6117, 6274, 6315, 6345, 6427, 6516, 7002, 7910, 8733, 9323, 9870, 10170, 10631, 10893, 11318, 11386, 11467, 12773, 13092, 14474, 14922, 15448, 15542, 16419, 17666, 18166, 18611, 19004, 19095, 19298, 19397, 4, 16, 69, 77, 97, 98, 99, 102, 103, 108, 109, 110, 111, 112, 114, 115, 116, 117, 140, 150, 158, 169, 176, 194, 199, 210, 216, 222, 226, 242, 256, 266, 283, 294, 108, 105, 103, 5, 198, 1, 59, 148, 1, 198, 80, 5, 38, 1, 59, 156, 1, 38, 99, 117, 116, 101, 5, 193, 1, 59, 167, 1, 193, 114, 101, 118, 101, 59, 1, 258, 4, 2, 105, 121, 182, 191, 114, 99, 5, 194, 1, 59, 189, 1, 194, 59, 1, 1040, 114, 59, 3, 55349, 56580, 114, 97, 118, 101, 5, 192, 1, 59, 208, 1, 192, 112, 104, 97, 59, 1, 913, 97, 99, 114, 59, 1, 256, 100, 59, 1, 10835, 4, 2, 103, 112, 232, 237, 111, 110, 59, 1, 260, 102, 59, 3, 55349, 56632, 112, 108, 121, 70, 117, 110, 99, 116, 105, 111, 110, 59, 1, 8289, 105, 110, 103, 5, 197, 1, 59, 264, 1, 197, 4, 2, 99, 115, 272, 277, 114, 59, 3, 55349, 56476, 105, 103, 110, 59, 1, 8788, 105, 108, 100, 101, 5, 195, 1, 59, 292, 1, 195, 109, 108, 5, 196, 1, 59, 301, 1, 196, 4, 8, 97, 99, 101, 102, 111, 114, 115, 117, 321, 350, 354, 383, 388, 394, 400, 405, 4, 2, 99, 114, 327, 336, 107, 115, 108, 97, 115, 104, 59, 1, 8726, 4, 2, 118, 119, 342, 345, 59, 1, 10983, 101, 100, 59, 1, 8966, 121, 59, 1, 1041, 4, 3, 99, 114, 116, 362, 369, 379, 97, 117, 115, 101, 59, 1, 8757, 110, 111, 117, 108, 108, 105, 115, 59, 1, 8492, 97, 59, 1, 914, 114, 59, 3, 55349, 56581, 112, 102, 59, 3, 55349, 56633, 101, 118, 101, 59, 1, 728, 99, 114, 59, 1, 8492, 109, 112, 101, 113, 59, 1, 8782, 4, 14, 72, 79, 97, 99, 100, 101, 102, 104, 105, 108, 111, 114, 115, 117, 442, 447, 456, 504, 542, 547, 569, 573, 577, 616, 678, 784, 790, 796, 99, 121, 59, 1, 1063, 80, 89, 5, 169, 1, 59, 454, 1, 169, 4, 3, 99, 112, 121, 464, 470, 497, 117, 116, 101, 59, 1, 262, 4, 2, 59, 105, 476, 478, 1, 8914, 116, 97, 108, 68, 105, 102, 102, 101, 114, 101, 110, 116, 105, 97, 108, 68, 59, 1, 8517, 108, 101, 121, 115, 59, 1, 8493, 4, 4, 97, 101, 105, 111, 514, 520, 530, 535, 114, 111, 110, 59, 1, 268, 100, 105, 108, 5, 199, 1, 59, 528, 1, 199, 114, 99, 59, 1, 264, 110, 105, 110, 116, 59, 1, 8752, 111, 116, 59, 1, 266, 4, 2, 100, 110, 553, 560, 105, 108, 108, 97, 59, 1, 184, 116, 101, 114, 68, 111, 116, 59, 1, 183, 114, 59, 1, 8493, 105, 59, 1, 935, 114, 99, 108, 101, 4, 4, 68, 77, 80, 84, 591, 596, 603, 609, 111, 116, 59, 1, 8857, 105, 110, 117, 115, 59, 1, 8854, 108, 117, 115, 59, 1, 8853, 105, 109, 101, 115, 59, 1, 8855, 111, 4, 2, 99, 115, 623, 646, 107, 119, 105, 115, 101, 67, 111, 110, 116, 111, 117, 114, 73, 110, 116, 101, 103, 114, 97, 108, 59, 1, 8754, 101, 67, 117, 114, 108, 121, 4, 2, 68, 81, 658, 671, 111, 117, 98, 108, 101, 81, 117, 111, 116, 101, 59, 1, 8221, 117, 111, 116, 101, 59, 1, 8217, 4, 4, 108, 110, 112, 117, 688, 701, 736, 753, 111, 110, 4, 2, 59, 101, 696, 698, 1, 8759, 59, 1, 10868, 4, 3, 103, 105, 116, 709, 717, 722, 114, 117, 101, 110, 116, 59, 1, 8801, 110, 116, 59, 1, 8751, 111, 117, 114, 73, 110, 116, 101, 103, 114, 97, 108, 59, 1, 8750, 4, 2, 102, 114, 742, 745, 59, 1, 8450, 111, 100, 117, 99, 116, 59, 1, 8720, 110, 116, 101, 114, 67, 108, 111, 99, 107, 119, 105, 115, 101, 67, 111, 110, 116, 111, 117, 114, 73, 110, 116, 101, 103, 114, 97, 108, 59, 1, 8755, 111, 115, 115, 59, 1, 10799, 99, 114, 59, 3, 55349, 56478, 112, 4, 2, 59, 67, 803, 805, 1, 8915, 97, 112, 59, 1, 8781, 4, 11, 68, 74, 83, 90, 97, 99, 101, 102, 105, 111, 115, 834, 850, 855, 860, 865, 888, 903, 916, 921, 1011, 1415, 4, 2, 59, 111, 840, 842, 1, 8517, 116, 114, 97, 104, 100, 59, 1, 10513, 99, 121, 59, 1, 1026, 99, 121, 59, 1, 1029, 99, 121, 59, 1, 1039, 4, 3, 103, 114, 115, 873, 879, 883, 103, 101, 114, 59, 1, 8225, 114, 59, 1, 8609, 104, 118, 59, 1, 10980, 4, 2, 97, 121, 894, 900, 114, 111, 110, 59, 1, 270, 59, 1, 1044, 108, 4, 2, 59, 116, 910, 912, 1, 8711, 97, 59, 1, 916, 114, 59, 3, 55349, 56583, 4, 2, 97, 102, 927, 998, 4, 2, 99, 109, 933, 992, 114, 105, 116, 105, 99, 97, 108, 4, 4, 65, 68, 71, 84, 950, 957, 978, 985, 99, 117, 116, 101, 59, 1, 180, 111, 4, 2, 116, 117, 964, 967, 59, 1, 729, 98, 108, 101, 65, 99, 117, 116, 101, 59, 1, 733, 114, 97, 118, 101, 59, 1, 96, 105, 108, 100, 101, 59, 1, 732, 111, 110, 100, 59, 1, 8900, 102, 101, 114, 101, 110, 116, 105, 97, 108, 68, 59, 1, 8518, 4, 4, 112, 116, 117, 119, 1021, 1026, 1048, 1249, 102, 59, 3, 55349, 56635, 4, 3, 59, 68, 69, 1034, 1036, 1041, 1, 168, 111, 116, 59, 1, 8412, 113, 117, 97, 108, 59, 1, 8784, 98, 108, 101, 4, 6, 67, 68, 76, 82, 85, 86, 1065, 1082, 1101, 1189, 1211, 1236, 111, 110, 116, 111, 117, 114, 73, 110, 116, 101, 103, 114, 97, 108, 59, 1, 8751, 111, 4, 2, 116, 119, 1089, 1092, 59, 1, 168, 110, 65, 114, 114, 111, 119, 59, 1, 8659, 4, 2, 101, 111, 1107, 1141, 102, 116, 4, 3, 65, 82, 84, 1117, 1124, 1136, 114, 114, 111, 119, 59, 1, 8656, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 8660, 101, 101, 59, 1, 10980, 110, 103, 4, 2, 76, 82, 1149, 1177, 101, 102, 116, 4, 2, 65, 82, 1158, 1165, 114, 114, 111, 119, 59, 1, 10232, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 10234, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 10233, 105, 103, 104, 116, 4, 2, 65, 84, 1199, 1206, 114, 114, 111, 119, 59, 1, 8658, 101, 101, 59, 1, 8872, 112, 4, 2, 65, 68, 1218, 1225, 114, 114, 111, 119, 59, 1, 8657, 111, 119, 110, 65, 114, 114, 111, 119, 59, 1, 8661, 101, 114, 116, 105, 99, 97, 108, 66, 97, 114, 59, 1, 8741, 110, 4, 6, 65, 66, 76, 82, 84, 97, 1264, 1292, 1299, 1352, 1391, 1408, 114, 114, 111, 119, 4, 3, 59, 66, 85, 1276, 1278, 1283, 1, 8595, 97, 114, 59, 1, 10515, 112, 65, 114, 114, 111, 119, 59, 1, 8693, 114, 101, 118, 101, 59, 1, 785, 101, 102, 116, 4, 3, 82, 84, 86, 1310, 1323, 1334, 105, 103, 104, 116, 86, 101, 99, 116, 111, 114, 59, 1, 10576, 101, 101, 86, 101, 99, 116, 111, 114, 59, 1, 10590, 101, 99, 116, 111, 114, 4, 2, 59, 66, 1345, 1347, 1, 8637, 97, 114, 59, 1, 10582, 105, 103, 104, 116, 4, 2, 84, 86, 1362, 1373, 101, 101, 86, 101, 99, 116, 111, 114, 59, 1, 10591, 101, 99, 116, 111, 114, 4, 2, 59, 66, 1384, 1386, 1, 8641, 97, 114, 59, 1, 10583, 101, 101, 4, 2, 59, 65, 1399, 1401, 1, 8868, 114, 114, 111, 119, 59, 1, 8615, 114, 114, 111, 119, 59, 1, 8659, 4, 2, 99, 116, 1421, 1426, 114, 59, 3, 55349, 56479, 114, 111, 107, 59, 1, 272, 4, 16, 78, 84, 97, 99, 100, 102, 103, 108, 109, 111, 112, 113, 115, 116, 117, 120, 1466, 1470, 1478, 1489, 1515, 1520, 1525, 1536, 1544, 1593, 1609, 1617, 1650, 1664, 1668, 1677, 71, 59, 1, 330, 72, 5, 208, 1, 59, 1476, 1, 208, 99, 117, 116, 101, 5, 201, 1, 59, 1487, 1, 201, 4, 3, 97, 105, 121, 1497, 1503, 1512, 114, 111, 110, 59, 1, 282, 114, 99, 5, 202, 1, 59, 1510, 1, 202, 59, 1, 1069, 111, 116, 59, 1, 278, 114, 59, 3, 55349, 56584, 114, 97, 118, 101, 5, 200, 1, 59, 1534, 1, 200, 101, 109, 101, 110, 116, 59, 1, 8712, 4, 2, 97, 112, 1550, 1555, 99, 114, 59, 1, 274, 116, 121, 4, 2, 83, 86, 1563, 1576, 109, 97, 108, 108, 83, 113, 117, 97, 114, 101, 59, 1, 9723, 101, 114, 121, 83, 109, 97, 108, 108, 83, 113, 117, 97, 114, 101, 59, 1, 9643, 4, 2, 103, 112, 1599, 1604, 111, 110, 59, 1, 280, 102, 59, 3, 55349, 56636, 115, 105, 108, 111, 110, 59, 1, 917, 117, 4, 2, 97, 105, 1624, 1640, 108, 4, 2, 59, 84, 1631, 1633, 1, 10869, 105, 108, 100, 101, 59, 1, 8770, 108, 105, 98, 114, 105, 117, 109, 59, 1, 8652, 4, 2, 99, 105, 1656, 1660, 114, 59, 1, 8496, 109, 59, 1, 10867, 97, 59, 1, 919, 109, 108, 5, 203, 1, 59, 1675, 1, 203, 4, 2, 105, 112, 1683, 1689, 115, 116, 115, 59, 1, 8707, 111, 110, 101, 110, 116, 105, 97, 108, 69, 59, 1, 8519, 4, 5, 99, 102, 105, 111, 115, 1713, 1717, 1722, 1762, 1791, 121, 59, 1, 1060, 114, 59, 3, 55349, 56585, 108, 108, 101, 100, 4, 2, 83, 86, 1732, 1745, 109, 97, 108, 108, 83, 113, 117, 97, 114, 101, 59, 1, 9724, 101, 114, 121, 83, 109, 97, 108, 108, 83, 113, 117, 97, 114, 101, 59, 1, 9642, 4, 3, 112, 114, 117, 1770, 1775, 1781, 102, 59, 3, 55349, 56637, 65, 108, 108, 59, 1, 8704, 114, 105, 101, 114, 116, 114, 102, 59, 1, 8497, 99, 114, 59, 1, 8497, 4, 12, 74, 84, 97, 98, 99, 100, 102, 103, 111, 114, 115, 116, 1822, 1827, 1834, 1848, 1855, 1877, 1882, 1887, 1890, 1896, 1978, 1984, 99, 121, 59, 1, 1027, 5, 62, 1, 59, 1832, 1, 62, 109, 109, 97, 4, 2, 59, 100, 1843, 1845, 1, 915, 59, 1, 988, 114, 101, 118, 101, 59, 1, 286, 4, 3, 101, 105, 121, 1863, 1869, 1874, 100, 105, 108, 59, 1, 290, 114, 99, 59, 1, 284, 59, 1, 1043, 111, 116, 59, 1, 288, 114, 59, 3, 55349, 56586, 59, 1, 8921, 112, 102, 59, 3, 55349, 56638, 101, 97, 116, 101, 114, 4, 6, 69, 70, 71, 76, 83, 84, 1915, 1933, 1944, 1953, 1959, 1971, 113, 117, 97, 108, 4, 2, 59, 76, 1925, 1927, 1, 8805, 101, 115, 115, 59, 1, 8923, 117, 108, 108, 69, 113, 117, 97, 108, 59, 1, 8807, 114, 101, 97, 116, 101, 114, 59, 1, 10914, 101, 115, 115, 59, 1, 8823, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 1, 10878, 105, 108, 100, 101, 59, 1, 8819, 99, 114, 59, 3, 55349, 56482, 59, 1, 8811, 4, 8, 65, 97, 99, 102, 105, 111, 115, 117, 2005, 2012, 2026, 2032, 2036, 2049, 2073, 2089, 82, 68, 99, 121, 59, 1, 1066, 4, 2, 99, 116, 2018, 2023, 101, 107, 59, 1, 711, 59, 1, 94, 105, 114, 99, 59, 1, 292, 114, 59, 1, 8460, 108, 98, 101, 114, 116, 83, 112, 97, 99, 101, 59, 1, 8459, 4, 2, 112, 114, 2055, 2059, 102, 59, 1, 8461, 105, 122, 111, 110, 116, 97, 108, 76, 105, 110, 101, 59, 1, 9472, 4, 2, 99, 116, 2079, 2083, 114, 59, 1, 8459, 114, 111, 107, 59, 1, 294, 109, 112, 4, 2, 68, 69, 2097, 2107, 111, 119, 110, 72, 117, 109, 112, 59, 1, 8782, 113, 117, 97, 108, 59, 1, 8783, 4, 14, 69, 74, 79, 97, 99, 100, 102, 103, 109, 110, 111, 115, 116, 117, 2144, 2149, 2155, 2160, 2171, 2189, 2194, 2198, 2209, 2245, 2307, 2329, 2334, 2341, 99, 121, 59, 1, 1045, 108, 105, 103, 59, 1, 306, 99, 121, 59, 1, 1025, 99, 117, 116, 101, 5, 205, 1, 59, 2169, 1, 205, 4, 2, 105, 121, 2177, 2186, 114, 99, 5, 206, 1, 59, 2184, 1, 206, 59, 1, 1048, 111, 116, 59, 1, 304, 114, 59, 1, 8465, 114, 97, 118, 101, 5, 204, 1, 59, 2207, 1, 204, 4, 3, 59, 97, 112, 2217, 2219, 2238, 1, 8465, 4, 2, 99, 103, 2225, 2229, 114, 59, 1, 298, 105, 110, 97, 114, 121, 73, 59, 1, 8520, 108, 105, 101, 115, 59, 1, 8658, 4, 2, 116, 118, 2251, 2281, 4, 2, 59, 101, 2257, 2259, 1, 8748, 4, 2, 103, 114, 2265, 2271, 114, 97, 108, 59, 1, 8747, 115, 101, 99, 116, 105, 111, 110, 59, 1, 8898, 105, 115, 105, 98, 108, 101, 4, 2, 67, 84, 2293, 2300, 111, 109, 109, 97, 59, 1, 8291, 105, 109, 101, 115, 59, 1, 8290, 4, 3, 103, 112, 116, 2315, 2320, 2325, 111, 110, 59, 1, 302, 102, 59, 3, 55349, 56640, 97, 59, 1, 921, 99, 114, 59, 1, 8464, 105, 108, 100, 101, 59, 1, 296, 4, 2, 107, 109, 2347, 2352, 99, 121, 59, 1, 1030, 108, 5, 207, 1, 59, 2358, 1, 207, 4, 5, 99, 102, 111, 115, 117, 2372, 2386, 2391, 2397, 2414, 4, 2, 105, 121, 2378, 2383, 114, 99, 59, 1, 308, 59, 1, 1049, 114, 59, 3, 55349, 56589, 112, 102, 59, 3, 55349, 56641, 4, 2, 99, 101, 2403, 2408, 114, 59, 3, 55349, 56485, 114, 99, 121, 59, 1, 1032, 107, 99, 121, 59, 1, 1028, 4, 7, 72, 74, 97, 99, 102, 111, 115, 2436, 2441, 2446, 2452, 2467, 2472, 2478, 99, 121, 59, 1, 1061, 99, 121, 59, 1, 1036, 112, 112, 97, 59, 1, 922, 4, 2, 101, 121, 2458, 2464, 100, 105, 108, 59, 1, 310, 59, 1, 1050, 114, 59, 3, 55349, 56590, 112, 102, 59, 3, 55349, 56642, 99, 114, 59, 3, 55349, 56486, 4, 11, 74, 84, 97, 99, 101, 102, 108, 109, 111, 115, 116, 2508, 2513, 2520, 2562, 2585, 2981, 2986, 3004, 3011, 3146, 3167, 99, 121, 59, 1, 1033, 5, 60, 1, 59, 2518, 1, 60, 4, 5, 99, 109, 110, 112, 114, 2532, 2538, 2544, 2548, 2558, 117, 116, 101, 59, 1, 313, 98, 100, 97, 59, 1, 923, 103, 59, 1, 10218, 108, 97, 99, 101, 116, 114, 102, 59, 1, 8466, 114, 59, 1, 8606, 4, 3, 97, 101, 121, 2570, 2576, 2582, 114, 111, 110, 59, 1, 317, 100, 105, 108, 59, 1, 315, 59, 1, 1051, 4, 2, 102, 115, 2591, 2907, 116, 4, 10, 65, 67, 68, 70, 82, 84, 85, 86, 97, 114, 2614, 2663, 2672, 2728, 2735, 2760, 2820, 2870, 2888, 2895, 4, 2, 110, 114, 2620, 2633, 103, 108, 101, 66, 114, 97, 99, 107, 101, 116, 59, 1, 10216, 114, 111, 119, 4, 3, 59, 66, 82, 2644, 2646, 2651, 1, 8592, 97, 114, 59, 1, 8676, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 8646, 101, 105, 108, 105, 110, 103, 59, 1, 8968, 111, 4, 2, 117, 119, 2679, 2692, 98, 108, 101, 66, 114, 97, 99, 107, 101, 116, 59, 1, 10214, 110, 4, 2, 84, 86, 2699, 2710, 101, 101, 86, 101, 99, 116, 111, 114, 59, 1, 10593, 101, 99, 116, 111, 114, 4, 2, 59, 66, 2721, 2723, 1, 8643, 97, 114, 59, 1, 10585, 108, 111, 111, 114, 59, 1, 8970, 105, 103, 104, 116, 4, 2, 65, 86, 2745, 2752, 114, 114, 111, 119, 59, 1, 8596, 101, 99, 116, 111, 114, 59, 1, 10574, 4, 2, 101, 114, 2766, 2792, 101, 4, 3, 59, 65, 86, 2775, 2777, 2784, 1, 8867, 114, 114, 111, 119, 59, 1, 8612, 101, 99, 116, 111, 114, 59, 1, 10586, 105, 97, 110, 103, 108, 101, 4, 3, 59, 66, 69, 2806, 2808, 2813, 1, 8882, 97, 114, 59, 1, 10703, 113, 117, 97, 108, 59, 1, 8884, 112, 4, 3, 68, 84, 86, 2829, 2841, 2852, 111, 119, 110, 86, 101, 99, 116, 111, 114, 59, 1, 10577, 101, 101, 86, 101, 99, 116, 111, 114, 59, 1, 10592, 101, 99, 116, 111, 114, 4, 2, 59, 66, 2863, 2865, 1, 8639, 97, 114, 59, 1, 10584, 101, 99, 116, 111, 114, 4, 2, 59, 66, 2881, 2883, 1, 8636, 97, 114, 59, 1, 10578, 114, 114, 111, 119, 59, 1, 8656, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8660, 115, 4, 6, 69, 70, 71, 76, 83, 84, 2922, 2936, 2947, 2956, 2962, 2974, 113, 117, 97, 108, 71, 114, 101, 97, 116, 101, 114, 59, 1, 8922, 117, 108, 108, 69, 113, 117, 97, 108, 59, 1, 8806, 114, 101, 97, 116, 101, 114, 59, 1, 8822, 101, 115, 115, 59, 1, 10913, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 1, 10877, 105, 108, 100, 101, 59, 1, 8818, 114, 59, 3, 55349, 56591, 4, 2, 59, 101, 2992, 2994, 1, 8920, 102, 116, 97, 114, 114, 111, 119, 59, 1, 8666, 105, 100, 111, 116, 59, 1, 319, 4, 3, 110, 112, 119, 3019, 3110, 3115, 103, 4, 4, 76, 82, 108, 114, 3030, 3058, 3070, 3098, 101, 102, 116, 4, 2, 65, 82, 3039, 3046, 114, 114, 111, 119, 59, 1, 10229, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 10231, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 10230, 101, 102, 116, 4, 2, 97, 114, 3079, 3086, 114, 114, 111, 119, 59, 1, 10232, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 10234, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 10233, 102, 59, 3, 55349, 56643, 101, 114, 4, 2, 76, 82, 3123, 3134, 101, 102, 116, 65, 114, 114, 111, 119, 59, 1, 8601, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 8600, 4, 3, 99, 104, 116, 3154, 3158, 3161, 114, 59, 1, 8466, 59, 1, 8624, 114, 111, 107, 59, 1, 321, 59, 1, 8810, 4, 8, 97, 99, 101, 102, 105, 111, 115, 117, 3188, 3192, 3196, 3222, 3227, 3237, 3243, 3248, 112, 59, 1, 10501, 121, 59, 1, 1052, 4, 2, 100, 108, 3202, 3213, 105, 117, 109, 83, 112, 97, 99, 101, 59, 1, 8287, 108, 105, 110, 116, 114, 102, 59, 1, 8499, 114, 59, 3, 55349, 56592, 110, 117, 115, 80, 108, 117, 115, 59, 1, 8723, 112, 102, 59, 3, 55349, 56644, 99, 114, 59, 1, 8499, 59, 1, 924, 4, 9, 74, 97, 99, 101, 102, 111, 115, 116, 117, 3271, 3276, 3283, 3306, 3422, 3427, 4120, 4126, 4137, 99, 121, 59, 1, 1034, 99, 117, 116, 101, 59, 1, 323, 4, 3, 97, 101, 121, 3291, 3297, 3303, 114, 111, 110, 59, 1, 327, 100, 105, 108, 59, 1, 325, 59, 1, 1053, 4, 3, 103, 115, 119, 3314, 3380, 3415, 97, 116, 105, 118, 101, 4, 3, 77, 84, 86, 3327, 3340, 3365, 101, 100, 105, 117, 109, 83, 112, 97, 99, 101, 59, 1, 8203, 104, 105, 4, 2, 99, 110, 3348, 3357, 107, 83, 112, 97, 99, 101, 59, 1, 8203, 83, 112, 97, 99, 101, 59, 1, 8203, 101, 114, 121, 84, 104, 105, 110, 83, 112, 97, 99, 101, 59, 1, 8203, 116, 101, 100, 4, 2, 71, 76, 3389, 3405, 114, 101, 97, 116, 101, 114, 71, 114, 101, 97, 116, 101, 114, 59, 1, 8811, 101, 115, 115, 76, 101, 115, 115, 59, 1, 8810, 76, 105, 110, 101, 59, 1, 10, 114, 59, 3, 55349, 56593, 4, 4, 66, 110, 112, 116, 3437, 3444, 3460, 3464, 114, 101, 97, 107, 59, 1, 8288, 66, 114, 101, 97, 107, 105, 110, 103, 83, 112, 97, 99, 101, 59, 1, 160, 102, 59, 1, 8469, 4, 13, 59, 67, 68, 69, 71, 72, 76, 78, 80, 82, 83, 84, 86, 3492, 3494, 3517, 3536, 3578, 3657, 3685, 3784, 3823, 3860, 3915, 4066, 4107, 1, 10988, 4, 2, 111, 117, 3500, 3510, 110, 103, 114, 117, 101, 110, 116, 59, 1, 8802, 112, 67, 97, 112, 59, 1, 8813, 111, 117, 98, 108, 101, 86, 101, 114, 116, 105, 99, 97, 108, 66, 97, 114, 59, 1, 8742, 4, 3, 108, 113, 120, 3544, 3552, 3571, 101, 109, 101, 110, 116, 59, 1, 8713, 117, 97, 108, 4, 2, 59, 84, 3561, 3563, 1, 8800, 105, 108, 100, 101, 59, 3, 8770, 824, 105, 115, 116, 115, 59, 1, 8708, 114, 101, 97, 116, 101, 114, 4, 7, 59, 69, 70, 71, 76, 83, 84, 3600, 3602, 3609, 3621, 3631, 3637, 3650, 1, 8815, 113, 117, 97, 108, 59, 1, 8817, 117, 108, 108, 69, 113, 117, 97, 108, 59, 3, 8807, 824, 114, 101, 97, 116, 101, 114, 59, 3, 8811, 824, 101, 115, 115, 59, 1, 8825, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 3, 10878, 824, 105, 108, 100, 101, 59, 1, 8821, 117, 109, 112, 4, 2, 68, 69, 3666, 3677, 111, 119, 110, 72, 117, 109, 112, 59, 3, 8782, 824, 113, 117, 97, 108, 59, 3, 8783, 824, 101, 4, 2, 102, 115, 3692, 3724, 116, 84, 114, 105, 97, 110, 103, 108, 101, 4, 3, 59, 66, 69, 3709, 3711, 3717, 1, 8938, 97, 114, 59, 3, 10703, 824, 113, 117, 97, 108, 59, 1, 8940, 115, 4, 6, 59, 69, 71, 76, 83, 84, 3739, 3741, 3748, 3757, 3764, 3777, 1, 8814, 113, 117, 97, 108, 59, 1, 8816, 114, 101, 97, 116, 101, 114, 59, 1, 8824, 101, 115, 115, 59, 3, 8810, 824, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 3, 10877, 824, 105, 108, 100, 101, 59, 1, 8820, 101, 115, 116, 101, 100, 4, 2, 71, 76, 3795, 3812, 114, 101, 97, 116, 101, 114, 71, 114, 101, 97, 116, 101, 114, 59, 3, 10914, 824, 101, 115, 115, 76, 101, 115, 115, 59, 3, 10913, 824, 114, 101, 99, 101, 100, 101, 115, 4, 3, 59, 69, 83, 3838, 3840, 3848, 1, 8832, 113, 117, 97, 108, 59, 3, 10927, 824, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 1, 8928, 4, 2, 101, 105, 3866, 3881, 118, 101, 114, 115, 101, 69, 108, 101, 109, 101, 110, 116, 59, 1, 8716, 103, 104, 116, 84, 114, 105, 97, 110, 103, 108, 101, 4, 3, 59, 66, 69, 3900, 3902, 3908, 1, 8939, 97, 114, 59, 3, 10704, 824, 113, 117, 97, 108, 59, 1, 8941, 4, 2, 113, 117, 3921, 3973, 117, 97, 114, 101, 83, 117, 4, 2, 98, 112, 3933, 3952, 115, 101, 116, 4, 2, 59, 69, 3942, 3945, 3, 8847, 824, 113, 117, 97, 108, 59, 1, 8930, 101, 114, 115, 101, 116, 4, 2, 59, 69, 3963, 3966, 3, 8848, 824, 113, 117, 97, 108, 59, 1, 8931, 4, 3, 98, 99, 112, 3981, 4e3, 4045, 115, 101, 116, 4, 2, 59, 69, 3990, 3993, 3, 8834, 8402, 113, 117, 97, 108, 59, 1, 8840, 99, 101, 101, 100, 115, 4, 4, 59, 69, 83, 84, 4015, 4017, 4025, 4037, 1, 8833, 113, 117, 97, 108, 59, 3, 10928, 824, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 1, 8929, 105, 108, 100, 101, 59, 3, 8831, 824, 101, 114, 115, 101, 116, 4, 2, 59, 69, 4056, 4059, 3, 8835, 8402, 113, 117, 97, 108, 59, 1, 8841, 105, 108, 100, 101, 4, 4, 59, 69, 70, 84, 4080, 4082, 4089, 4100, 1, 8769, 113, 117, 97, 108, 59, 1, 8772, 117, 108, 108, 69, 113, 117, 97, 108, 59, 1, 8775, 105, 108, 100, 101, 59, 1, 8777, 101, 114, 116, 105, 99, 97, 108, 66, 97, 114, 59, 1, 8740, 99, 114, 59, 3, 55349, 56489, 105, 108, 100, 101, 5, 209, 1, 59, 4135, 1, 209, 59, 1, 925, 4, 14, 69, 97, 99, 100, 102, 103, 109, 111, 112, 114, 115, 116, 117, 118, 4170, 4176, 4187, 4205, 4212, 4217, 4228, 4253, 4259, 4292, 4295, 4316, 4337, 4346, 108, 105, 103, 59, 1, 338, 99, 117, 116, 101, 5, 211, 1, 59, 4185, 1, 211, 4, 2, 105, 121, 4193, 4202, 114, 99, 5, 212, 1, 59, 4200, 1, 212, 59, 1, 1054, 98, 108, 97, 99, 59, 1, 336, 114, 59, 3, 55349, 56594, 114, 97, 118, 101, 5, 210, 1, 59, 4226, 1, 210, 4, 3, 97, 101, 105, 4236, 4241, 4246, 99, 114, 59, 1, 332, 103, 97, 59, 1, 937, 99, 114, 111, 110, 59, 1, 927, 112, 102, 59, 3, 55349, 56646, 101, 110, 67, 117, 114, 108, 121, 4, 2, 68, 81, 4272, 4285, 111, 117, 98, 108, 101, 81, 117, 111, 116, 101, 59, 1, 8220, 117, 111, 116, 101, 59, 1, 8216, 59, 1, 10836, 4, 2, 99, 108, 4301, 4306, 114, 59, 3, 55349, 56490, 97, 115, 104, 5, 216, 1, 59, 4314, 1, 216, 105, 4, 2, 108, 109, 4323, 4332, 100, 101, 5, 213, 1, 59, 4330, 1, 213, 101, 115, 59, 1, 10807, 109, 108, 5, 214, 1, 59, 4344, 1, 214, 101, 114, 4, 2, 66, 80, 4354, 4380, 4, 2, 97, 114, 4360, 4364, 114, 59, 1, 8254, 97, 99, 4, 2, 101, 107, 4372, 4375, 59, 1, 9182, 101, 116, 59, 1, 9140, 97, 114, 101, 110, 116, 104, 101, 115, 105, 115, 59, 1, 9180, 4, 9, 97, 99, 102, 104, 105, 108, 111, 114, 115, 4413, 4422, 4426, 4431, 4435, 4438, 4448, 4471, 4561, 114, 116, 105, 97, 108, 68, 59, 1, 8706, 121, 59, 1, 1055, 114, 59, 3, 55349, 56595, 105, 59, 1, 934, 59, 1, 928, 117, 115, 77, 105, 110, 117, 115, 59, 1, 177, 4, 2, 105, 112, 4454, 4467, 110, 99, 97, 114, 101, 112, 108, 97, 110, 101, 59, 1, 8460, 102, 59, 1, 8473, 4, 4, 59, 101, 105, 111, 4481, 4483, 4526, 4531, 1, 10939, 99, 101, 100, 101, 115, 4, 4, 59, 69, 83, 84, 4498, 4500, 4507, 4519, 1, 8826, 113, 117, 97, 108, 59, 1, 10927, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 1, 8828, 105, 108, 100, 101, 59, 1, 8830, 109, 101, 59, 1, 8243, 4, 2, 100, 112, 4537, 4543, 117, 99, 116, 59, 1, 8719, 111, 114, 116, 105, 111, 110, 4, 2, 59, 97, 4555, 4557, 1, 8759, 108, 59, 1, 8733, 4, 2, 99, 105, 4567, 4572, 114, 59, 3, 55349, 56491, 59, 1, 936, 4, 4, 85, 102, 111, 115, 4585, 4594, 4599, 4604, 79, 84, 5, 34, 1, 59, 4592, 1, 34, 114, 59, 3, 55349, 56596, 112, 102, 59, 1, 8474, 99, 114, 59, 3, 55349, 56492, 4, 12, 66, 69, 97, 99, 101, 102, 104, 105, 111, 114, 115, 117, 4636, 4642, 4650, 4681, 4704, 4763, 4767, 4771, 5047, 5069, 5081, 5094, 97, 114, 114, 59, 1, 10512, 71, 5, 174, 1, 59, 4648, 1, 174, 4, 3, 99, 110, 114, 4658, 4664, 4668, 117, 116, 101, 59, 1, 340, 103, 59, 1, 10219, 114, 4, 2, 59, 116, 4675, 4677, 1, 8608, 108, 59, 1, 10518, 4, 3, 97, 101, 121, 4689, 4695, 4701, 114, 111, 110, 59, 1, 344, 100, 105, 108, 59, 1, 342, 59, 1, 1056, 4, 2, 59, 118, 4710, 4712, 1, 8476, 101, 114, 115, 101, 4, 2, 69, 85, 4722, 4748, 4, 2, 108, 113, 4728, 4736, 101, 109, 101, 110, 116, 59, 1, 8715, 117, 105, 108, 105, 98, 114, 105, 117, 109, 59, 1, 8651, 112, 69, 113, 117, 105, 108, 105, 98, 114, 105, 117, 109, 59, 1, 10607, 114, 59, 1, 8476, 111, 59, 1, 929, 103, 104, 116, 4, 8, 65, 67, 68, 70, 84, 85, 86, 97, 4792, 4840, 4849, 4905, 4912, 4972, 5022, 5040, 4, 2, 110, 114, 4798, 4811, 103, 108, 101, 66, 114, 97, 99, 107, 101, 116, 59, 1, 10217, 114, 111, 119, 4, 3, 59, 66, 76, 4822, 4824, 4829, 1, 8594, 97, 114, 59, 1, 8677, 101, 102, 116, 65, 114, 114, 111, 119, 59, 1, 8644, 101, 105, 108, 105, 110, 103, 59, 1, 8969, 111, 4, 2, 117, 119, 4856, 4869, 98, 108, 101, 66, 114, 97, 99, 107, 101, 116, 59, 1, 10215, 110, 4, 2, 84, 86, 4876, 4887, 101, 101, 86, 101, 99, 116, 111, 114, 59, 1, 10589, 101, 99, 116, 111, 114, 4, 2, 59, 66, 4898, 4900, 1, 8642, 97, 114, 59, 1, 10581, 108, 111, 111, 114, 59, 1, 8971, 4, 2, 101, 114, 4918, 4944, 101, 4, 3, 59, 65, 86, 4927, 4929, 4936, 1, 8866, 114, 114, 111, 119, 59, 1, 8614, 101, 99, 116, 111, 114, 59, 1, 10587, 105, 97, 110, 103, 108, 101, 4, 3, 59, 66, 69, 4958, 4960, 4965, 1, 8883, 97, 114, 59, 1, 10704, 113, 117, 97, 108, 59, 1, 8885, 112, 4, 3, 68, 84, 86, 4981, 4993, 5004, 111, 119, 110, 86, 101, 99, 116, 111, 114, 59, 1, 10575, 101, 101, 86, 101, 99, 116, 111, 114, 59, 1, 10588, 101, 99, 116, 111, 114, 4, 2, 59, 66, 5015, 5017, 1, 8638, 97, 114, 59, 1, 10580, 101, 99, 116, 111, 114, 4, 2, 59, 66, 5033, 5035, 1, 8640, 97, 114, 59, 1, 10579, 114, 114, 111, 119, 59, 1, 8658, 4, 2, 112, 117, 5053, 5057, 102, 59, 1, 8477, 110, 100, 73, 109, 112, 108, 105, 101, 115, 59, 1, 10608, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8667, 4, 2, 99, 104, 5087, 5091, 114, 59, 1, 8475, 59, 1, 8625, 108, 101, 68, 101, 108, 97, 121, 101, 100, 59, 1, 10740, 4, 13, 72, 79, 97, 99, 102, 104, 105, 109, 111, 113, 115, 116, 117, 5134, 5150, 5157, 5164, 5198, 5203, 5259, 5265, 5277, 5283, 5374, 5380, 5385, 4, 2, 67, 99, 5140, 5146, 72, 99, 121, 59, 1, 1065, 121, 59, 1, 1064, 70, 84, 99, 121, 59, 1, 1068, 99, 117, 116, 101, 59, 1, 346, 4, 5, 59, 97, 101, 105, 121, 5176, 5178, 5184, 5190, 5195, 1, 10940, 114, 111, 110, 59, 1, 352, 100, 105, 108, 59, 1, 350, 114, 99, 59, 1, 348, 59, 1, 1057, 114, 59, 3, 55349, 56598, 111, 114, 116, 4, 4, 68, 76, 82, 85, 5216, 5227, 5238, 5250, 111, 119, 110, 65, 114, 114, 111, 119, 59, 1, 8595, 101, 102, 116, 65, 114, 114, 111, 119, 59, 1, 8592, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 8594, 112, 65, 114, 114, 111, 119, 59, 1, 8593, 103, 109, 97, 59, 1, 931, 97, 108, 108, 67, 105, 114, 99, 108, 101, 59, 1, 8728, 112, 102, 59, 3, 55349, 56650, 4, 2, 114, 117, 5289, 5293, 116, 59, 1, 8730, 97, 114, 101, 4, 4, 59, 73, 83, 85, 5306, 5308, 5322, 5367, 1, 9633, 110, 116, 101, 114, 115, 101, 99, 116, 105, 111, 110, 59, 1, 8851, 117, 4, 2, 98, 112, 5329, 5347, 115, 101, 116, 4, 2, 59, 69, 5338, 5340, 1, 8847, 113, 117, 97, 108, 59, 1, 8849, 101, 114, 115, 101, 116, 4, 2, 59, 69, 5358, 5360, 1, 8848, 113, 117, 97, 108, 59, 1, 8850, 110, 105, 111, 110, 59, 1, 8852, 99, 114, 59, 3, 55349, 56494, 97, 114, 59, 1, 8902, 4, 4, 98, 99, 109, 112, 5395, 5420, 5475, 5478, 4, 2, 59, 115, 5401, 5403, 1, 8912, 101, 116, 4, 2, 59, 69, 5411, 5413, 1, 8912, 113, 117, 97, 108, 59, 1, 8838, 4, 2, 99, 104, 5426, 5468, 101, 101, 100, 115, 4, 4, 59, 69, 83, 84, 5440, 5442, 5449, 5461, 1, 8827, 113, 117, 97, 108, 59, 1, 10928, 108, 97, 110, 116, 69, 113, 117, 97, 108, 59, 1, 8829, 105, 108, 100, 101, 59, 1, 8831, 84, 104, 97, 116, 59, 1, 8715, 59, 1, 8721, 4, 3, 59, 101, 115, 5486, 5488, 5507, 1, 8913, 114, 115, 101, 116, 4, 2, 59, 69, 5498, 5500, 1, 8835, 113, 117, 97, 108, 59, 1, 8839, 101, 116, 59, 1, 8913, 4, 11, 72, 82, 83, 97, 99, 102, 104, 105, 111, 114, 115, 5536, 5546, 5552, 5567, 5579, 5602, 5607, 5655, 5695, 5701, 5711, 79, 82, 78, 5, 222, 1, 59, 5544, 1, 222, 65, 68, 69, 59, 1, 8482, 4, 2, 72, 99, 5558, 5563, 99, 121, 59, 1, 1035, 121, 59, 1, 1062, 4, 2, 98, 117, 5573, 5576, 59, 1, 9, 59, 1, 932, 4, 3, 97, 101, 121, 5587, 5593, 5599, 114, 111, 110, 59, 1, 356, 100, 105, 108, 59, 1, 354, 59, 1, 1058, 114, 59, 3, 55349, 56599, 4, 2, 101, 105, 5613, 5631, 4, 2, 114, 116, 5619, 5627, 101, 102, 111, 114, 101, 59, 1, 8756, 97, 59, 1, 920, 4, 2, 99, 110, 5637, 5647, 107, 83, 112, 97, 99, 101, 59, 3, 8287, 8202, 83, 112, 97, 99, 101, 59, 1, 8201, 108, 100, 101, 4, 4, 59, 69, 70, 84, 5668, 5670, 5677, 5688, 1, 8764, 113, 117, 97, 108, 59, 1, 8771, 117, 108, 108, 69, 113, 117, 97, 108, 59, 1, 8773, 105, 108, 100, 101, 59, 1, 8776, 112, 102, 59, 3, 55349, 56651, 105, 112, 108, 101, 68, 111, 116, 59, 1, 8411, 4, 2, 99, 116, 5717, 5722, 114, 59, 3, 55349, 56495, 114, 111, 107, 59, 1, 358, 4, 14, 97, 98, 99, 100, 102, 103, 109, 110, 111, 112, 114, 115, 116, 117, 5758, 5789, 5805, 5823, 5830, 5835, 5846, 5852, 5921, 5937, 6089, 6095, 6101, 6108, 4, 2, 99, 114, 5764, 5774, 117, 116, 101, 5, 218, 1, 59, 5772, 1, 218, 114, 4, 2, 59, 111, 5781, 5783, 1, 8607, 99, 105, 114, 59, 1, 10569, 114, 4, 2, 99, 101, 5796, 5800, 121, 59, 1, 1038, 118, 101, 59, 1, 364, 4, 2, 105, 121, 5811, 5820, 114, 99, 5, 219, 1, 59, 5818, 1, 219, 59, 1, 1059, 98, 108, 97, 99, 59, 1, 368, 114, 59, 3, 55349, 56600, 114, 97, 118, 101, 5, 217, 1, 59, 5844, 1, 217, 97, 99, 114, 59, 1, 362, 4, 2, 100, 105, 5858, 5905, 101, 114, 4, 2, 66, 80, 5866, 5892, 4, 2, 97, 114, 5872, 5876, 114, 59, 1, 95, 97, 99, 4, 2, 101, 107, 5884, 5887, 59, 1, 9183, 101, 116, 59, 1, 9141, 97, 114, 101, 110, 116, 104, 101, 115, 105, 115, 59, 1, 9181, 111, 110, 4, 2, 59, 80, 5913, 5915, 1, 8899, 108, 117, 115, 59, 1, 8846, 4, 2, 103, 112, 5927, 5932, 111, 110, 59, 1, 370, 102, 59, 3, 55349, 56652, 4, 8, 65, 68, 69, 84, 97, 100, 112, 115, 5955, 5985, 5996, 6009, 6026, 6033, 6044, 6075, 114, 114, 111, 119, 4, 3, 59, 66, 68, 5967, 5969, 5974, 1, 8593, 97, 114, 59, 1, 10514, 111, 119, 110, 65, 114, 114, 111, 119, 59, 1, 8645, 111, 119, 110, 65, 114, 114, 111, 119, 59, 1, 8597, 113, 117, 105, 108, 105, 98, 114, 105, 117, 109, 59, 1, 10606, 101, 101, 4, 2, 59, 65, 6017, 6019, 1, 8869, 114, 114, 111, 119, 59, 1, 8613, 114, 114, 111, 119, 59, 1, 8657, 111, 119, 110, 97, 114, 114, 111, 119, 59, 1, 8661, 101, 114, 4, 2, 76, 82, 6052, 6063, 101, 102, 116, 65, 114, 114, 111, 119, 59, 1, 8598, 105, 103, 104, 116, 65, 114, 114, 111, 119, 59, 1, 8599, 105, 4, 2, 59, 108, 6082, 6084, 1, 978, 111, 110, 59, 1, 933, 105, 110, 103, 59, 1, 366, 99, 114, 59, 3, 55349, 56496, 105, 108, 100, 101, 59, 1, 360, 109, 108, 5, 220, 1, 59, 6115, 1, 220, 4, 9, 68, 98, 99, 100, 101, 102, 111, 115, 118, 6137, 6143, 6148, 6152, 6166, 6250, 6255, 6261, 6267, 97, 115, 104, 59, 1, 8875, 97, 114, 59, 1, 10987, 121, 59, 1, 1042, 97, 115, 104, 4, 2, 59, 108, 6161, 6163, 1, 8873, 59, 1, 10982, 4, 2, 101, 114, 6172, 6175, 59, 1, 8897, 4, 3, 98, 116, 121, 6183, 6188, 6238, 97, 114, 59, 1, 8214, 4, 2, 59, 105, 6194, 6196, 1, 8214, 99, 97, 108, 4, 4, 66, 76, 83, 84, 6209, 6214, 6220, 6231, 97, 114, 59, 1, 8739, 105, 110, 101, 59, 1, 124, 101, 112, 97, 114, 97, 116, 111, 114, 59, 1, 10072, 105, 108, 100, 101, 59, 1, 8768, 84, 104, 105, 110, 83, 112, 97, 99, 101, 59, 1, 8202, 114, 59, 3, 55349, 56601, 112, 102, 59, 3, 55349, 56653, 99, 114, 59, 3, 55349, 56497, 100, 97, 115, 104, 59, 1, 8874, 4, 5, 99, 101, 102, 111, 115, 6286, 6292, 6298, 6303, 6309, 105, 114, 99, 59, 1, 372, 100, 103, 101, 59, 1, 8896, 114, 59, 3, 55349, 56602, 112, 102, 59, 3, 55349, 56654, 99, 114, 59, 3, 55349, 56498, 4, 4, 102, 105, 111, 115, 6325, 6330, 6333, 6339, 114, 59, 3, 55349, 56603, 59, 1, 926, 112, 102, 59, 3, 55349, 56655, 99, 114, 59, 3, 55349, 56499, 4, 9, 65, 73, 85, 97, 99, 102, 111, 115, 117, 6365, 6370, 6375, 6380, 6391, 6405, 6410, 6416, 6422, 99, 121, 59, 1, 1071, 99, 121, 59, 1, 1031, 99, 121, 59, 1, 1070, 99, 117, 116, 101, 5, 221, 1, 59, 6389, 1, 221, 4, 2, 105, 121, 6397, 6402, 114, 99, 59, 1, 374, 59, 1, 1067, 114, 59, 3, 55349, 56604, 112, 102, 59, 3, 55349, 56656, 99, 114, 59, 3, 55349, 56500, 109, 108, 59, 1, 376, 4, 8, 72, 97, 99, 100, 101, 102, 111, 115, 6445, 6450, 6457, 6472, 6477, 6501, 6505, 6510, 99, 121, 59, 1, 1046, 99, 117, 116, 101, 59, 1, 377, 4, 2, 97, 121, 6463, 6469, 114, 111, 110, 59, 1, 381, 59, 1, 1047, 111, 116, 59, 1, 379, 4, 2, 114, 116, 6483, 6497, 111, 87, 105, 100, 116, 104, 83, 112, 97, 99, 101, 59, 1, 8203, 97, 59, 1, 918, 114, 59, 1, 8488, 112, 102, 59, 1, 8484, 99, 114, 59, 3, 55349, 56501, 4, 16, 97, 98, 99, 101, 102, 103, 108, 109, 110, 111, 112, 114, 115, 116, 117, 119, 6550, 6561, 6568, 6612, 6622, 6634, 6645, 6672, 6699, 6854, 6870, 6923, 6933, 6963, 6974, 6983, 99, 117, 116, 101, 5, 225, 1, 59, 6559, 1, 225, 114, 101, 118, 101, 59, 1, 259, 4, 6, 59, 69, 100, 105, 117, 121, 6582, 6584, 6588, 6591, 6600, 6609, 1, 8766, 59, 3, 8766, 819, 59, 1, 8767, 114, 99, 5, 226, 1, 59, 6598, 1, 226, 116, 101, 5, 180, 1, 59, 6607, 1, 180, 59, 1, 1072, 108, 105, 103, 5, 230, 1, 59, 6620, 1, 230, 4, 2, 59, 114, 6628, 6630, 1, 8289, 59, 3, 55349, 56606, 114, 97, 118, 101, 5, 224, 1, 59, 6643, 1, 224, 4, 2, 101, 112, 6651, 6667, 4, 2, 102, 112, 6657, 6663, 115, 121, 109, 59, 1, 8501, 104, 59, 1, 8501, 104, 97, 59, 1, 945, 4, 2, 97, 112, 6678, 6692, 4, 2, 99, 108, 6684, 6688, 114, 59, 1, 257, 103, 59, 1, 10815, 5, 38, 1, 59, 6697, 1, 38, 4, 2, 100, 103, 6705, 6737, 4, 5, 59, 97, 100, 115, 118, 6717, 6719, 6724, 6727, 6734, 1, 8743, 110, 100, 59, 1, 10837, 59, 1, 10844, 108, 111, 112, 101, 59, 1, 10840, 59, 1, 10842, 4, 7, 59, 101, 108, 109, 114, 115, 122, 6753, 6755, 6758, 6762, 6814, 6835, 6848, 1, 8736, 59, 1, 10660, 101, 59, 1, 8736, 115, 100, 4, 2, 59, 97, 6770, 6772, 1, 8737, 4, 8, 97, 98, 99, 100, 101, 102, 103, 104, 6790, 6793, 6796, 6799, 6802, 6805, 6808, 6811, 59, 1, 10664, 59, 1, 10665, 59, 1, 10666, 59, 1, 10667, 59, 1, 10668, 59, 1, 10669, 59, 1, 10670, 59, 1, 10671, 116, 4, 2, 59, 118, 6821, 6823, 1, 8735, 98, 4, 2, 59, 100, 6830, 6832, 1, 8894, 59, 1, 10653, 4, 2, 112, 116, 6841, 6845, 104, 59, 1, 8738, 59, 1, 197, 97, 114, 114, 59, 1, 9084, 4, 2, 103, 112, 6860, 6865, 111, 110, 59, 1, 261, 102, 59, 3, 55349, 56658, 4, 7, 59, 69, 97, 101, 105, 111, 112, 6886, 6888, 6891, 6897, 6900, 6904, 6908, 1, 8776, 59, 1, 10864, 99, 105, 114, 59, 1, 10863, 59, 1, 8778, 100, 59, 1, 8779, 115, 59, 1, 39, 114, 111, 120, 4, 2, 59, 101, 6917, 6919, 1, 8776, 113, 59, 1, 8778, 105, 110, 103, 5, 229, 1, 59, 6931, 1, 229, 4, 3, 99, 116, 121, 6941, 6946, 6949, 114, 59, 3, 55349, 56502, 59, 1, 42, 109, 112, 4, 2, 59, 101, 6957, 6959, 1, 8776, 113, 59, 1, 8781, 105, 108, 100, 101, 5, 227, 1, 59, 6972, 1, 227, 109, 108, 5, 228, 1, 59, 6981, 1, 228, 4, 2, 99, 105, 6989, 6997, 111, 110, 105, 110, 116, 59, 1, 8755, 110, 116, 59, 1, 10769, 4, 16, 78, 97, 98, 99, 100, 101, 102, 105, 107, 108, 110, 111, 112, 114, 115, 117, 7036, 7041, 7119, 7135, 7149, 7155, 7219, 7224, 7347, 7354, 7463, 7489, 7786, 7793, 7814, 7866, 111, 116, 59, 1, 10989, 4, 2, 99, 114, 7047, 7094, 107, 4, 4, 99, 101, 112, 115, 7058, 7064, 7073, 7080, 111, 110, 103, 59, 1, 8780, 112, 115, 105, 108, 111, 110, 59, 1, 1014, 114, 105, 109, 101, 59, 1, 8245, 105, 109, 4, 2, 59, 101, 7088, 7090, 1, 8765, 113, 59, 1, 8909, 4, 2, 118, 119, 7100, 7105, 101, 101, 59, 1, 8893, 101, 100, 4, 2, 59, 103, 7113, 7115, 1, 8965, 101, 59, 1, 8965, 114, 107, 4, 2, 59, 116, 7127, 7129, 1, 9141, 98, 114, 107, 59, 1, 9142, 4, 2, 111, 121, 7141, 7146, 110, 103, 59, 1, 8780, 59, 1, 1073, 113, 117, 111, 59, 1, 8222, 4, 5, 99, 109, 112, 114, 116, 7167, 7181, 7188, 7193, 7199, 97, 117, 115, 4, 2, 59, 101, 7176, 7178, 1, 8757, 59, 1, 8757, 112, 116, 121, 118, 59, 1, 10672, 115, 105, 59, 1, 1014, 110, 111, 117, 59, 1, 8492, 4, 3, 97, 104, 119, 7207, 7210, 7213, 59, 1, 946, 59, 1, 8502, 101, 101, 110, 59, 1, 8812, 114, 59, 3, 55349, 56607, 103, 4, 7, 99, 111, 115, 116, 117, 118, 119, 7241, 7262, 7288, 7305, 7328, 7335, 7340, 4, 3, 97, 105, 117, 7249, 7253, 7258, 112, 59, 1, 8898, 114, 99, 59, 1, 9711, 112, 59, 1, 8899, 4, 3, 100, 112, 116, 7270, 7275, 7281, 111, 116, 59, 1, 10752, 108, 117, 115, 59, 1, 10753, 105, 109, 101, 115, 59, 1, 10754, 4, 2, 113, 116, 7294, 7300, 99, 117, 112, 59, 1, 10758, 97, 114, 59, 1, 9733, 114, 105, 97, 110, 103, 108, 101, 4, 2, 100, 117, 7318, 7324, 111, 119, 110, 59, 1, 9661, 112, 59, 1, 9651, 112, 108, 117, 115, 59, 1, 10756, 101, 101, 59, 1, 8897, 101, 100, 103, 101, 59, 1, 8896, 97, 114, 111, 119, 59, 1, 10509, 4, 3, 97, 107, 111, 7362, 7436, 7458, 4, 2, 99, 110, 7368, 7432, 107, 4, 3, 108, 115, 116, 7377, 7386, 7394, 111, 122, 101, 110, 103, 101, 59, 1, 10731, 113, 117, 97, 114, 101, 59, 1, 9642, 114, 105, 97, 110, 103, 108, 101, 4, 4, 59, 100, 108, 114, 7411, 7413, 7419, 7425, 1, 9652, 111, 119, 110, 59, 1, 9662, 101, 102, 116, 59, 1, 9666, 105, 103, 104, 116, 59, 1, 9656, 107, 59, 1, 9251, 4, 2, 49, 51, 7442, 7454, 4, 2, 50, 52, 7448, 7451, 59, 1, 9618, 59, 1, 9617, 52, 59, 1, 9619, 99, 107, 59, 1, 9608, 4, 2, 101, 111, 7469, 7485, 4, 2, 59, 113, 7475, 7478, 3, 61, 8421, 117, 105, 118, 59, 3, 8801, 8421, 116, 59, 1, 8976, 4, 4, 112, 116, 119, 120, 7499, 7504, 7517, 7523, 102, 59, 3, 55349, 56659, 4, 2, 59, 116, 7510, 7512, 1, 8869, 111, 109, 59, 1, 8869, 116, 105, 101, 59, 1, 8904, 4, 12, 68, 72, 85, 86, 98, 100, 104, 109, 112, 116, 117, 118, 7549, 7571, 7597, 7619, 7655, 7660, 7682, 7708, 7715, 7721, 7728, 7750, 4, 4, 76, 82, 108, 114, 7559, 7562, 7565, 7568, 59, 1, 9559, 59, 1, 9556, 59, 1, 9558, 59, 1, 9555, 4, 5, 59, 68, 85, 100, 117, 7583, 7585, 7588, 7591, 7594, 1, 9552, 59, 1, 9574, 59, 1, 9577, 59, 1, 9572, 59, 1, 9575, 4, 4, 76, 82, 108, 114, 7607, 7610, 7613, 7616, 59, 1, 9565, 59, 1, 9562, 59, 1, 9564, 59, 1, 9561, 4, 7, 59, 72, 76, 82, 104, 108, 114, 7635, 7637, 7640, 7643, 7646, 7649, 7652, 1, 9553, 59, 1, 9580, 59, 1, 9571, 59, 1, 9568, 59, 1, 9579, 59, 1, 9570, 59, 1, 9567, 111, 120, 59, 1, 10697, 4, 4, 76, 82, 108, 114, 7670, 7673, 7676, 7679, 59, 1, 9557, 59, 1, 9554, 59, 1, 9488, 59, 1, 9484, 4, 5, 59, 68, 85, 100, 117, 7694, 7696, 7699, 7702, 7705, 1, 9472, 59, 1, 9573, 59, 1, 9576, 59, 1, 9516, 59, 1, 9524, 105, 110, 117, 115, 59, 1, 8863, 108, 117, 115, 59, 1, 8862, 105, 109, 101, 115, 59, 1, 8864, 4, 4, 76, 82, 108, 114, 7738, 7741, 7744, 7747, 59, 1, 9563, 59, 1, 9560, 59, 1, 9496, 59, 1, 9492, 4, 7, 59, 72, 76, 82, 104, 108, 114, 7766, 7768, 7771, 7774, 7777, 7780, 7783, 1, 9474, 59, 1, 9578, 59, 1, 9569, 59, 1, 9566, 59, 1, 9532, 59, 1, 9508, 59, 1, 9500, 114, 105, 109, 101, 59, 1, 8245, 4, 2, 101, 118, 7799, 7804, 118, 101, 59, 1, 728, 98, 97, 114, 5, 166, 1, 59, 7812, 1, 166, 4, 4, 99, 101, 105, 111, 7824, 7829, 7834, 7846, 114, 59, 3, 55349, 56503, 109, 105, 59, 1, 8271, 109, 4, 2, 59, 101, 7841, 7843, 1, 8765, 59, 1, 8909, 108, 4, 3, 59, 98, 104, 7855, 7857, 7860, 1, 92, 59, 1, 10693, 115, 117, 98, 59, 1, 10184, 4, 2, 108, 109, 7872, 7885, 108, 4, 2, 59, 101, 7879, 7881, 1, 8226, 116, 59, 1, 8226, 112, 4, 3, 59, 69, 101, 7894, 7896, 7899, 1, 8782, 59, 1, 10926, 4, 2, 59, 113, 7905, 7907, 1, 8783, 59, 1, 8783, 4, 15, 97, 99, 100, 101, 102, 104, 105, 108, 111, 114, 115, 116, 117, 119, 121, 7942, 8021, 8075, 8080, 8121, 8126, 8157, 8279, 8295, 8430, 8446, 8485, 8491, 8707, 8726, 4, 3, 99, 112, 114, 7950, 7956, 8007, 117, 116, 101, 59, 1, 263, 4, 6, 59, 97, 98, 99, 100, 115, 7970, 7972, 7977, 7984, 7998, 8003, 1, 8745, 110, 100, 59, 1, 10820, 114, 99, 117, 112, 59, 1, 10825, 4, 2, 97, 117, 7990, 7994, 112, 59, 1, 10827, 112, 59, 1, 10823, 111, 116, 59, 1, 10816, 59, 3, 8745, 65024, 4, 2, 101, 111, 8013, 8017, 116, 59, 1, 8257, 110, 59, 1, 711, 4, 4, 97, 101, 105, 117, 8031, 8046, 8056, 8061, 4, 2, 112, 114, 8037, 8041, 115, 59, 1, 10829, 111, 110, 59, 1, 269, 100, 105, 108, 5, 231, 1, 59, 8054, 1, 231, 114, 99, 59, 1, 265, 112, 115, 4, 2, 59, 115, 8069, 8071, 1, 10828, 109, 59, 1, 10832, 111, 116, 59, 1, 267, 4, 3, 100, 109, 110, 8088, 8097, 8104, 105, 108, 5, 184, 1, 59, 8095, 1, 184, 112, 116, 121, 118, 59, 1, 10674, 116, 5, 162, 2, 59, 101, 8112, 8114, 1, 162, 114, 100, 111, 116, 59, 1, 183, 114, 59, 3, 55349, 56608, 4, 3, 99, 101, 105, 8134, 8138, 8154, 121, 59, 1, 1095, 99, 107, 4, 2, 59, 109, 8146, 8148, 1, 10003, 97, 114, 107, 59, 1, 10003, 59, 1, 967, 114, 4, 7, 59, 69, 99, 101, 102, 109, 115, 8174, 8176, 8179, 8258, 8261, 8268, 8273, 1, 9675, 59, 1, 10691, 4, 3, 59, 101, 108, 8187, 8189, 8193, 1, 710, 113, 59, 1, 8791, 101, 4, 2, 97, 100, 8200, 8223, 114, 114, 111, 119, 4, 2, 108, 114, 8210, 8216, 101, 102, 116, 59, 1, 8634, 105, 103, 104, 116, 59, 1, 8635, 4, 5, 82, 83, 97, 99, 100, 8235, 8238, 8241, 8246, 8252, 59, 1, 174, 59, 1, 9416, 115, 116, 59, 1, 8859, 105, 114, 99, 59, 1, 8858, 97, 115, 104, 59, 1, 8861, 59, 1, 8791, 110, 105, 110, 116, 59, 1, 10768, 105, 100, 59, 1, 10991, 99, 105, 114, 59, 1, 10690, 117, 98, 115, 4, 2, 59, 117, 8288, 8290, 1, 9827, 105, 116, 59, 1, 9827, 4, 4, 108, 109, 110, 112, 8305, 8326, 8376, 8400, 111, 110, 4, 2, 59, 101, 8313, 8315, 1, 58, 4, 2, 59, 113, 8321, 8323, 1, 8788, 59, 1, 8788, 4, 2, 109, 112, 8332, 8344, 97, 4, 2, 59, 116, 8339, 8341, 1, 44, 59, 1, 64, 4, 3, 59, 102, 108, 8352, 8354, 8358, 1, 8705, 110, 59, 1, 8728, 101, 4, 2, 109, 120, 8365, 8371, 101, 110, 116, 59, 1, 8705, 101, 115, 59, 1, 8450, 4, 2, 103, 105, 8382, 8395, 4, 2, 59, 100, 8388, 8390, 1, 8773, 111, 116, 59, 1, 10861, 110, 116, 59, 1, 8750, 4, 3, 102, 114, 121, 8408, 8412, 8417, 59, 3, 55349, 56660, 111, 100, 59, 1, 8720, 5, 169, 2, 59, 115, 8424, 8426, 1, 169, 114, 59, 1, 8471, 4, 2, 97, 111, 8436, 8441, 114, 114, 59, 1, 8629, 115, 115, 59, 1, 10007, 4, 2, 99, 117, 8452, 8457, 114, 59, 3, 55349, 56504, 4, 2, 98, 112, 8463, 8474, 4, 2, 59, 101, 8469, 8471, 1, 10959, 59, 1, 10961, 4, 2, 59, 101, 8480, 8482, 1, 10960, 59, 1, 10962, 100, 111, 116, 59, 1, 8943, 4, 7, 100, 101, 108, 112, 114, 118, 119, 8507, 8522, 8536, 8550, 8600, 8697, 8702, 97, 114, 114, 4, 2, 108, 114, 8516, 8519, 59, 1, 10552, 59, 1, 10549, 4, 2, 112, 115, 8528, 8532, 114, 59, 1, 8926, 99, 59, 1, 8927, 97, 114, 114, 4, 2, 59, 112, 8545, 8547, 1, 8630, 59, 1, 10557, 4, 6, 59, 98, 99, 100, 111, 115, 8564, 8566, 8573, 8587, 8592, 8596, 1, 8746, 114, 99, 97, 112, 59, 1, 10824, 4, 2, 97, 117, 8579, 8583, 112, 59, 1, 10822, 112, 59, 1, 10826, 111, 116, 59, 1, 8845, 114, 59, 1, 10821, 59, 3, 8746, 65024, 4, 4, 97, 108, 114, 118, 8610, 8623, 8663, 8672, 114, 114, 4, 2, 59, 109, 8618, 8620, 1, 8631, 59, 1, 10556, 121, 4, 3, 101, 118, 119, 8632, 8651, 8656, 113, 4, 2, 112, 115, 8639, 8645, 114, 101, 99, 59, 1, 8926, 117, 99, 99, 59, 1, 8927, 101, 101, 59, 1, 8910, 101, 100, 103, 101, 59, 1, 8911, 101, 110, 5, 164, 1, 59, 8670, 1, 164, 101, 97, 114, 114, 111, 119, 4, 2, 108, 114, 8684, 8690, 101, 102, 116, 59, 1, 8630, 105, 103, 104, 116, 59, 1, 8631, 101, 101, 59, 1, 8910, 101, 100, 59, 1, 8911, 4, 2, 99, 105, 8713, 8721, 111, 110, 105, 110, 116, 59, 1, 8754, 110, 116, 59, 1, 8753, 108, 99, 116, 121, 59, 1, 9005, 4, 19, 65, 72, 97, 98, 99, 100, 101, 102, 104, 105, 106, 108, 111, 114, 115, 116, 117, 119, 122, 8773, 8778, 8783, 8821, 8839, 8854, 8887, 8914, 8930, 8944, 9036, 9041, 9058, 9197, 9227, 9258, 9281, 9297, 9305, 114, 114, 59, 1, 8659, 97, 114, 59, 1, 10597, 4, 4, 103, 108, 114, 115, 8793, 8799, 8805, 8809, 103, 101, 114, 59, 1, 8224, 101, 116, 104, 59, 1, 8504, 114, 59, 1, 8595, 104, 4, 2, 59, 118, 8816, 8818, 1, 8208, 59, 1, 8867, 4, 2, 107, 108, 8827, 8834, 97, 114, 111, 119, 59, 1, 10511, 97, 99, 59, 1, 733, 4, 2, 97, 121, 8845, 8851, 114, 111, 110, 59, 1, 271, 59, 1, 1076, 4, 3, 59, 97, 111, 8862, 8864, 8880, 1, 8518, 4, 2, 103, 114, 8870, 8876, 103, 101, 114, 59, 1, 8225, 114, 59, 1, 8650, 116, 115, 101, 113, 59, 1, 10871, 4, 3, 103, 108, 109, 8895, 8902, 8907, 5, 176, 1, 59, 8900, 1, 176, 116, 97, 59, 1, 948, 112, 116, 121, 118, 59, 1, 10673, 4, 2, 105, 114, 8920, 8926, 115, 104, 116, 59, 1, 10623, 59, 3, 55349, 56609, 97, 114, 4, 2, 108, 114, 8938, 8941, 59, 1, 8643, 59, 1, 8642, 4, 5, 97, 101, 103, 115, 118, 8956, 8986, 8989, 8996, 9001, 109, 4, 3, 59, 111, 115, 8965, 8967, 8983, 1, 8900, 110, 100, 4, 2, 59, 115, 8975, 8977, 1, 8900, 117, 105, 116, 59, 1, 9830, 59, 1, 9830, 59, 1, 168, 97, 109, 109, 97, 59, 1, 989, 105, 110, 59, 1, 8946, 4, 3, 59, 105, 111, 9009, 9011, 9031, 1, 247, 100, 101, 5, 247, 2, 59, 111, 9020, 9022, 1, 247, 110, 116, 105, 109, 101, 115, 59, 1, 8903, 110, 120, 59, 1, 8903, 99, 121, 59, 1, 1106, 99, 4, 2, 111, 114, 9048, 9053, 114, 110, 59, 1, 8990, 111, 112, 59, 1, 8973, 4, 5, 108, 112, 116, 117, 119, 9070, 9076, 9081, 9130, 9144, 108, 97, 114, 59, 1, 36, 102, 59, 3, 55349, 56661, 4, 5, 59, 101, 109, 112, 115, 9093, 9095, 9109, 9116, 9122, 1, 729, 113, 4, 2, 59, 100, 9102, 9104, 1, 8784, 111, 116, 59, 1, 8785, 105, 110, 117, 115, 59, 1, 8760, 108, 117, 115, 59, 1, 8724, 113, 117, 97, 114, 101, 59, 1, 8865, 98, 108, 101, 98, 97, 114, 119, 101, 100, 103, 101, 59, 1, 8966, 110, 4, 3, 97, 100, 104, 9153, 9160, 9172, 114, 114, 111, 119, 59, 1, 8595, 111, 119, 110, 97, 114, 114, 111, 119, 115, 59, 1, 8650, 97, 114, 112, 111, 111, 110, 4, 2, 108, 114, 9184, 9190, 101, 102, 116, 59, 1, 8643, 105, 103, 104, 116, 59, 1, 8642, 4, 2, 98, 99, 9203, 9211, 107, 97, 114, 111, 119, 59, 1, 10512, 4, 2, 111, 114, 9217, 9222, 114, 110, 59, 1, 8991, 111, 112, 59, 1, 8972, 4, 3, 99, 111, 116, 9235, 9248, 9252, 4, 2, 114, 121, 9241, 9245, 59, 3, 55349, 56505, 59, 1, 1109, 108, 59, 1, 10742, 114, 111, 107, 59, 1, 273, 4, 2, 100, 114, 9264, 9269, 111, 116, 59, 1, 8945, 105, 4, 2, 59, 102, 9276, 9278, 1, 9663, 59, 1, 9662, 4, 2, 97, 104, 9287, 9292, 114, 114, 59, 1, 8693, 97, 114, 59, 1, 10607, 97, 110, 103, 108, 101, 59, 1, 10662, 4, 2, 99, 105, 9311, 9315, 121, 59, 1, 1119, 103, 114, 97, 114, 114, 59, 1, 10239, 4, 18, 68, 97, 99, 100, 101, 102, 103, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 120, 9361, 9376, 9398, 9439, 9444, 9447, 9462, 9495, 9531, 9585, 9598, 9614, 9659, 9755, 9771, 9792, 9808, 9826, 4, 2, 68, 111, 9367, 9372, 111, 116, 59, 1, 10871, 116, 59, 1, 8785, 4, 2, 99, 115, 9382, 9392, 117, 116, 101, 5, 233, 1, 59, 9390, 1, 233, 116, 101, 114, 59, 1, 10862, 4, 4, 97, 105, 111, 121, 9408, 9414, 9430, 9436, 114, 111, 110, 59, 1, 283, 114, 4, 2, 59, 99, 9421, 9423, 1, 8790, 5, 234, 1, 59, 9428, 1, 234, 108, 111, 110, 59, 1, 8789, 59, 1, 1101, 111, 116, 59, 1, 279, 59, 1, 8519, 4, 2, 68, 114, 9453, 9458, 111, 116, 59, 1, 8786, 59, 3, 55349, 56610, 4, 3, 59, 114, 115, 9470, 9472, 9482, 1, 10906, 97, 118, 101, 5, 232, 1, 59, 9480, 1, 232, 4, 2, 59, 100, 9488, 9490, 1, 10902, 111, 116, 59, 1, 10904, 4, 4, 59, 105, 108, 115, 9505, 9507, 9515, 9518, 1, 10905, 110, 116, 101, 114, 115, 59, 1, 9191, 59, 1, 8467, 4, 2, 59, 100, 9524, 9526, 1, 10901, 111, 116, 59, 1, 10903, 4, 3, 97, 112, 115, 9539, 9544, 9564, 99, 114, 59, 1, 275, 116, 121, 4, 3, 59, 115, 118, 9554, 9556, 9561, 1, 8709, 101, 116, 59, 1, 8709, 59, 1, 8709, 112, 4, 2, 49, 59, 9571, 9583, 4, 2, 51, 52, 9577, 9580, 59, 1, 8196, 59, 1, 8197, 1, 8195, 4, 2, 103, 115, 9591, 9594, 59, 1, 331, 112, 59, 1, 8194, 4, 2, 103, 112, 9604, 9609, 111, 110, 59, 1, 281, 102, 59, 3, 55349, 56662, 4, 3, 97, 108, 115, 9622, 9635, 9640, 114, 4, 2, 59, 115, 9629, 9631, 1, 8917, 108, 59, 1, 10723, 117, 115, 59, 1, 10865, 105, 4, 3, 59, 108, 118, 9649, 9651, 9656, 1, 949, 111, 110, 59, 1, 949, 59, 1, 1013, 4, 4, 99, 115, 117, 118, 9669, 9686, 9716, 9747, 4, 2, 105, 111, 9675, 9680, 114, 99, 59, 1, 8790, 108, 111, 110, 59, 1, 8789, 4, 2, 105, 108, 9692, 9696, 109, 59, 1, 8770, 97, 110, 116, 4, 2, 103, 108, 9705, 9710, 116, 114, 59, 1, 10902, 101, 115, 115, 59, 1, 10901, 4, 3, 97, 101, 105, 9724, 9729, 9734, 108, 115, 59, 1, 61, 115, 116, 59, 1, 8799, 118, 4, 2, 59, 68, 9741, 9743, 1, 8801, 68, 59, 1, 10872, 112, 97, 114, 115, 108, 59, 1, 10725, 4, 2, 68, 97, 9761, 9766, 111, 116, 59, 1, 8787, 114, 114, 59, 1, 10609, 4, 3, 99, 100, 105, 9779, 9783, 9788, 114, 59, 1, 8495, 111, 116, 59, 1, 8784, 109, 59, 1, 8770, 4, 2, 97, 104, 9798, 9801, 59, 1, 951, 5, 240, 1, 59, 9806, 1, 240, 4, 2, 109, 114, 9814, 9822, 108, 5, 235, 1, 59, 9820, 1, 235, 111, 59, 1, 8364, 4, 3, 99, 105, 112, 9834, 9838, 9843, 108, 59, 1, 33, 115, 116, 59, 1, 8707, 4, 2, 101, 111, 9849, 9859, 99, 116, 97, 116, 105, 111, 110, 59, 1, 8496, 110, 101, 110, 116, 105, 97, 108, 101, 59, 1, 8519, 4, 12, 97, 99, 101, 102, 105, 106, 108, 110, 111, 112, 114, 115, 9896, 9910, 9914, 9921, 9954, 9960, 9967, 9989, 9994, 10027, 10036, 10164, 108, 108, 105, 110, 103, 100, 111, 116, 115, 101, 113, 59, 1, 8786, 121, 59, 1, 1092, 109, 97, 108, 101, 59, 1, 9792, 4, 3, 105, 108, 114, 9929, 9935, 9950, 108, 105, 103, 59, 1, 64259, 4, 2, 105, 108, 9941, 9945, 103, 59, 1, 64256, 105, 103, 59, 1, 64260, 59, 3, 55349, 56611, 108, 105, 103, 59, 1, 64257, 108, 105, 103, 59, 3, 102, 106, 4, 3, 97, 108, 116, 9975, 9979, 9984, 116, 59, 1, 9837, 105, 103, 59, 1, 64258, 110, 115, 59, 1, 9649, 111, 102, 59, 1, 402, 4, 2, 112, 114, 1e4, 10005, 102, 59, 3, 55349, 56663, 4, 2, 97, 107, 10011, 10016, 108, 108, 59, 1, 8704, 4, 2, 59, 118, 10022, 10024, 1, 8916, 59, 1, 10969, 97, 114, 116, 105, 110, 116, 59, 1, 10765, 4, 2, 97, 111, 10042, 10159, 4, 2, 99, 115, 10048, 10155, 4, 6, 49, 50, 51, 52, 53, 55, 10062, 10102, 10114, 10135, 10139, 10151, 4, 6, 50, 51, 52, 53, 54, 56, 10076, 10083, 10086, 10093, 10096, 10099, 5, 189, 1, 59, 10081, 1, 189, 59, 1, 8531, 5, 188, 1, 59, 10091, 1, 188, 59, 1, 8533, 59, 1, 8537, 59, 1, 8539, 4, 2, 51, 53, 10108, 10111, 59, 1, 8532, 59, 1, 8534, 4, 3, 52, 53, 56, 10122, 10129, 10132, 5, 190, 1, 59, 10127, 1, 190, 59, 1, 8535, 59, 1, 8540, 53, 59, 1, 8536, 4, 2, 54, 56, 10145, 10148, 59, 1, 8538, 59, 1, 8541, 56, 59, 1, 8542, 108, 59, 1, 8260, 119, 110, 59, 1, 8994, 99, 114, 59, 3, 55349, 56507, 4, 17, 69, 97, 98, 99, 100, 101, 102, 103, 105, 106, 108, 110, 111, 114, 115, 116, 118, 10206, 10217, 10247, 10254, 10268, 10273, 10358, 10363, 10374, 10380, 10385, 10406, 10458, 10464, 10470, 10497, 10610, 4, 2, 59, 108, 10212, 10214, 1, 8807, 59, 1, 10892, 4, 3, 99, 109, 112, 10225, 10231, 10244, 117, 116, 101, 59, 1, 501, 109, 97, 4, 2, 59, 100, 10239, 10241, 1, 947, 59, 1, 989, 59, 1, 10886, 114, 101, 118, 101, 59, 1, 287, 4, 2, 105, 121, 10260, 10265, 114, 99, 59, 1, 285, 59, 1, 1075, 111, 116, 59, 1, 289, 4, 4, 59, 108, 113, 115, 10283, 10285, 10288, 10308, 1, 8805, 59, 1, 8923, 4, 3, 59, 113, 115, 10296, 10298, 10301, 1, 8805, 59, 1, 8807, 108, 97, 110, 116, 59, 1, 10878, 4, 4, 59, 99, 100, 108, 10318, 10320, 10324, 10345, 1, 10878, 99, 59, 1, 10921, 111, 116, 4, 2, 59, 111, 10332, 10334, 1, 10880, 4, 2, 59, 108, 10340, 10342, 1, 10882, 59, 1, 10884, 4, 2, 59, 101, 10351, 10354, 3, 8923, 65024, 115, 59, 1, 10900, 114, 59, 3, 55349, 56612, 4, 2, 59, 103, 10369, 10371, 1, 8811, 59, 1, 8921, 109, 101, 108, 59, 1, 8503, 99, 121, 59, 1, 1107, 4, 4, 59, 69, 97, 106, 10395, 10397, 10400, 10403, 1, 8823, 59, 1, 10898, 59, 1, 10917, 59, 1, 10916, 4, 4, 69, 97, 101, 115, 10416, 10419, 10434, 10453, 59, 1, 8809, 112, 4, 2, 59, 112, 10426, 10428, 1, 10890, 114, 111, 120, 59, 1, 10890, 4, 2, 59, 113, 10440, 10442, 1, 10888, 4, 2, 59, 113, 10448, 10450, 1, 10888, 59, 1, 8809, 105, 109, 59, 1, 8935, 112, 102, 59, 3, 55349, 56664, 97, 118, 101, 59, 1, 96, 4, 2, 99, 105, 10476, 10480, 114, 59, 1, 8458, 109, 4, 3, 59, 101, 108, 10489, 10491, 10494, 1, 8819, 59, 1, 10894, 59, 1, 10896, 5, 62, 6, 59, 99, 100, 108, 113, 114, 10512, 10514, 10527, 10532, 10538, 10545, 1, 62, 4, 2, 99, 105, 10520, 10523, 59, 1, 10919, 114, 59, 1, 10874, 111, 116, 59, 1, 8919, 80, 97, 114, 59, 1, 10645, 117, 101, 115, 116, 59, 1, 10876, 4, 5, 97, 100, 101, 108, 115, 10557, 10574, 10579, 10599, 10605, 4, 2, 112, 114, 10563, 10570, 112, 114, 111, 120, 59, 1, 10886, 114, 59, 1, 10616, 111, 116, 59, 1, 8919, 113, 4, 2, 108, 113, 10586, 10592, 101, 115, 115, 59, 1, 8923, 108, 101, 115, 115, 59, 1, 10892, 101, 115, 115, 59, 1, 8823, 105, 109, 59, 1, 8819, 4, 2, 101, 110, 10616, 10626, 114, 116, 110, 101, 113, 113, 59, 3, 8809, 65024, 69, 59, 3, 8809, 65024, 4, 10, 65, 97, 98, 99, 101, 102, 107, 111, 115, 121, 10653, 10658, 10713, 10718, 10724, 10760, 10765, 10786, 10850, 10875, 114, 114, 59, 1, 8660, 4, 4, 105, 108, 109, 114, 10668, 10674, 10678, 10684, 114, 115, 112, 59, 1, 8202, 102, 59, 1, 189, 105, 108, 116, 59, 1, 8459, 4, 2, 100, 114, 10690, 10695, 99, 121, 59, 1, 1098, 4, 3, 59, 99, 119, 10703, 10705, 10710, 1, 8596, 105, 114, 59, 1, 10568, 59, 1, 8621, 97, 114, 59, 1, 8463, 105, 114, 99, 59, 1, 293, 4, 3, 97, 108, 114, 10732, 10748, 10754, 114, 116, 115, 4, 2, 59, 117, 10741, 10743, 1, 9829, 105, 116, 59, 1, 9829, 108, 105, 112, 59, 1, 8230, 99, 111, 110, 59, 1, 8889, 114, 59, 3, 55349, 56613, 115, 4, 2, 101, 119, 10772, 10779, 97, 114, 111, 119, 59, 1, 10533, 97, 114, 111, 119, 59, 1, 10534, 4, 5, 97, 109, 111, 112, 114, 10798, 10803, 10809, 10839, 10844, 114, 114, 59, 1, 8703, 116, 104, 116, 59, 1, 8763, 107, 4, 2, 108, 114, 10816, 10827, 101, 102, 116, 97, 114, 114, 111, 119, 59, 1, 8617, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8618, 102, 59, 3, 55349, 56665, 98, 97, 114, 59, 1, 8213, 4, 3, 99, 108, 116, 10858, 10863, 10869, 114, 59, 3, 55349, 56509, 97, 115, 104, 59, 1, 8463, 114, 111, 107, 59, 1, 295, 4, 2, 98, 112, 10881, 10887, 117, 108, 108, 59, 1, 8259, 104, 101, 110, 59, 1, 8208, 4, 15, 97, 99, 101, 102, 103, 105, 106, 109, 110, 111, 112, 113, 115, 116, 117, 10925, 10936, 10958, 10977, 10990, 11001, 11039, 11045, 11101, 11192, 11220, 11226, 11237, 11285, 11299, 99, 117, 116, 101, 5, 237, 1, 59, 10934, 1, 237, 4, 3, 59, 105, 121, 10944, 10946, 10955, 1, 8291, 114, 99, 5, 238, 1, 59, 10953, 1, 238, 59, 1, 1080, 4, 2, 99, 120, 10964, 10968, 121, 59, 1, 1077, 99, 108, 5, 161, 1, 59, 10975, 1, 161, 4, 2, 102, 114, 10983, 10986, 59, 1, 8660, 59, 3, 55349, 56614, 114, 97, 118, 101, 5, 236, 1, 59, 10999, 1, 236, 4, 4, 59, 105, 110, 111, 11011, 11013, 11028, 11034, 1, 8520, 4, 2, 105, 110, 11019, 11024, 110, 116, 59, 1, 10764, 116, 59, 1, 8749, 102, 105, 110, 59, 1, 10716, 116, 97, 59, 1, 8489, 108, 105, 103, 59, 1, 307, 4, 3, 97, 111, 112, 11053, 11092, 11096, 4, 3, 99, 103, 116, 11061, 11065, 11088, 114, 59, 1, 299, 4, 3, 101, 108, 112, 11073, 11076, 11082, 59, 1, 8465, 105, 110, 101, 59, 1, 8464, 97, 114, 116, 59, 1, 8465, 104, 59, 1, 305, 102, 59, 1, 8887, 101, 100, 59, 1, 437, 4, 5, 59, 99, 102, 111, 116, 11113, 11115, 11121, 11136, 11142, 1, 8712, 97, 114, 101, 59, 1, 8453, 105, 110, 4, 2, 59, 116, 11129, 11131, 1, 8734, 105, 101, 59, 1, 10717, 100, 111, 116, 59, 1, 305, 4, 5, 59, 99, 101, 108, 112, 11154, 11156, 11161, 11179, 11186, 1, 8747, 97, 108, 59, 1, 8890, 4, 2, 103, 114, 11167, 11173, 101, 114, 115, 59, 1, 8484, 99, 97, 108, 59, 1, 8890, 97, 114, 104, 107, 59, 1, 10775, 114, 111, 100, 59, 1, 10812, 4, 4, 99, 103, 112, 116, 11202, 11206, 11211, 11216, 121, 59, 1, 1105, 111, 110, 59, 1, 303, 102, 59, 3, 55349, 56666, 97, 59, 1, 953, 114, 111, 100, 59, 1, 10812, 117, 101, 115, 116, 5, 191, 1, 59, 11235, 1, 191, 4, 2, 99, 105, 11243, 11248, 114, 59, 3, 55349, 56510, 110, 4, 5, 59, 69, 100, 115, 118, 11261, 11263, 11266, 11271, 11282, 1, 8712, 59, 1, 8953, 111, 116, 59, 1, 8949, 4, 2, 59, 118, 11277, 11279, 1, 8948, 59, 1, 8947, 59, 1, 8712, 4, 2, 59, 105, 11291, 11293, 1, 8290, 108, 100, 101, 59, 1, 297, 4, 2, 107, 109, 11305, 11310, 99, 121, 59, 1, 1110, 108, 5, 239, 1, 59, 11316, 1, 239, 4, 6, 99, 102, 109, 111, 115, 117, 11332, 11346, 11351, 11357, 11363, 11380, 4, 2, 105, 121, 11338, 11343, 114, 99, 59, 1, 309, 59, 1, 1081, 114, 59, 3, 55349, 56615, 97, 116, 104, 59, 1, 567, 112, 102, 59, 3, 55349, 56667, 4, 2, 99, 101, 11369, 11374, 114, 59, 3, 55349, 56511, 114, 99, 121, 59, 1, 1112, 107, 99, 121, 59, 1, 1108, 4, 8, 97, 99, 102, 103, 104, 106, 111, 115, 11404, 11418, 11433, 11438, 11445, 11450, 11455, 11461, 112, 112, 97, 4, 2, 59, 118, 11413, 11415, 1, 954, 59, 1, 1008, 4, 2, 101, 121, 11424, 11430, 100, 105, 108, 59, 1, 311, 59, 1, 1082, 114, 59, 3, 55349, 56616, 114, 101, 101, 110, 59, 1, 312, 99, 121, 59, 1, 1093, 99, 121, 59, 1, 1116, 112, 102, 59, 3, 55349, 56668, 99, 114, 59, 3, 55349, 56512, 4, 23, 65, 66, 69, 72, 97, 98, 99, 100, 101, 102, 103, 104, 106, 108, 109, 110, 111, 112, 114, 115, 116, 117, 118, 11515, 11538, 11544, 11555, 11560, 11721, 11780, 11818, 11868, 12136, 12160, 12171, 12203, 12208, 12246, 12275, 12327, 12509, 12523, 12569, 12641, 12732, 12752, 4, 3, 97, 114, 116, 11523, 11528, 11532, 114, 114, 59, 1, 8666, 114, 59, 1, 8656, 97, 105, 108, 59, 1, 10523, 97, 114, 114, 59, 1, 10510, 4, 2, 59, 103, 11550, 11552, 1, 8806, 59, 1, 10891, 97, 114, 59, 1, 10594, 4, 9, 99, 101, 103, 109, 110, 112, 113, 114, 116, 11580, 11586, 11594, 11600, 11606, 11624, 11627, 11636, 11694, 117, 116, 101, 59, 1, 314, 109, 112, 116, 121, 118, 59, 1, 10676, 114, 97, 110, 59, 1, 8466, 98, 100, 97, 59, 1, 955, 103, 4, 3, 59, 100, 108, 11615, 11617, 11620, 1, 10216, 59, 1, 10641, 101, 59, 1, 10216, 59, 1, 10885, 117, 111, 5, 171, 1, 59, 11634, 1, 171, 114, 4, 8, 59, 98, 102, 104, 108, 112, 115, 116, 11655, 11657, 11669, 11673, 11677, 11681, 11685, 11690, 1, 8592, 4, 2, 59, 102, 11663, 11665, 1, 8676, 115, 59, 1, 10527, 115, 59, 1, 10525, 107, 59, 1, 8617, 112, 59, 1, 8619, 108, 59, 1, 10553, 105, 109, 59, 1, 10611, 108, 59, 1, 8610, 4, 3, 59, 97, 101, 11702, 11704, 11709, 1, 10923, 105, 108, 59, 1, 10521, 4, 2, 59, 115, 11715, 11717, 1, 10925, 59, 3, 10925, 65024, 4, 3, 97, 98, 114, 11729, 11734, 11739, 114, 114, 59, 1, 10508, 114, 107, 59, 1, 10098, 4, 2, 97, 107, 11745, 11758, 99, 4, 2, 101, 107, 11752, 11755, 59, 1, 123, 59, 1, 91, 4, 2, 101, 115, 11764, 11767, 59, 1, 10635, 108, 4, 2, 100, 117, 11774, 11777, 59, 1, 10639, 59, 1, 10637, 4, 4, 97, 101, 117, 121, 11790, 11796, 11811, 11815, 114, 111, 110, 59, 1, 318, 4, 2, 100, 105, 11802, 11807, 105, 108, 59, 1, 316, 108, 59, 1, 8968, 98, 59, 1, 123, 59, 1, 1083, 4, 4, 99, 113, 114, 115, 11828, 11832, 11845, 11864, 97, 59, 1, 10550, 117, 111, 4, 2, 59, 114, 11840, 11842, 1, 8220, 59, 1, 8222, 4, 2, 100, 117, 11851, 11857, 104, 97, 114, 59, 1, 10599, 115, 104, 97, 114, 59, 1, 10571, 104, 59, 1, 8626, 4, 5, 59, 102, 103, 113, 115, 11880, 11882, 12008, 12011, 12031, 1, 8804, 116, 4, 5, 97, 104, 108, 114, 116, 11895, 11913, 11935, 11947, 11996, 114, 114, 111, 119, 4, 2, 59, 116, 11905, 11907, 1, 8592, 97, 105, 108, 59, 1, 8610, 97, 114, 112, 111, 111, 110, 4, 2, 100, 117, 11925, 11931, 111, 119, 110, 59, 1, 8637, 112, 59, 1, 8636, 101, 102, 116, 97, 114, 114, 111, 119, 115, 59, 1, 8647, 105, 103, 104, 116, 4, 3, 97, 104, 115, 11959, 11974, 11984, 114, 114, 111, 119, 4, 2, 59, 115, 11969, 11971, 1, 8596, 59, 1, 8646, 97, 114, 112, 111, 111, 110, 115, 59, 1, 8651, 113, 117, 105, 103, 97, 114, 114, 111, 119, 59, 1, 8621, 104, 114, 101, 101, 116, 105, 109, 101, 115, 59, 1, 8907, 59, 1, 8922, 4, 3, 59, 113, 115, 12019, 12021, 12024, 1, 8804, 59, 1, 8806, 108, 97, 110, 116, 59, 1, 10877, 4, 5, 59, 99, 100, 103, 115, 12043, 12045, 12049, 12070, 12083, 1, 10877, 99, 59, 1, 10920, 111, 116, 4, 2, 59, 111, 12057, 12059, 1, 10879, 4, 2, 59, 114, 12065, 12067, 1, 10881, 59, 1, 10883, 4, 2, 59, 101, 12076, 12079, 3, 8922, 65024, 115, 59, 1, 10899, 4, 5, 97, 100, 101, 103, 115, 12095, 12103, 12108, 12126, 12131, 112, 112, 114, 111, 120, 59, 1, 10885, 111, 116, 59, 1, 8918, 113, 4, 2, 103, 113, 12115, 12120, 116, 114, 59, 1, 8922, 103, 116, 114, 59, 1, 10891, 116, 114, 59, 1, 8822, 105, 109, 59, 1, 8818, 4, 3, 105, 108, 114, 12144, 12150, 12156, 115, 104, 116, 59, 1, 10620, 111, 111, 114, 59, 1, 8970, 59, 3, 55349, 56617, 4, 2, 59, 69, 12166, 12168, 1, 8822, 59, 1, 10897, 4, 2, 97, 98, 12177, 12198, 114, 4, 2, 100, 117, 12184, 12187, 59, 1, 8637, 4, 2, 59, 108, 12193, 12195, 1, 8636, 59, 1, 10602, 108, 107, 59, 1, 9604, 99, 121, 59, 1, 1113, 4, 5, 59, 97, 99, 104, 116, 12220, 12222, 12227, 12235, 12241, 1, 8810, 114, 114, 59, 1, 8647, 111, 114, 110, 101, 114, 59, 1, 8990, 97, 114, 100, 59, 1, 10603, 114, 105, 59, 1, 9722, 4, 2, 105, 111, 12252, 12258, 100, 111, 116, 59, 1, 320, 117, 115, 116, 4, 2, 59, 97, 12267, 12269, 1, 9136, 99, 104, 101, 59, 1, 9136, 4, 4, 69, 97, 101, 115, 12285, 12288, 12303, 12322, 59, 1, 8808, 112, 4, 2, 59, 112, 12295, 12297, 1, 10889, 114, 111, 120, 59, 1, 10889, 4, 2, 59, 113, 12309, 12311, 1, 10887, 4, 2, 59, 113, 12317, 12319, 1, 10887, 59, 1, 8808, 105, 109, 59, 1, 8934, 4, 8, 97, 98, 110, 111, 112, 116, 119, 122, 12345, 12359, 12364, 12421, 12446, 12467, 12474, 12490, 4, 2, 110, 114, 12351, 12355, 103, 59, 1, 10220, 114, 59, 1, 8701, 114, 107, 59, 1, 10214, 103, 4, 3, 108, 109, 114, 12373, 12401, 12409, 101, 102, 116, 4, 2, 97, 114, 12382, 12389, 114, 114, 111, 119, 59, 1, 10229, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 10231, 97, 112, 115, 116, 111, 59, 1, 10236, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 10230, 112, 97, 114, 114, 111, 119, 4, 2, 108, 114, 12433, 12439, 101, 102, 116, 59, 1, 8619, 105, 103, 104, 116, 59, 1, 8620, 4, 3, 97, 102, 108, 12454, 12458, 12462, 114, 59, 1, 10629, 59, 3, 55349, 56669, 117, 115, 59, 1, 10797, 105, 109, 101, 115, 59, 1, 10804, 4, 2, 97, 98, 12480, 12485, 115, 116, 59, 1, 8727, 97, 114, 59, 1, 95, 4, 3, 59, 101, 102, 12498, 12500, 12506, 1, 9674, 110, 103, 101, 59, 1, 9674, 59, 1, 10731, 97, 114, 4, 2, 59, 108, 12517, 12519, 1, 40, 116, 59, 1, 10643, 4, 5, 97, 99, 104, 109, 116, 12535, 12540, 12548, 12561, 12564, 114, 114, 59, 1, 8646, 111, 114, 110, 101, 114, 59, 1, 8991, 97, 114, 4, 2, 59, 100, 12556, 12558, 1, 8651, 59, 1, 10605, 59, 1, 8206, 114, 105, 59, 1, 8895, 4, 6, 97, 99, 104, 105, 113, 116, 12583, 12589, 12594, 12597, 12614, 12635, 113, 117, 111, 59, 1, 8249, 114, 59, 3, 55349, 56513, 59, 1, 8624, 109, 4, 3, 59, 101, 103, 12606, 12608, 12611, 1, 8818, 59, 1, 10893, 59, 1, 10895, 4, 2, 98, 117, 12620, 12623, 59, 1, 91, 111, 4, 2, 59, 114, 12630, 12632, 1, 8216, 59, 1, 8218, 114, 111, 107, 59, 1, 322, 5, 60, 8, 59, 99, 100, 104, 105, 108, 113, 114, 12660, 12662, 12675, 12680, 12686, 12692, 12698, 12705, 1, 60, 4, 2, 99, 105, 12668, 12671, 59, 1, 10918, 114, 59, 1, 10873, 111, 116, 59, 1, 8918, 114, 101, 101, 59, 1, 8907, 109, 101, 115, 59, 1, 8905, 97, 114, 114, 59, 1, 10614, 117, 101, 115, 116, 59, 1, 10875, 4, 2, 80, 105, 12711, 12716, 97, 114, 59, 1, 10646, 4, 3, 59, 101, 102, 12724, 12726, 12729, 1, 9667, 59, 1, 8884, 59, 1, 9666, 114, 4, 2, 100, 117, 12739, 12746, 115, 104, 97, 114, 59, 1, 10570, 104, 97, 114, 59, 1, 10598, 4, 2, 101, 110, 12758, 12768, 114, 116, 110, 101, 113, 113, 59, 3, 8808, 65024, 69, 59, 3, 8808, 65024, 4, 14, 68, 97, 99, 100, 101, 102, 104, 105, 108, 110, 111, 112, 115, 117, 12803, 12809, 12893, 12908, 12914, 12928, 12933, 12937, 13011, 13025, 13032, 13049, 13052, 13069, 68, 111, 116, 59, 1, 8762, 4, 4, 99, 108, 112, 114, 12819, 12827, 12849, 12887, 114, 5, 175, 1, 59, 12825, 1, 175, 4, 2, 101, 116, 12833, 12836, 59, 1, 9794, 4, 2, 59, 101, 12842, 12844, 1, 10016, 115, 101, 59, 1, 10016, 4, 2, 59, 115, 12855, 12857, 1, 8614, 116, 111, 4, 4, 59, 100, 108, 117, 12869, 12871, 12877, 12883, 1, 8614, 111, 119, 110, 59, 1, 8615, 101, 102, 116, 59, 1, 8612, 112, 59, 1, 8613, 107, 101, 114, 59, 1, 9646, 4, 2, 111, 121, 12899, 12905, 109, 109, 97, 59, 1, 10793, 59, 1, 1084, 97, 115, 104, 59, 1, 8212, 97, 115, 117, 114, 101, 100, 97, 110, 103, 108, 101, 59, 1, 8737, 114, 59, 3, 55349, 56618, 111, 59, 1, 8487, 4, 3, 99, 100, 110, 12945, 12954, 12985, 114, 111, 5, 181, 1, 59, 12952, 1, 181, 4, 4, 59, 97, 99, 100, 12964, 12966, 12971, 12976, 1, 8739, 115, 116, 59, 1, 42, 105, 114, 59, 1, 10992, 111, 116, 5, 183, 1, 59, 12983, 1, 183, 117, 115, 4, 3, 59, 98, 100, 12995, 12997, 13e3, 1, 8722, 59, 1, 8863, 4, 2, 59, 117, 13006, 13008, 1, 8760, 59, 1, 10794, 4, 2, 99, 100, 13017, 13021, 112, 59, 1, 10971, 114, 59, 1, 8230, 112, 108, 117, 115, 59, 1, 8723, 4, 2, 100, 112, 13038, 13044, 101, 108, 115, 59, 1, 8871, 102, 59, 3, 55349, 56670, 59, 1, 8723, 4, 2, 99, 116, 13058, 13063, 114, 59, 3, 55349, 56514, 112, 111, 115, 59, 1, 8766, 4, 3, 59, 108, 109, 13077, 13079, 13087, 1, 956, 116, 105, 109, 97, 112, 59, 1, 8888, 97, 112, 59, 1, 8888, 4, 24, 71, 76, 82, 86, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 108, 109, 111, 112, 114, 115, 116, 117, 118, 119, 13142, 13165, 13217, 13229, 13247, 13330, 13359, 13414, 13420, 13508, 13513, 13579, 13602, 13626, 13631, 13762, 13767, 13855, 13936, 13995, 14214, 14285, 14312, 14432, 4, 2, 103, 116, 13148, 13152, 59, 3, 8921, 824, 4, 2, 59, 118, 13158, 13161, 3, 8811, 8402, 59, 3, 8811, 824, 4, 3, 101, 108, 116, 13173, 13200, 13204, 102, 116, 4, 2, 97, 114, 13181, 13188, 114, 114, 111, 119, 59, 1, 8653, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8654, 59, 3, 8920, 824, 4, 2, 59, 118, 13210, 13213, 3, 8810, 8402, 59, 3, 8810, 824, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8655, 4, 2, 68, 100, 13235, 13241, 97, 115, 104, 59, 1, 8879, 97, 115, 104, 59, 1, 8878, 4, 5, 98, 99, 110, 112, 116, 13259, 13264, 13270, 13275, 13308, 108, 97, 59, 1, 8711, 117, 116, 101, 59, 1, 324, 103, 59, 3, 8736, 8402, 4, 5, 59, 69, 105, 111, 112, 13287, 13289, 13293, 13298, 13302, 1, 8777, 59, 3, 10864, 824, 100, 59, 3, 8779, 824, 115, 59, 1, 329, 114, 111, 120, 59, 1, 8777, 117, 114, 4, 2, 59, 97, 13316, 13318, 1, 9838, 108, 4, 2, 59, 115, 13325, 13327, 1, 9838, 59, 1, 8469, 4, 2, 115, 117, 13336, 13344, 112, 5, 160, 1, 59, 13342, 1, 160, 109, 112, 4, 2, 59, 101, 13352, 13355, 3, 8782, 824, 59, 3, 8783, 824, 4, 5, 97, 101, 111, 117, 121, 13371, 13385, 13391, 13407, 13411, 4, 2, 112, 114, 13377, 13380, 59, 1, 10819, 111, 110, 59, 1, 328, 100, 105, 108, 59, 1, 326, 110, 103, 4, 2, 59, 100, 13399, 13401, 1, 8775, 111, 116, 59, 3, 10861, 824, 112, 59, 1, 10818, 59, 1, 1085, 97, 115, 104, 59, 1, 8211, 4, 7, 59, 65, 97, 100, 113, 115, 120, 13436, 13438, 13443, 13466, 13472, 13478, 13494, 1, 8800, 114, 114, 59, 1, 8663, 114, 4, 2, 104, 114, 13450, 13454, 107, 59, 1, 10532, 4, 2, 59, 111, 13460, 13462, 1, 8599, 119, 59, 1, 8599, 111, 116, 59, 3, 8784, 824, 117, 105, 118, 59, 1, 8802, 4, 2, 101, 105, 13484, 13489, 97, 114, 59, 1, 10536, 109, 59, 3, 8770, 824, 105, 115, 116, 4, 2, 59, 115, 13503, 13505, 1, 8708, 59, 1, 8708, 114, 59, 3, 55349, 56619, 4, 4, 69, 101, 115, 116, 13523, 13527, 13563, 13568, 59, 3, 8807, 824, 4, 3, 59, 113, 115, 13535, 13537, 13559, 1, 8817, 4, 3, 59, 113, 115, 13545, 13547, 13551, 1, 8817, 59, 3, 8807, 824, 108, 97, 110, 116, 59, 3, 10878, 824, 59, 3, 10878, 824, 105, 109, 59, 1, 8821, 4, 2, 59, 114, 13574, 13576, 1, 8815, 59, 1, 8815, 4, 3, 65, 97, 112, 13587, 13592, 13597, 114, 114, 59, 1, 8654, 114, 114, 59, 1, 8622, 97, 114, 59, 1, 10994, 4, 3, 59, 115, 118, 13610, 13612, 13623, 1, 8715, 4, 2, 59, 100, 13618, 13620, 1, 8956, 59, 1, 8954, 59, 1, 8715, 99, 121, 59, 1, 1114, 4, 7, 65, 69, 97, 100, 101, 115, 116, 13647, 13652, 13656, 13661, 13665, 13737, 13742, 114, 114, 59, 1, 8653, 59, 3, 8806, 824, 114, 114, 59, 1, 8602, 114, 59, 1, 8229, 4, 4, 59, 102, 113, 115, 13675, 13677, 13703, 13725, 1, 8816, 116, 4, 2, 97, 114, 13684, 13691, 114, 114, 111, 119, 59, 1, 8602, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8622, 4, 3, 59, 113, 115, 13711, 13713, 13717, 1, 8816, 59, 3, 8806, 824, 108, 97, 110, 116, 59, 3, 10877, 824, 4, 2, 59, 115, 13731, 13734, 3, 10877, 824, 59, 1, 8814, 105, 109, 59, 1, 8820, 4, 2, 59, 114, 13748, 13750, 1, 8814, 105, 4, 2, 59, 101, 13757, 13759, 1, 8938, 59, 1, 8940, 105, 100, 59, 1, 8740, 4, 2, 112, 116, 13773, 13778, 102, 59, 3, 55349, 56671, 5, 172, 3, 59, 105, 110, 13787, 13789, 13829, 1, 172, 110, 4, 4, 59, 69, 100, 118, 13800, 13802, 13806, 13812, 1, 8713, 59, 3, 8953, 824, 111, 116, 59, 3, 8949, 824, 4, 3, 97, 98, 99, 13820, 13823, 13826, 59, 1, 8713, 59, 1, 8951, 59, 1, 8950, 105, 4, 2, 59, 118, 13836, 13838, 1, 8716, 4, 3, 97, 98, 99, 13846, 13849, 13852, 59, 1, 8716, 59, 1, 8958, 59, 1, 8957, 4, 3, 97, 111, 114, 13863, 13892, 13899, 114, 4, 4, 59, 97, 115, 116, 13874, 13876, 13883, 13888, 1, 8742, 108, 108, 101, 108, 59, 1, 8742, 108, 59, 3, 11005, 8421, 59, 3, 8706, 824, 108, 105, 110, 116, 59, 1, 10772, 4, 3, 59, 99, 101, 13907, 13909, 13914, 1, 8832, 117, 101, 59, 1, 8928, 4, 2, 59, 99, 13920, 13923, 3, 10927, 824, 4, 2, 59, 101, 13929, 13931, 1, 8832, 113, 59, 3, 10927, 824, 4, 4, 65, 97, 105, 116, 13946, 13951, 13971, 13982, 114, 114, 59, 1, 8655, 114, 114, 4, 3, 59, 99, 119, 13961, 13963, 13967, 1, 8603, 59, 3, 10547, 824, 59, 3, 8605, 824, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8603, 114, 105, 4, 2, 59, 101, 13990, 13992, 1, 8939, 59, 1, 8941, 4, 7, 99, 104, 105, 109, 112, 113, 117, 14011, 14036, 14060, 14080, 14085, 14090, 14106, 4, 4, 59, 99, 101, 114, 14021, 14023, 14028, 14032, 1, 8833, 117, 101, 59, 1, 8929, 59, 3, 10928, 824, 59, 3, 55349, 56515, 111, 114, 116, 4, 2, 109, 112, 14045, 14050, 105, 100, 59, 1, 8740, 97, 114, 97, 108, 108, 101, 108, 59, 1, 8742, 109, 4, 2, 59, 101, 14067, 14069, 1, 8769, 4, 2, 59, 113, 14075, 14077, 1, 8772, 59, 1, 8772, 105, 100, 59, 1, 8740, 97, 114, 59, 1, 8742, 115, 117, 4, 2, 98, 112, 14098, 14102, 101, 59, 1, 8930, 101, 59, 1, 8931, 4, 3, 98, 99, 112, 14114, 14157, 14171, 4, 4, 59, 69, 101, 115, 14124, 14126, 14130, 14133, 1, 8836, 59, 3, 10949, 824, 59, 1, 8840, 101, 116, 4, 2, 59, 101, 14141, 14144, 3, 8834, 8402, 113, 4, 2, 59, 113, 14151, 14153, 1, 8840, 59, 3, 10949, 824, 99, 4, 2, 59, 101, 14164, 14166, 1, 8833, 113, 59, 3, 10928, 824, 4, 4, 59, 69, 101, 115, 14181, 14183, 14187, 14190, 1, 8837, 59, 3, 10950, 824, 59, 1, 8841, 101, 116, 4, 2, 59, 101, 14198, 14201, 3, 8835, 8402, 113, 4, 2, 59, 113, 14208, 14210, 1, 8841, 59, 3, 10950, 824, 4, 4, 103, 105, 108, 114, 14224, 14228, 14238, 14242, 108, 59, 1, 8825, 108, 100, 101, 5, 241, 1, 59, 14236, 1, 241, 103, 59, 1, 8824, 105, 97, 110, 103, 108, 101, 4, 2, 108, 114, 14254, 14269, 101, 102, 116, 4, 2, 59, 101, 14263, 14265, 1, 8938, 113, 59, 1, 8940, 105, 103, 104, 116, 4, 2, 59, 101, 14279, 14281, 1, 8939, 113, 59, 1, 8941, 4, 2, 59, 109, 14291, 14293, 1, 957, 4, 3, 59, 101, 115, 14301, 14303, 14308, 1, 35, 114, 111, 59, 1, 8470, 112, 59, 1, 8199, 4, 9, 68, 72, 97, 100, 103, 105, 108, 114, 115, 14332, 14338, 14344, 14349, 14355, 14369, 14376, 14408, 14426, 97, 115, 104, 59, 1, 8877, 97, 114, 114, 59, 1, 10500, 112, 59, 3, 8781, 8402, 97, 115, 104, 59, 1, 8876, 4, 2, 101, 116, 14361, 14365, 59, 3, 8805, 8402, 59, 3, 62, 8402, 110, 102, 105, 110, 59, 1, 10718, 4, 3, 65, 101, 116, 14384, 14389, 14393, 114, 114, 59, 1, 10498, 59, 3, 8804, 8402, 4, 2, 59, 114, 14399, 14402, 3, 60, 8402, 105, 101, 59, 3, 8884, 8402, 4, 2, 65, 116, 14414, 14419, 114, 114, 59, 1, 10499, 114, 105, 101, 59, 3, 8885, 8402, 105, 109, 59, 3, 8764, 8402, 4, 3, 65, 97, 110, 14440, 14445, 14468, 114, 114, 59, 1, 8662, 114, 4, 2, 104, 114, 14452, 14456, 107, 59, 1, 10531, 4, 2, 59, 111, 14462, 14464, 1, 8598, 119, 59, 1, 8598, 101, 97, 114, 59, 1, 10535, 4, 18, 83, 97, 99, 100, 101, 102, 103, 104, 105, 108, 109, 111, 112, 114, 115, 116, 117, 118, 14512, 14515, 14535, 14560, 14597, 14603, 14618, 14643, 14657, 14662, 14701, 14741, 14747, 14769, 14851, 14877, 14907, 14916, 59, 1, 9416, 4, 2, 99, 115, 14521, 14531, 117, 116, 101, 5, 243, 1, 59, 14529, 1, 243, 116, 59, 1, 8859, 4, 2, 105, 121, 14541, 14557, 114, 4, 2, 59, 99, 14548, 14550, 1, 8858, 5, 244, 1, 59, 14555, 1, 244, 59, 1, 1086, 4, 5, 97, 98, 105, 111, 115, 14572, 14577, 14583, 14587, 14591, 115, 104, 59, 1, 8861, 108, 97, 99, 59, 1, 337, 118, 59, 1, 10808, 116, 59, 1, 8857, 111, 108, 100, 59, 1, 10684, 108, 105, 103, 59, 1, 339, 4, 2, 99, 114, 14609, 14614, 105, 114, 59, 1, 10687, 59, 3, 55349, 56620, 4, 3, 111, 114, 116, 14626, 14630, 14640, 110, 59, 1, 731, 97, 118, 101, 5, 242, 1, 59, 14638, 1, 242, 59, 1, 10689, 4, 2, 98, 109, 14649, 14654, 97, 114, 59, 1, 10677, 59, 1, 937, 110, 116, 59, 1, 8750, 4, 4, 97, 99, 105, 116, 14672, 14677, 14693, 14698, 114, 114, 59, 1, 8634, 4, 2, 105, 114, 14683, 14687, 114, 59, 1, 10686, 111, 115, 115, 59, 1, 10683, 110, 101, 59, 1, 8254, 59, 1, 10688, 4, 3, 97, 101, 105, 14709, 14714, 14719, 99, 114, 59, 1, 333, 103, 97, 59, 1, 969, 4, 3, 99, 100, 110, 14727, 14733, 14736, 114, 111, 110, 59, 1, 959, 59, 1, 10678, 117, 115, 59, 1, 8854, 112, 102, 59, 3, 55349, 56672, 4, 3, 97, 101, 108, 14755, 14759, 14764, 114, 59, 1, 10679, 114, 112, 59, 1, 10681, 117, 115, 59, 1, 8853, 4, 7, 59, 97, 100, 105, 111, 115, 118, 14785, 14787, 14792, 14831, 14837, 14841, 14848, 1, 8744, 114, 114, 59, 1, 8635, 4, 4, 59, 101, 102, 109, 14802, 14804, 14817, 14824, 1, 10845, 114, 4, 2, 59, 111, 14811, 14813, 1, 8500, 102, 59, 1, 8500, 5, 170, 1, 59, 14822, 1, 170, 5, 186, 1, 59, 14829, 1, 186, 103, 111, 102, 59, 1, 8886, 114, 59, 1, 10838, 108, 111, 112, 101, 59, 1, 10839, 59, 1, 10843, 4, 3, 99, 108, 111, 14859, 14863, 14873, 114, 59, 1, 8500, 97, 115, 104, 5, 248, 1, 59, 14871, 1, 248, 108, 59, 1, 8856, 105, 4, 2, 108, 109, 14884, 14893, 100, 101, 5, 245, 1, 59, 14891, 1, 245, 101, 115, 4, 2, 59, 97, 14901, 14903, 1, 8855, 115, 59, 1, 10806, 109, 108, 5, 246, 1, 59, 14914, 1, 246, 98, 97, 114, 59, 1, 9021, 4, 12, 97, 99, 101, 102, 104, 105, 108, 109, 111, 114, 115, 117, 14948, 14992, 14996, 15033, 15038, 15068, 15090, 15189, 15192, 15222, 15427, 15441, 114, 4, 4, 59, 97, 115, 116, 14959, 14961, 14976, 14989, 1, 8741, 5, 182, 2, 59, 108, 14968, 14970, 1, 182, 108, 101, 108, 59, 1, 8741, 4, 2, 105, 108, 14982, 14986, 109, 59, 1, 10995, 59, 1, 11005, 59, 1, 8706, 121, 59, 1, 1087, 114, 4, 5, 99, 105, 109, 112, 116, 15009, 15014, 15019, 15024, 15027, 110, 116, 59, 1, 37, 111, 100, 59, 1, 46, 105, 108, 59, 1, 8240, 59, 1, 8869, 101, 110, 107, 59, 1, 8241, 114, 59, 3, 55349, 56621, 4, 3, 105, 109, 111, 15046, 15057, 15063, 4, 2, 59, 118, 15052, 15054, 1, 966, 59, 1, 981, 109, 97, 116, 59, 1, 8499, 110, 101, 59, 1, 9742, 4, 3, 59, 116, 118, 15076, 15078, 15087, 1, 960, 99, 104, 102, 111, 114, 107, 59, 1, 8916, 59, 1, 982, 4, 2, 97, 117, 15096, 15119, 110, 4, 2, 99, 107, 15103, 15115, 107, 4, 2, 59, 104, 15110, 15112, 1, 8463, 59, 1, 8462, 118, 59, 1, 8463, 115, 4, 9, 59, 97, 98, 99, 100, 101, 109, 115, 116, 15140, 15142, 15148, 15151, 15156, 15168, 15171, 15179, 15184, 1, 43, 99, 105, 114, 59, 1, 10787, 59, 1, 8862, 105, 114, 59, 1, 10786, 4, 2, 111, 117, 15162, 15165, 59, 1, 8724, 59, 1, 10789, 59, 1, 10866, 110, 5, 177, 1, 59, 15177, 1, 177, 105, 109, 59, 1, 10790, 119, 111, 59, 1, 10791, 59, 1, 177, 4, 3, 105, 112, 117, 15200, 15208, 15213, 110, 116, 105, 110, 116, 59, 1, 10773, 102, 59, 3, 55349, 56673, 110, 100, 5, 163, 1, 59, 15220, 1, 163, 4, 10, 59, 69, 97, 99, 101, 105, 110, 111, 115, 117, 15244, 15246, 15249, 15253, 15258, 15334, 15347, 15367, 15416, 15421, 1, 8826, 59, 1, 10931, 112, 59, 1, 10935, 117, 101, 59, 1, 8828, 4, 2, 59, 99, 15264, 15266, 1, 10927, 4, 6, 59, 97, 99, 101, 110, 115, 15280, 15282, 15290, 15299, 15303, 15329, 1, 8826, 112, 112, 114, 111, 120, 59, 1, 10935, 117, 114, 108, 121, 101, 113, 59, 1, 8828, 113, 59, 1, 10927, 4, 3, 97, 101, 115, 15311, 15319, 15324, 112, 112, 114, 111, 120, 59, 1, 10937, 113, 113, 59, 1, 10933, 105, 109, 59, 1, 8936, 105, 109, 59, 1, 8830, 109, 101, 4, 2, 59, 115, 15342, 15344, 1, 8242, 59, 1, 8473, 4, 3, 69, 97, 115, 15355, 15358, 15362, 59, 1, 10933, 112, 59, 1, 10937, 105, 109, 59, 1, 8936, 4, 3, 100, 102, 112, 15375, 15378, 15404, 59, 1, 8719, 4, 3, 97, 108, 115, 15386, 15392, 15398, 108, 97, 114, 59, 1, 9006, 105, 110, 101, 59, 1, 8978, 117, 114, 102, 59, 1, 8979, 4, 2, 59, 116, 15410, 15412, 1, 8733, 111, 59, 1, 8733, 105, 109, 59, 1, 8830, 114, 101, 108, 59, 1, 8880, 4, 2, 99, 105, 15433, 15438, 114, 59, 3, 55349, 56517, 59, 1, 968, 110, 99, 115, 112, 59, 1, 8200, 4, 6, 102, 105, 111, 112, 115, 117, 15462, 15467, 15472, 15478, 15485, 15491, 114, 59, 3, 55349, 56622, 110, 116, 59, 1, 10764, 112, 102, 59, 3, 55349, 56674, 114, 105, 109, 101, 59, 1, 8279, 99, 114, 59, 3, 55349, 56518, 4, 3, 97, 101, 111, 15499, 15520, 15534, 116, 4, 2, 101, 105, 15506, 15515, 114, 110, 105, 111, 110, 115, 59, 1, 8461, 110, 116, 59, 1, 10774, 115, 116, 4, 2, 59, 101, 15528, 15530, 1, 63, 113, 59, 1, 8799, 116, 5, 34, 1, 59, 15540, 1, 34, 4, 21, 65, 66, 72, 97, 98, 99, 100, 101, 102, 104, 105, 108, 109, 110, 111, 112, 114, 115, 116, 117, 120, 15586, 15609, 15615, 15620, 15796, 15855, 15893, 15931, 15977, 16001, 16039, 16183, 16204, 16222, 16228, 16285, 16312, 16318, 16363, 16408, 16416, 4, 3, 97, 114, 116, 15594, 15599, 15603, 114, 114, 59, 1, 8667, 114, 59, 1, 8658, 97, 105, 108, 59, 1, 10524, 97, 114, 114, 59, 1, 10511, 97, 114, 59, 1, 10596, 4, 7, 99, 100, 101, 110, 113, 114, 116, 15636, 15651, 15656, 15664, 15687, 15696, 15770, 4, 2, 101, 117, 15642, 15646, 59, 3, 8765, 817, 116, 101, 59, 1, 341, 105, 99, 59, 1, 8730, 109, 112, 116, 121, 118, 59, 1, 10675, 103, 4, 4, 59, 100, 101, 108, 15675, 15677, 15680, 15683, 1, 10217, 59, 1, 10642, 59, 1, 10661, 101, 59, 1, 10217, 117, 111, 5, 187, 1, 59, 15694, 1, 187, 114, 4, 11, 59, 97, 98, 99, 102, 104, 108, 112, 115, 116, 119, 15721, 15723, 15727, 15739, 15742, 15746, 15750, 15754, 15758, 15763, 15767, 1, 8594, 112, 59, 1, 10613, 4, 2, 59, 102, 15733, 15735, 1, 8677, 115, 59, 1, 10528, 59, 1, 10547, 115, 59, 1, 10526, 107, 59, 1, 8618, 112, 59, 1, 8620, 108, 59, 1, 10565, 105, 109, 59, 1, 10612, 108, 59, 1, 8611, 59, 1, 8605, 4, 2, 97, 105, 15776, 15781, 105, 108, 59, 1, 10522, 111, 4, 2, 59, 110, 15788, 15790, 1, 8758, 97, 108, 115, 59, 1, 8474, 4, 3, 97, 98, 114, 15804, 15809, 15814, 114, 114, 59, 1, 10509, 114, 107, 59, 1, 10099, 4, 2, 97, 107, 15820, 15833, 99, 4, 2, 101, 107, 15827, 15830, 59, 1, 125, 59, 1, 93, 4, 2, 101, 115, 15839, 15842, 59, 1, 10636, 108, 4, 2, 100, 117, 15849, 15852, 59, 1, 10638, 59, 1, 10640, 4, 4, 97, 101, 117, 121, 15865, 15871, 15886, 15890, 114, 111, 110, 59, 1, 345, 4, 2, 100, 105, 15877, 15882, 105, 108, 59, 1, 343, 108, 59, 1, 8969, 98, 59, 1, 125, 59, 1, 1088, 4, 4, 99, 108, 113, 115, 15903, 15907, 15914, 15927, 97, 59, 1, 10551, 100, 104, 97, 114, 59, 1, 10601, 117, 111, 4, 2, 59, 114, 15922, 15924, 1, 8221, 59, 1, 8221, 104, 59, 1, 8627, 4, 3, 97, 99, 103, 15939, 15966, 15970, 108, 4, 4, 59, 105, 112, 115, 15950, 15952, 15957, 15963, 1, 8476, 110, 101, 59, 1, 8475, 97, 114, 116, 59, 1, 8476, 59, 1, 8477, 116, 59, 1, 9645, 5, 174, 1, 59, 15975, 1, 174, 4, 3, 105, 108, 114, 15985, 15991, 15997, 115, 104, 116, 59, 1, 10621, 111, 111, 114, 59, 1, 8971, 59, 3, 55349, 56623, 4, 2, 97, 111, 16007, 16028, 114, 4, 2, 100, 117, 16014, 16017, 59, 1, 8641, 4, 2, 59, 108, 16023, 16025, 1, 8640, 59, 1, 10604, 4, 2, 59, 118, 16034, 16036, 1, 961, 59, 1, 1009, 4, 3, 103, 110, 115, 16047, 16167, 16171, 104, 116, 4, 6, 97, 104, 108, 114, 115, 116, 16063, 16081, 16103, 16130, 16143, 16155, 114, 114, 111, 119, 4, 2, 59, 116, 16073, 16075, 1, 8594, 97, 105, 108, 59, 1, 8611, 97, 114, 112, 111, 111, 110, 4, 2, 100, 117, 16093, 16099, 111, 119, 110, 59, 1, 8641, 112, 59, 1, 8640, 101, 102, 116, 4, 2, 97, 104, 16112, 16120, 114, 114, 111, 119, 115, 59, 1, 8644, 97, 114, 112, 111, 111, 110, 115, 59, 1, 8652, 105, 103, 104, 116, 97, 114, 114, 111, 119, 115, 59, 1, 8649, 113, 117, 105, 103, 97, 114, 114, 111, 119, 59, 1, 8605, 104, 114, 101, 101, 116, 105, 109, 101, 115, 59, 1, 8908, 103, 59, 1, 730, 105, 110, 103, 100, 111, 116, 115, 101, 113, 59, 1, 8787, 4, 3, 97, 104, 109, 16191, 16196, 16201, 114, 114, 59, 1, 8644, 97, 114, 59, 1, 8652, 59, 1, 8207, 111, 117, 115, 116, 4, 2, 59, 97, 16214, 16216, 1, 9137, 99, 104, 101, 59, 1, 9137, 109, 105, 100, 59, 1, 10990, 4, 4, 97, 98, 112, 116, 16238, 16252, 16257, 16278, 4, 2, 110, 114, 16244, 16248, 103, 59, 1, 10221, 114, 59, 1, 8702, 114, 107, 59, 1, 10215, 4, 3, 97, 102, 108, 16265, 16269, 16273, 114, 59, 1, 10630, 59, 3, 55349, 56675, 117, 115, 59, 1, 10798, 105, 109, 101, 115, 59, 1, 10805, 4, 2, 97, 112, 16291, 16304, 114, 4, 2, 59, 103, 16298, 16300, 1, 41, 116, 59, 1, 10644, 111, 108, 105, 110, 116, 59, 1, 10770, 97, 114, 114, 59, 1, 8649, 4, 4, 97, 99, 104, 113, 16328, 16334, 16339, 16342, 113, 117, 111, 59, 1, 8250, 114, 59, 3, 55349, 56519, 59, 1, 8625, 4, 2, 98, 117, 16348, 16351, 59, 1, 93, 111, 4, 2, 59, 114, 16358, 16360, 1, 8217, 59, 1, 8217, 4, 3, 104, 105, 114, 16371, 16377, 16383, 114, 101, 101, 59, 1, 8908, 109, 101, 115, 59, 1, 8906, 105, 4, 4, 59, 101, 102, 108, 16394, 16396, 16399, 16402, 1, 9657, 59, 1, 8885, 59, 1, 9656, 116, 114, 105, 59, 1, 10702, 108, 117, 104, 97, 114, 59, 1, 10600, 59, 1, 8478, 4, 19, 97, 98, 99, 100, 101, 102, 104, 105, 108, 109, 111, 112, 113, 114, 115, 116, 117, 119, 122, 16459, 16466, 16472, 16572, 16590, 16672, 16687, 16746, 16844, 16850, 16924, 16963, 16988, 17115, 17121, 17154, 17206, 17614, 17656, 99, 117, 116, 101, 59, 1, 347, 113, 117, 111, 59, 1, 8218, 4, 10, 59, 69, 97, 99, 101, 105, 110, 112, 115, 121, 16494, 16496, 16499, 16513, 16518, 16531, 16536, 16556, 16564, 16569, 1, 8827, 59, 1, 10932, 4, 2, 112, 114, 16505, 16508, 59, 1, 10936, 111, 110, 59, 1, 353, 117, 101, 59, 1, 8829, 4, 2, 59, 100, 16524, 16526, 1, 10928, 105, 108, 59, 1, 351, 114, 99, 59, 1, 349, 4, 3, 69, 97, 115, 16544, 16547, 16551, 59, 1, 10934, 112, 59, 1, 10938, 105, 109, 59, 1, 8937, 111, 108, 105, 110, 116, 59, 1, 10771, 105, 109, 59, 1, 8831, 59, 1, 1089, 111, 116, 4, 3, 59, 98, 101, 16582, 16584, 16587, 1, 8901, 59, 1, 8865, 59, 1, 10854, 4, 7, 65, 97, 99, 109, 115, 116, 120, 16606, 16611, 16634, 16642, 16646, 16652, 16668, 114, 114, 59, 1, 8664, 114, 4, 2, 104, 114, 16618, 16622, 107, 59, 1, 10533, 4, 2, 59, 111, 16628, 16630, 1, 8600, 119, 59, 1, 8600, 116, 5, 167, 1, 59, 16640, 1, 167, 105, 59, 1, 59, 119, 97, 114, 59, 1, 10537, 109, 4, 2, 105, 110, 16659, 16665, 110, 117, 115, 59, 1, 8726, 59, 1, 8726, 116, 59, 1, 10038, 114, 4, 2, 59, 111, 16679, 16682, 3, 55349, 56624, 119, 110, 59, 1, 8994, 4, 4, 97, 99, 111, 121, 16697, 16702, 16716, 16739, 114, 112, 59, 1, 9839, 4, 2, 104, 121, 16708, 16713, 99, 121, 59, 1, 1097, 59, 1, 1096, 114, 116, 4, 2, 109, 112, 16724, 16729, 105, 100, 59, 1, 8739, 97, 114, 97, 108, 108, 101, 108, 59, 1, 8741, 5, 173, 1, 59, 16744, 1, 173, 4, 2, 103, 109, 16752, 16770, 109, 97, 4, 3, 59, 102, 118, 16762, 16764, 16767, 1, 963, 59, 1, 962, 59, 1, 962, 4, 8, 59, 100, 101, 103, 108, 110, 112, 114, 16788, 16790, 16795, 16806, 16817, 16828, 16832, 16838, 1, 8764, 111, 116, 59, 1, 10858, 4, 2, 59, 113, 16801, 16803, 1, 8771, 59, 1, 8771, 4, 2, 59, 69, 16812, 16814, 1, 10910, 59, 1, 10912, 4, 2, 59, 69, 16823, 16825, 1, 10909, 59, 1, 10911, 101, 59, 1, 8774, 108, 117, 115, 59, 1, 10788, 97, 114, 114, 59, 1, 10610, 97, 114, 114, 59, 1, 8592, 4, 4, 97, 101, 105, 116, 16860, 16883, 16891, 16904, 4, 2, 108, 115, 16866, 16878, 108, 115, 101, 116, 109, 105, 110, 117, 115, 59, 1, 8726, 104, 112, 59, 1, 10803, 112, 97, 114, 115, 108, 59, 1, 10724, 4, 2, 100, 108, 16897, 16900, 59, 1, 8739, 101, 59, 1, 8995, 4, 2, 59, 101, 16910, 16912, 1, 10922, 4, 2, 59, 115, 16918, 16920, 1, 10924, 59, 3, 10924, 65024, 4, 3, 102, 108, 112, 16932, 16938, 16958, 116, 99, 121, 59, 1, 1100, 4, 2, 59, 98, 16944, 16946, 1, 47, 4, 2, 59, 97, 16952, 16954, 1, 10692, 114, 59, 1, 9023, 102, 59, 3, 55349, 56676, 97, 4, 2, 100, 114, 16970, 16985, 101, 115, 4, 2, 59, 117, 16978, 16980, 1, 9824, 105, 116, 59, 1, 9824, 59, 1, 8741, 4, 3, 99, 115, 117, 16996, 17028, 17089, 4, 2, 97, 117, 17002, 17015, 112, 4, 2, 59, 115, 17009, 17011, 1, 8851, 59, 3, 8851, 65024, 112, 4, 2, 59, 115, 17022, 17024, 1, 8852, 59, 3, 8852, 65024, 117, 4, 2, 98, 112, 17035, 17062, 4, 3, 59, 101, 115, 17043, 17045, 17048, 1, 8847, 59, 1, 8849, 101, 116, 4, 2, 59, 101, 17056, 17058, 1, 8847, 113, 59, 1, 8849, 4, 3, 59, 101, 115, 17070, 17072, 17075, 1, 8848, 59, 1, 8850, 101, 116, 4, 2, 59, 101, 17083, 17085, 1, 8848, 113, 59, 1, 8850, 4, 3, 59, 97, 102, 17097, 17099, 17112, 1, 9633, 114, 4, 2, 101, 102, 17106, 17109, 59, 1, 9633, 59, 1, 9642, 59, 1, 9642, 97, 114, 114, 59, 1, 8594, 4, 4, 99, 101, 109, 116, 17131, 17136, 17142, 17148, 114, 59, 3, 55349, 56520, 116, 109, 110, 59, 1, 8726, 105, 108, 101, 59, 1, 8995, 97, 114, 102, 59, 1, 8902, 4, 2, 97, 114, 17160, 17172, 114, 4, 2, 59, 102, 17167, 17169, 1, 9734, 59, 1, 9733, 4, 2, 97, 110, 17178, 17202, 105, 103, 104, 116, 4, 2, 101, 112, 17188, 17197, 112, 115, 105, 108, 111, 110, 59, 1, 1013, 104, 105, 59, 1, 981, 115, 59, 1, 175, 4, 5, 98, 99, 109, 110, 112, 17218, 17351, 17420, 17423, 17427, 4, 9, 59, 69, 100, 101, 109, 110, 112, 114, 115, 17238, 17240, 17243, 17248, 17261, 17267, 17279, 17285, 17291, 1, 8834, 59, 1, 10949, 111, 116, 59, 1, 10941, 4, 2, 59, 100, 17254, 17256, 1, 8838, 111, 116, 59, 1, 10947, 117, 108, 116, 59, 1, 10945, 4, 2, 69, 101, 17273, 17276, 59, 1, 10955, 59, 1, 8842, 108, 117, 115, 59, 1, 10943, 97, 114, 114, 59, 1, 10617, 4, 3, 101, 105, 117, 17299, 17335, 17339, 116, 4, 3, 59, 101, 110, 17308, 17310, 17322, 1, 8834, 113, 4, 2, 59, 113, 17317, 17319, 1, 8838, 59, 1, 10949, 101, 113, 4, 2, 59, 113, 17330, 17332, 1, 8842, 59, 1, 10955, 109, 59, 1, 10951, 4, 2, 98, 112, 17345, 17348, 59, 1, 10965, 59, 1, 10963, 99, 4, 6, 59, 97, 99, 101, 110, 115, 17366, 17368, 17376, 17385, 17389, 17415, 1, 8827, 112, 112, 114, 111, 120, 59, 1, 10936, 117, 114, 108, 121, 101, 113, 59, 1, 8829, 113, 59, 1, 10928, 4, 3, 97, 101, 115, 17397, 17405, 17410, 112, 112, 114, 111, 120, 59, 1, 10938, 113, 113, 59, 1, 10934, 105, 109, 59, 1, 8937, 105, 109, 59, 1, 8831, 59, 1, 8721, 103, 59, 1, 9834, 4, 13, 49, 50, 51, 59, 69, 100, 101, 104, 108, 109, 110, 112, 115, 17455, 17462, 17469, 17476, 17478, 17481, 17496, 17509, 17524, 17530, 17536, 17548, 17554, 5, 185, 1, 59, 17460, 1, 185, 5, 178, 1, 59, 17467, 1, 178, 5, 179, 1, 59, 17474, 1, 179, 1, 8835, 59, 1, 10950, 4, 2, 111, 115, 17487, 17491, 116, 59, 1, 10942, 117, 98, 59, 1, 10968, 4, 2, 59, 100, 17502, 17504, 1, 8839, 111, 116, 59, 1, 10948, 115, 4, 2, 111, 117, 17516, 17520, 108, 59, 1, 10185, 98, 59, 1, 10967, 97, 114, 114, 59, 1, 10619, 117, 108, 116, 59, 1, 10946, 4, 2, 69, 101, 17542, 17545, 59, 1, 10956, 59, 1, 8843, 108, 117, 115, 59, 1, 10944, 4, 3, 101, 105, 117, 17562, 17598, 17602, 116, 4, 3, 59, 101, 110, 17571, 17573, 17585, 1, 8835, 113, 4, 2, 59, 113, 17580, 17582, 1, 8839, 59, 1, 10950, 101, 113, 4, 2, 59, 113, 17593, 17595, 1, 8843, 59, 1, 10956, 109, 59, 1, 10952, 4, 2, 98, 112, 17608, 17611, 59, 1, 10964, 59, 1, 10966, 4, 3, 65, 97, 110, 17622, 17627, 17650, 114, 114, 59, 1, 8665, 114, 4, 2, 104, 114, 17634, 17638, 107, 59, 1, 10534, 4, 2, 59, 111, 17644, 17646, 1, 8601, 119, 59, 1, 8601, 119, 97, 114, 59, 1, 10538, 108, 105, 103, 5, 223, 1, 59, 17664, 1, 223, 4, 13, 97, 98, 99, 100, 101, 102, 104, 105, 111, 112, 114, 115, 119, 17694, 17709, 17714, 17737, 17742, 17749, 17754, 17860, 17905, 17957, 17964, 18090, 18122, 4, 2, 114, 117, 17700, 17706, 103, 101, 116, 59, 1, 8982, 59, 1, 964, 114, 107, 59, 1, 9140, 4, 3, 97, 101, 121, 17722, 17728, 17734, 114, 111, 110, 59, 1, 357, 100, 105, 108, 59, 1, 355, 59, 1, 1090, 111, 116, 59, 1, 8411, 108, 114, 101, 99, 59, 1, 8981, 114, 59, 3, 55349, 56625, 4, 4, 101, 105, 107, 111, 17764, 17805, 17836, 17851, 4, 2, 114, 116, 17770, 17786, 101, 4, 2, 52, 102, 17777, 17780, 59, 1, 8756, 111, 114, 101, 59, 1, 8756, 97, 4, 3, 59, 115, 118, 17795, 17797, 17802, 1, 952, 121, 109, 59, 1, 977, 59, 1, 977, 4, 2, 99, 110, 17811, 17831, 107, 4, 2, 97, 115, 17818, 17826, 112, 112, 114, 111, 120, 59, 1, 8776, 105, 109, 59, 1, 8764, 115, 112, 59, 1, 8201, 4, 2, 97, 115, 17842, 17846, 112, 59, 1, 8776, 105, 109, 59, 1, 8764, 114, 110, 5, 254, 1, 59, 17858, 1, 254, 4, 3, 108, 109, 110, 17868, 17873, 17901, 100, 101, 59, 1, 732, 101, 115, 5, 215, 3, 59, 98, 100, 17884, 17886, 17898, 1, 215, 4, 2, 59, 97, 17892, 17894, 1, 8864, 114, 59, 1, 10801, 59, 1, 10800, 116, 59, 1, 8749, 4, 3, 101, 112, 115, 17913, 17917, 17953, 97, 59, 1, 10536, 4, 4, 59, 98, 99, 102, 17927, 17929, 17934, 17939, 1, 8868, 111, 116, 59, 1, 9014, 105, 114, 59, 1, 10993, 4, 2, 59, 111, 17945, 17948, 3, 55349, 56677, 114, 107, 59, 1, 10970, 97, 59, 1, 10537, 114, 105, 109, 101, 59, 1, 8244, 4, 3, 97, 105, 112, 17972, 17977, 18082, 100, 101, 59, 1, 8482, 4, 7, 97, 100, 101, 109, 112, 115, 116, 17993, 18051, 18056, 18059, 18066, 18072, 18076, 110, 103, 108, 101, 4, 5, 59, 100, 108, 113, 114, 18009, 18011, 18017, 18032, 18035, 1, 9653, 111, 119, 110, 59, 1, 9663, 101, 102, 116, 4, 2, 59, 101, 18026, 18028, 1, 9667, 113, 59, 1, 8884, 59, 1, 8796, 105, 103, 104, 116, 4, 2, 59, 101, 18045, 18047, 1, 9657, 113, 59, 1, 8885, 111, 116, 59, 1, 9708, 59, 1, 8796, 105, 110, 117, 115, 59, 1, 10810, 108, 117, 115, 59, 1, 10809, 98, 59, 1, 10701, 105, 109, 101, 59, 1, 10811, 101, 122, 105, 117, 109, 59, 1, 9186, 4, 3, 99, 104, 116, 18098, 18111, 18116, 4, 2, 114, 121, 18104, 18108, 59, 3, 55349, 56521, 59, 1, 1094, 99, 121, 59, 1, 1115, 114, 111, 107, 59, 1, 359, 4, 2, 105, 111, 18128, 18133, 120, 116, 59, 1, 8812, 104, 101, 97, 100, 4, 2, 108, 114, 18143, 18154, 101, 102, 116, 97, 114, 114, 111, 119, 59, 1, 8606, 105, 103, 104, 116, 97, 114, 114, 111, 119, 59, 1, 8608, 4, 18, 65, 72, 97, 98, 99, 100, 102, 103, 104, 108, 109, 111, 112, 114, 115, 116, 117, 119, 18204, 18209, 18214, 18234, 18250, 18268, 18292, 18308, 18319, 18343, 18379, 18397, 18413, 18504, 18547, 18553, 18584, 18603, 114, 114, 59, 1, 8657, 97, 114, 59, 1, 10595, 4, 2, 99, 114, 18220, 18230, 117, 116, 101, 5, 250, 1, 59, 18228, 1, 250, 114, 59, 1, 8593, 114, 4, 2, 99, 101, 18241, 18245, 121, 59, 1, 1118, 118, 101, 59, 1, 365, 4, 2, 105, 121, 18256, 18265, 114, 99, 5, 251, 1, 59, 18263, 1, 251, 59, 1, 1091, 4, 3, 97, 98, 104, 18276, 18281, 18287, 114, 114, 59, 1, 8645, 108, 97, 99, 59, 1, 369, 97, 114, 59, 1, 10606, 4, 2, 105, 114, 18298, 18304, 115, 104, 116, 59, 1, 10622, 59, 3, 55349, 56626, 114, 97, 118, 101, 5, 249, 1, 59, 18317, 1, 249, 4, 2, 97, 98, 18325, 18338, 114, 4, 2, 108, 114, 18332, 18335, 59, 1, 8639, 59, 1, 8638, 108, 107, 59, 1, 9600, 4, 2, 99, 116, 18349, 18374, 4, 2, 111, 114, 18355, 18369, 114, 110, 4, 2, 59, 101, 18363, 18365, 1, 8988, 114, 59, 1, 8988, 111, 112, 59, 1, 8975, 114, 105, 59, 1, 9720, 4, 2, 97, 108, 18385, 18390, 99, 114, 59, 1, 363, 5, 168, 1, 59, 18395, 1, 168, 4, 2, 103, 112, 18403, 18408, 111, 110, 59, 1, 371, 102, 59, 3, 55349, 56678, 4, 6, 97, 100, 104, 108, 115, 117, 18427, 18434, 18445, 18470, 18475, 18494, 114, 114, 111, 119, 59, 1, 8593, 111, 119, 110, 97, 114, 114, 111, 119, 59, 1, 8597, 97, 114, 112, 111, 111, 110, 4, 2, 108, 114, 18457, 18463, 101, 102, 116, 59, 1, 8639, 105, 103, 104, 116, 59, 1, 8638, 117, 115, 59, 1, 8846, 105, 4, 3, 59, 104, 108, 18484, 18486, 18489, 1, 965, 59, 1, 978, 111, 110, 59, 1, 965, 112, 97, 114, 114, 111, 119, 115, 59, 1, 8648, 4, 3, 99, 105, 116, 18512, 18537, 18542, 4, 2, 111, 114, 18518, 18532, 114, 110, 4, 2, 59, 101, 18526, 18528, 1, 8989, 114, 59, 1, 8989, 111, 112, 59, 1, 8974, 110, 103, 59, 1, 367, 114, 105, 59, 1, 9721, 99, 114, 59, 3, 55349, 56522, 4, 3, 100, 105, 114, 18561, 18566, 18572, 111, 116, 59, 1, 8944, 108, 100, 101, 59, 1, 361, 105, 4, 2, 59, 102, 18579, 18581, 1, 9653, 59, 1, 9652, 4, 2, 97, 109, 18590, 18595, 114, 114, 59, 1, 8648, 108, 5, 252, 1, 59, 18601, 1, 252, 97, 110, 103, 108, 101, 59, 1, 10663, 4, 15, 65, 66, 68, 97, 99, 100, 101, 102, 108, 110, 111, 112, 114, 115, 122, 18643, 18648, 18661, 18667, 18847, 18851, 18857, 18904, 18909, 18915, 18931, 18937, 18943, 18949, 18996, 114, 114, 59, 1, 8661, 97, 114, 4, 2, 59, 118, 18656, 18658, 1, 10984, 59, 1, 10985, 97, 115, 104, 59, 1, 8872, 4, 2, 110, 114, 18673, 18679, 103, 114, 116, 59, 1, 10652, 4, 7, 101, 107, 110, 112, 114, 115, 116, 18695, 18704, 18711, 18720, 18742, 18754, 18810, 112, 115, 105, 108, 111, 110, 59, 1, 1013, 97, 112, 112, 97, 59, 1, 1008, 111, 116, 104, 105, 110, 103, 59, 1, 8709, 4, 3, 104, 105, 114, 18728, 18732, 18735, 105, 59, 1, 981, 59, 1, 982, 111, 112, 116, 111, 59, 1, 8733, 4, 2, 59, 104, 18748, 18750, 1, 8597, 111, 59, 1, 1009, 4, 2, 105, 117, 18760, 18766, 103, 109, 97, 59, 1, 962, 4, 2, 98, 112, 18772, 18791, 115, 101, 116, 110, 101, 113, 4, 2, 59, 113, 18784, 18787, 3, 8842, 65024, 59, 3, 10955, 65024, 115, 101, 116, 110, 101, 113, 4, 2, 59, 113, 18803, 18806, 3, 8843, 65024, 59, 3, 10956, 65024, 4, 2, 104, 114, 18816, 18822, 101, 116, 97, 59, 1, 977, 105, 97, 110, 103, 108, 101, 4, 2, 108, 114, 18834, 18840, 101, 102, 116, 59, 1, 8882, 105, 103, 104, 116, 59, 1, 8883, 121, 59, 1, 1074, 97, 115, 104, 59, 1, 8866, 4, 3, 101, 108, 114, 18865, 18884, 18890, 4, 3, 59, 98, 101, 18873, 18875, 18880, 1, 8744, 97, 114, 59, 1, 8891, 113, 59, 1, 8794, 108, 105, 112, 59, 1, 8942, 4, 2, 98, 116, 18896, 18901, 97, 114, 59, 1, 124, 59, 1, 124, 114, 59, 3, 55349, 56627, 116, 114, 105, 59, 1, 8882, 115, 117, 4, 2, 98, 112, 18923, 18927, 59, 3, 8834, 8402, 59, 3, 8835, 8402, 112, 102, 59, 3, 55349, 56679, 114, 111, 112, 59, 1, 8733, 116, 114, 105, 59, 1, 8883, 4, 2, 99, 117, 18955, 18960, 114, 59, 3, 55349, 56523, 4, 2, 98, 112, 18966, 18981, 110, 4, 2, 69, 101, 18973, 18977, 59, 3, 10955, 65024, 59, 3, 8842, 65024, 110, 4, 2, 69, 101, 18988, 18992, 59, 3, 10956, 65024, 59, 3, 8843, 65024, 105, 103, 122, 97, 103, 59, 1, 10650, 4, 7, 99, 101, 102, 111, 112, 114, 115, 19020, 19026, 19061, 19066, 19072, 19075, 19089, 105, 114, 99, 59, 1, 373, 4, 2, 100, 105, 19032, 19055, 4, 2, 98, 103, 19038, 19043, 97, 114, 59, 1, 10847, 101, 4, 2, 59, 113, 19050, 19052, 1, 8743, 59, 1, 8793, 101, 114, 112, 59, 1, 8472, 114, 59, 3, 55349, 56628, 112, 102, 59, 3, 55349, 56680, 59, 1, 8472, 4, 2, 59, 101, 19081, 19083, 1, 8768, 97, 116, 104, 59, 1, 8768, 99, 114, 59, 3, 55349, 56524, 4, 14, 99, 100, 102, 104, 105, 108, 109, 110, 111, 114, 115, 117, 118, 119, 19125, 19146, 19152, 19157, 19173, 19176, 19192, 19197, 19202, 19236, 19252, 19269, 19286, 19291, 4, 3, 97, 105, 117, 19133, 19137, 19142, 112, 59, 1, 8898, 114, 99, 59, 1, 9711, 112, 59, 1, 8899, 116, 114, 105, 59, 1, 9661, 114, 59, 3, 55349, 56629, 4, 2, 65, 97, 19163, 19168, 114, 114, 59, 1, 10234, 114, 114, 59, 1, 10231, 59, 1, 958, 4, 2, 65, 97, 19182, 19187, 114, 114, 59, 1, 10232, 114, 114, 59, 1, 10229, 97, 112, 59, 1, 10236, 105, 115, 59, 1, 8955, 4, 3, 100, 112, 116, 19210, 19215, 19230, 111, 116, 59, 1, 10752, 4, 2, 102, 108, 19221, 19225, 59, 3, 55349, 56681, 117, 115, 59, 1, 10753, 105, 109, 101, 59, 1, 10754, 4, 2, 65, 97, 19242, 19247, 114, 114, 59, 1, 10233, 114, 114, 59, 1, 10230, 4, 2, 99, 113, 19258, 19263, 114, 59, 3, 55349, 56525, 99, 117, 112, 59, 1, 10758, 4, 2, 112, 116, 19275, 19281, 108, 117, 115, 59, 1, 10756, 114, 105, 59, 1, 9651, 101, 101, 59, 1, 8897, 101, 100, 103, 101, 59, 1, 8896, 4, 8, 97, 99, 101, 102, 105, 111, 115, 117, 19316, 19335, 19349, 19357, 19362, 19367, 19373, 19379, 99, 4, 2, 117, 121, 19323, 19332, 116, 101, 5, 253, 1, 59, 19330, 1, 253, 59, 1, 1103, 4, 2, 105, 121, 19341, 19346, 114, 99, 59, 1, 375, 59, 1, 1099, 110, 5, 165, 1, 59, 19355, 1, 165, 114, 59, 3, 55349, 56630, 99, 121, 59, 1, 1111, 112, 102, 59, 3, 55349, 56682, 99, 114, 59, 3, 55349, 56526, 4, 2, 99, 109, 19385, 19389, 121, 59, 1, 1102, 108, 5, 255, 1, 59, 19395, 1, 255, 4, 10, 97, 99, 100, 101, 102, 104, 105, 111, 115, 119, 19419, 19426, 19441, 19446, 19462, 19467, 19472, 19480, 19486, 19492, 99, 117, 116, 101, 59, 1, 378, 4, 2, 97, 121, 19432, 19438, 114, 111, 110, 59, 1, 382, 59, 1, 1079, 111, 116, 59, 1, 380, 4, 2, 101, 116, 19452, 19458, 116, 114, 102, 59, 1, 8488, 97, 59, 1, 950, 114, 59, 3, 55349, 56631, 99, 121, 59, 1, 1078, 103, 114, 97, 114, 114, 59, 1, 8669, 112, 102, 59, 3, 55349, 56683, 99, 114, 59, 3, 55349, 56527, 4, 2, 106, 110, 19498, 19501, 59, 1, 8205, 106, 59, 1, 8204])
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(54),
             a = o.TAG_NAMES,
             s = o.NAMESPACES;
 
         function u(e) {
             switch (e.length) {
                 case 1:
@@ -41430,16 +41430,16 @@
                     for (; u(this.currentTagName) && this.currentTagName !== e;) this.pop()
                 }
             }]), e
         }();
         e.exports = f
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = function() {
                 function e(t) {
                     r(this, e), this.length = 0, this.entries = [], this.treeAdapter = t, this.bookmark = null
                 }
                 return i(e, [{
                     key: "_getNoahArkConditionCandidates",
                     value: function(t) {
@@ -41538,16 +41538,16 @@
                         return null
                     }
                 }]), e
             }();
         o.MARKER_ENTRY = "MARKER_ENTRY", o.ELEMENT_ENTRY = "ELEMENT_ENTRY", e.exports = o
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(35),
             a = n(36),
             s = n(38),
             u = n(74),
             l = n(122),
             c = n(276),
             f = n(54).TAG_NAMES,
@@ -41663,16 +41663,16 @@
                         }
                     }
                 }]), n
             }(s);
         e.exports = d
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(35),
             a = n(36),
             s = function(e) {
                 o(n, e);
                 var t = a(n);
 
                 function n(e, i) {
@@ -41696,16 +41696,16 @@
                         }
                     }
                 }]), n
             }(n(38));
         e.exports = s
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(35),
             a = n(36),
             s = n(100),
             u = n(278),
             l = n(122),
             c = n(38),
             f = function(e) {
@@ -41737,15 +41737,15 @@
                         }
                     }
                 }]), n
             }(s);
         e.exports = f
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
+        var r = n(27),
             i = n(35),
             o = n(36),
             a = n(100),
             s = n(279),
             u = n(38),
             l = function(e) {
                 i(n, e);
@@ -41758,16 +41758,16 @@
                     return o.posTracker = a.posTracker, o
                 }
                 return n
             }(a);
         e.exports = l
     }, function(e, t, n) {
         "use strict";
-        var r = n(26),
-            i = n(28),
+        var r = n(27),
+            i = n(29),
             o = n(124),
             a = n(62),
             s = n(35),
             u = n(36),
             l = n(100),
             c = n(123),
             f = n(38),
@@ -42165,16 +42165,16 @@
     }, function(e, t, n) {}, function(e, t, n) {
         var r = n(124),
             i = n(62),
             o = n(287),
             a = n(72),
             s = n(35),
             u = n(36),
-            l = n(26),
-            c = n(28),
+            l = n(27),
+            c = n(29),
             f = n(121);
         e.exports = function(e) {
             "use strict";
 
             function t(e) {
                 if (e && e.__esModule) return e;
                 var t = Object.create(null);
@@ -44815,15 +44815,15 @@
                 Offcanvas: kt,
                 Popover: Qt,
                 ScrollSpy: on,
                 Tab: fn,
                 Toast: bn,
                 Tooltip: Wt
             }
-        }(n(294))
+        }(n(295))
     }, function(e, t, n) {
         var r = n(73);
 
         function i(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
@@ -44840,15 +44840,15 @@
                     r(e, t, n[t])
                 })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : i(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-    }, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, , function(e, t, n) {
+    }, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, function(e, t, n) {}, , , function(e, t, n) {
         "use strict";
         n.r(t), n.d(t, "top", (function() {
             return r
         })), n.d(t, "bottom", (function() {
             return i
         })), n.d(t, "right", (function() {
             return o
@@ -46015,15 +46015,15 @@
         var Ie = Se(),
             Ne = Se({
                 defaultModifiers: [ne, Te, ee, x, _e, ve, we, X, ye]
             }),
             xe = Se({
                 defaultModifiers: [ne, Te, ee, x]
             })
-    }, , , , , , , , , , , , , , , , , , function(e, t, n) {
+    }, , , , , , , , , , , , , , , , , function(e, t, n) {
         "use strict";
         n.d(t, "a", (function() {
             return _n
         }));
         var r = {};
         n.r(r), n.d(r, "document", (function() {
             return lt
@@ -46045,15 +46045,15 @@
             return vt
         }));
         var i = n(14),
             o = n(1),
             a = n.n(o),
             s = n(15),
             u = n(19),
-            l = n(24),
+            l = n(25),
             c = n(131),
             f = n.n(c),
             d = n(41),
             p = n(42),
             h = n(89),
             m = {}.hasOwnProperty;
 
@@ -47065,15 +47065,15 @@
                 e.resolveAll && !o.includes(e) && o.push(e), e.resolve && Object(ne.b)(c.events, t, c.events.length - t, e.resolve(c.events.slice(t), c)), e.resolveTo && (c.events = e.resolveTo(c.events, c))
             }
 
             function E() {
                 r.line in i && r.column < 2 && (r.column = i[r.line], r.offset += i[r.line] - 1)
             }
         }
-        var Ee = n(8),
+        var Ee = n(9),
             ye = {
                 name: "thematicBreak",
                 tokenize: function(e, t, n) {
                     var r, i = 0;
                     return function(t) {
                         return e.enter("thematicBreak"), r = t, o(t)
                     };
@@ -49412,15 +49412,15 @@
             components: Zt.a.object
         }
     }, function(e, t, n) {
         "use strict";
         var r = n(4),
             i = n(76),
             o = n(19),
-            a = n(24),
+            a = n(25),
             s = n(46);
 
         function u(e) {
             var t = {
                 "!": "%21",
                 "'": "%27",
                 "(": "%28",
@@ -49616,15 +49616,15 @@
         };
         r.a.forEach(["delete", "get", "head"], (function(e) {
             y.headers[e] = {}
         })), r.a.forEach(["post", "put", "patch"], (function(e) {
             y.headers[e] = r.a.merge(E)
         }));
         var _ = y,
-            T = n(9),
+            T = n(8),
             w = r.a.toObjectSet(["age", "authorization", "content-length", "content-type", "etag", "expires", "from", "host", "if-modified-since", "if-unmodified-since", "last-modified", "location", "max-forwards", "proxy-authorization", "referer", "retry-after", "user-agent"]),
             O = Symbol("internals");
 
         function A(e) {
             return e && String(e).trim().toLowerCase()
         }
 
@@ -50428,15 +50428,15 @@
             he = n.n(pe),
             me = n(166),
             ge = n.n(me),
             ve = n(167),
             be = n.n(ve),
             Ee = n(15),
             ye = n(19),
-            _e = n(24),
+            _e = n(25),
             Te = n(34),
             we = n.n(Te),
             Oe = n(168),
             Ae = n.n(Oe),
             ke = Object.assign(De(Error), {
                 eval: De(EvalError),
                 range: De(RangeError),
@@ -50788,8 +50788,8 @@
                     if ("no-highlight" === r || "nohighlight" === r) return !1;
                     if ("lang-" === r.slice(0, 5)) return r.slice(5);
                     if ("language-" === r.slice(0, 9)) return r.slice(9)
                 }
         }
     }]
 ]);
-//# sourceMappingURL=2.206848a5.chunk.js.map
+//# sourceMappingURL=2.20c8cb43.chunk.js.map
```

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/js/2.206848a5.chunk.js.LICENSE.txt` & `mercury-2.3.2/mercury/frontend-dist/static/js/2.20c8cb43.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/js/2.206848a5.chunk.js.map` & `mercury-2.3.2/mercury/frontend-dist/static/js/2.20c8cb43.chunk.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8566743004012467%*

 * *Differences: {"'file'": "'static/js/2.20c8cb43.chunk.js'",*

 * * "'mappings'": "';kGAGEA,EAAOC,QAAUC,EAAQ,M,6BCAzBF,EAAOC,QAAUC,EAAQ,M,6BCH3B,2UAAIC,EAAS,EAEAC,EAAUC,IACVC,EAAaD,IACbE,EAAoBF,IACpBG,EAASH,IACTI,EAAiBJ,IACjBK,EAAiBL,IACjBM,EAAwBN,IAErC,SAASA,IACP,gBAAO,IAAOF,K,qbCLT,ICWMS,EAAaC,EAAW,YAQxBC,EAAaD,EAAW,MAexBE,EAAgBF,EAAW,cAS3BG,EAAoBH,EAAW,cAU/BI,EAAmBJ,EAAW,kBAkB9BK,EAAaL,EAAW,uBAW9B,SAASM,EAAaC,GAC3B,OAGW,OAATA,IAAkBA,EAAO,IAAe,MAATA,GAW5B,SAASC,EAA0BD,GACxC,OAAgB,OAATA,IAAkBA,EAAO,GAAc,KAATA,GAgBhC,SAASE,EAAm […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/2.206848a5.chunk.js",
+    "file": "static/js/2.20c8cb43.chunk.js",
     "names": [
         "module",
         "exports",
         "require",
         "powers",
         "boolean",
         "increment",
@@ -674,26 +674,26 @@
         "unwrap",
         "URLSearchParams",
         "getAll",
         "some",
         "v",
         "handle",
         "pathMatches",
-        "_defineProperty",
-        "configurable",
         "_slicedToArray",
         "arrayWithHoles",
         "_arr",
         "_n",
         "_d",
         "_e",
         "_s",
         "_i",
         "unsupportedIterableToArray",
         "nonIterableRest",
+        "_defineProperty",
+        "configurable",
         "_extends",
         "apply",
         "is",
         "x",
         "checkIfSnapshotChanged",
         "inst",
         "latestGetSnapshot",
@@ -11493,17 +11493,17 @@
         "../node_modules/react-redux/es/hooks/useDispatch.js",
         "../node_modules/react-redux/es/hooks/useSelector.js",
         "../node_modules/react-redux/es/index.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/regenerator/index.js",
         "../../history.ts",
         "../../utils.ts",
         "../../router.ts",
-        "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/defineProperty.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/slicedToArray.js",
         "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/iterableToArrayLimit.js",
+        "../node_modules/babel-preset-react-app/node_modules/@babel/runtime/helpers/esm/defineProperty.js",
         "../node_modules/@babel/runtime/helpers/esm/extends.js",
         "../../lib/use-sync-external-store-shim/useSyncExternalStoreShimClient.ts",
         "../../lib/use-sync-external-store-shim/index.ts",
         "../../lib/use-sync-external-store-shim/useSyncExternalStoreShimServer.ts",
         "../../lib/context.ts",
         "../../lib/hooks.tsx",
         "../../lib/components.tsx",
@@ -12138,17 +12138,17 @@
         "import { ReactReduxContext } from '../components/Context';\nimport { useStore as useDefaultStore, createStoreHook } from './useStore';\n/**\n * Hook factory, which creates a `useDispatch` hook bound to a given context.\n *\n * @param {React.Context} [context=ReactReduxContext] Context passed to your `<Provider>`.\n * @returns {Function} A `useDispatch` hook bound to the specified context.\n */\n\nexport function createDispatchHook(context) {\n  if (context === void 0) {\n    context = ReactReduxContext;\n  }\n\n  var useStore = context === ReactReduxContext ? useDefaultStore : createStoreHook(context);\n  return function useDispatch() {\n    var store = useStore();\n    return store.dispatch;\n  };\n}\n/**\n * A hook to access the redux `dispatch` function.\n *\n * @returns {any|function} redux store's `dispatch` function\n *\n * @example\n *\n * import React, { useCallback } from 'react'\n * import { useDispatch } from 'react-redux'\n *\n * export const CounterComponent = ({ value }) => {\n *   const dispatch = useDispatch()\n *   const increaseCounter = useCallback(() => dispatch({ type: 'increase-counter' }), [])\n *   return (\n *     <div>\n *       <span>{value}</span>\n *       <button onClick={increaseCounter}>Increase counter</button>\n *     </div>\n *   )\n * }\n */\n\nexport var useDispatch = /*#__PURE__*/createDispatchHook();",
         "import { useReducer, useRef, useMemo, useContext, useDebugValue } from 'react';\nimport { useReduxContext as useDefaultReduxContext } from './useReduxContext';\nimport { createSubscription } from '../utils/Subscription';\nimport { useIsomorphicLayoutEffect } from '../utils/useIsomorphicLayoutEffect';\nimport { ReactReduxContext } from '../components/Context';\n\nvar refEquality = function refEquality(a, b) {\n  return a === b;\n};\n\nfunction useSelectorWithStoreAndSubscription(selector, equalityFn, store, contextSub) {\n  var _useReducer = useReducer(function (s) {\n    return s + 1;\n  }, 0),\n      forceRender = _useReducer[1];\n\n  var subscription = useMemo(function () {\n    return createSubscription(store, contextSub);\n  }, [store, contextSub]);\n  var latestSubscriptionCallbackError = useRef();\n  var latestSelector = useRef();\n  var latestStoreState = useRef();\n  var latestSelectedState = useRef();\n  var storeState = store.getState();\n  var selectedState;\n\n  try {\n    if (selector !== latestSelector.current || storeState !== latestStoreState.current || latestSubscriptionCallbackError.current) {\n      var newSelectedState = selector(storeState); // ensure latest selected state is reused so that a custom equality function can result in identical references\n\n      if (latestSelectedState.current === undefined || !equalityFn(newSelectedState, latestSelectedState.current)) {\n        selectedState = newSelectedState;\n      } else {\n        selectedState = latestSelectedState.current;\n      }\n    } else {\n      selectedState = latestSelectedState.current;\n    }\n  } catch (err) {\n    if (latestSubscriptionCallbackError.current) {\n      err.message += \"\\nThe error may be correlated with this previous error:\\n\" + latestSubscriptionCallbackError.current.stack + \"\\n\\n\";\n    }\n\n    throw err;\n  }\n\n  useIsomorphicLayoutEffect(function () {\n    latestSelector.current = selector;\n    latestStoreState.current = storeState;\n    latestSelectedState.current = selectedState;\n    latestSubscriptionCallbackError.current = undefined;\n  });\n  useIsomorphicLayoutEffect(function () {\n    function checkForUpdates() {\n      try {\n        var newStoreState = store.getState(); // Avoid calling selector multiple times if the store's state has not changed\n\n        if (newStoreState === latestStoreState.current) {\n          return;\n        }\n\n        var _newSelectedState = latestSelector.current(newStoreState);\n\n        if (equalityFn(_newSelectedState, latestSelectedState.current)) {\n          return;\n        }\n\n        latestSelectedState.current = _newSelectedState;\n        latestStoreState.current = newStoreState;\n      } catch (err) {\n        // we ignore all errors here, since when the component\n        // is re-rendered, the selectors are called again, and\n        // will throw again, if neither props nor store state\n        // changed\n        latestSubscriptionCallbackError.current = err;\n      }\n\n      forceRender();\n    }\n\n    subscription.onStateChange = checkForUpdates;\n    subscription.trySubscribe();\n    checkForUpdates();\n    return function () {\n      return subscription.tryUnsubscribe();\n    };\n  }, [store, subscription]);\n  return selectedState;\n}\n/**\n * Hook factory, which creates a `useSelector` hook bound to a given context.\n *\n * @param {React.Context} [context=ReactReduxContext] Context passed to your `<Provider>`.\n * @returns {Function} A `useSelector` hook bound to the specified context.\n */\n\n\nexport function createSelectorHook(context) {\n  if (context === void 0) {\n    context = ReactReduxContext;\n  }\n\n  var useReduxContext = context === ReactReduxContext ? useDefaultReduxContext : function () {\n    return useContext(context);\n  };\n  return function useSelector(selector, equalityFn) {\n    if (equalityFn === void 0) {\n      equalityFn = refEquality;\n    }\n\n    if (process.env.NODE_ENV !== 'production') {\n      if (!selector) {\n        throw new Error(\"You must pass a selector to useSelector\");\n      }\n\n      if (typeof selector !== 'function') {\n        throw new Error(\"You must pass a function as a selector to useSelector\");\n      }\n\n      if (typeof equalityFn !== 'function') {\n        throw new Error(\"You must pass a function as an equality function to useSelector\");\n      }\n    }\n\n    var _useReduxContext = useReduxContext(),\n        store = _useReduxContext.store,\n        contextSub = _useReduxContext.subscription;\n\n    var selectedState = useSelectorWithStoreAndSubscription(selector, equalityFn, store, contextSub);\n    useDebugValue(selectedState);\n    return selectedState;\n  };\n}\n/**\n * A hook to access the redux store's state. This hook takes a selector function\n * as an argument. The selector is called with the store state.\n *\n * This hook takes an optional equality comparison function as the second parameter\n * that allows you to customize the way the selected state is compared to determine\n * whether the component needs to be re-rendered.\n *\n * @param {Function} selector the selector function\n * @param {Function=} equalityFn the function that will be used to determine equality\n *\n * @returns {any} the selected state\n *\n * @example\n *\n * import React from 'react'\n * import { useSelector } from 'react-redux'\n *\n * export const CounterComponent = () => {\n *   const counter = useSelector(state => state.counter)\n *   return <div>{counter}</div>\n * }\n */\n\nexport var useSelector = /*#__PURE__*/createSelectorHook();",
         "export * from './exports';\nimport { unstable_batchedUpdates as batch } from './utils/reactBatchedUpdates';\nimport { setBatch } from './utils/batch'; // Enable batched updates in our subscriptions for use\n// with standard React renderers (ReactDOM, React Native)\n\nsetBatch(batch);\nexport { batch };",
         "module.exports = require(\"regenerator-runtime\");\n",
         "////////////////////////////////////////////////////////////////////////////////\n//#region Types and Constants\n////////////////////////////////////////////////////////////////////////////////\n\n/**\n * Actions represent the type of change to a location value.\n */\nexport enum Action {\n  /**\n   * A POP indicates a change to an arbitrary index in the history stack, such\n   * as a back or forward navigation. It does not describe the direction of the\n   * navigation, only that the current index changed.\n   *\n   * Note: This is the default action for newly created history objects.\n   */\n  Pop = \"POP\",\n\n  /**\n   * A PUSH indicates a new entry being added to the history stack, such as when\n   * a link is clicked and a new page loads. When this happens, all subsequent\n   * entries in the stack are lost.\n   */\n  Push = \"PUSH\",\n\n  /**\n   * A REPLACE indicates the entry at the current index in the history stack\n   * being replaced by a new one.\n   */\n  Replace = \"REPLACE\",\n}\n\n/**\n * The pathname, search, and hash values of a URL.\n */\nexport interface Path {\n  /**\n   * A URL pathname, beginning with a /.\n   */\n  pathname: string;\n\n  /**\n   * A URL search string, beginning with a ?.\n   */\n  search: string;\n\n  /**\n   * A URL fragment identifier, beginning with a #.\n   */\n  hash: string;\n}\n\n/**\n * An entry in a history stack. A location contains information about the\n * URL path, as well as possibly some arbitrary state and a key.\n */\nexport interface Location extends Path {\n  /**\n   * A value of arbitrary data associated with this location.\n   */\n  state: any;\n\n  /**\n   * A unique string associated with this location. May be used to safely store\n   * and retrieve data in some other storage API, like `localStorage`.\n   *\n   * Note: This value is always \"default\" on the initial location.\n   */\n  key: string;\n}\n\n/**\n * A change to the current location.\n */\nexport interface Update {\n  /**\n   * The action that triggered the change.\n   */\n  action: Action;\n\n  /**\n   * The new location.\n   */\n  location: Location;\n\n  /**\n   * The delta between this location and the former location in the history stack\n   */\n  delta: number | null;\n}\n\n/**\n * A function that receives notifications about location changes.\n */\nexport interface Listener {\n  (update: Update): void;\n}\n\n/**\n * Describes a location that is the destination of some navigation, either via\n * `history.push` or `history.replace`. May be either a URL or the pieces of a\n * URL path.\n */\nexport type To = string | Partial<Path>;\n\n/**\n * A history is an interface to the navigation stack. The history serves as the\n * source of truth for the current location, as well as provides a set of\n * methods that may be used to change it.\n *\n * It is similar to the DOM's `window.history` object, but with a smaller, more\n * focused API.\n */\nexport interface History {\n  /**\n   * The last action that modified the current location. This will always be\n   * Action.Pop when a history instance is first created. This value is mutable.\n   */\n  readonly action: Action;\n\n  /**\n   * The current location. This value is mutable.\n   */\n  readonly location: Location;\n\n  /**\n   * Returns a valid href for the given `to` value that may be used as\n   * the value of an <a href> attribute.\n   *\n   * @param to - The destination URL\n   */\n  createHref(to: To): string;\n\n  /**\n   * Returns a URL for the given `to` value\n   *\n   * @param to - The destination URL\n   */\n  createURL(to: To): URL;\n\n  /**\n   * Encode a location the same way window.history would do (no-op for memory\n   * history) so we ensure our PUSH/REPLACE navigations for data routers\n   * behave the same as POP\n   *\n   * @param to Unencoded path\n   */\n  encodeLocation(to: To): Path;\n\n  /**\n   * Pushes a new location onto the history stack, increasing its length by one.\n   * If there were any entries in the stack after the current one, they are\n   * lost.\n   *\n   * @param to - The new URL\n   * @param state - Data to associate with the new location\n   */\n  push(to: To, state?: any): void;\n\n  /**\n   * Replaces the current location in the history stack with a new one.  The\n   * location that was replaced will no longer be available.\n   *\n   * @param to - The new URL\n   * @param state - Data to associate with the new location\n   */\n  replace(to: To, state?: any): void;\n\n  /**\n   * Navigates `n` entries backward/forward in the history stack relative to the\n   * current index. For example, a \"back\" navigation would use go(-1).\n   *\n   * @param delta - The delta in the stack index\n   */\n  go(delta: number): void;\n\n  /**\n   * Sets up a listener that will be called whenever the current location\n   * changes.\n   *\n   * @param listener - A function that will be called when the location changes\n   * @returns unlisten - A function that may be used to stop listening\n   */\n  listen(listener: Listener): () => void;\n}\n\ntype HistoryState = {\n  usr: any;\n  key?: string;\n  idx: number;\n};\n\nconst PopStateEventType = \"popstate\";\n//#endregion\n\n////////////////////////////////////////////////////////////////////////////////\n//#region Memory History\n////////////////////////////////////////////////////////////////////////////////\n\n/**\n * A user-supplied object that describes a location. Used when providing\n * entries to `createMemoryHistory` via its `initialEntries` option.\n */\nexport type InitialEntry = string | Partial<Location>;\n\nexport type MemoryHistoryOptions = {\n  initialEntries?: InitialEntry[];\n  initialIndex?: number;\n  v5Compat?: boolean;\n};\n\n/**\n * A memory history stores locations in memory. This is useful in stateful\n * environments where there is no web browser, such as node tests or React\n * Native.\n */\nexport interface MemoryHistory extends History {\n  /**\n   * The current index in the history stack.\n   */\n  readonly index: number;\n}\n\n/**\n * Memory history stores the current location in memory. It is designed for use\n * in stateful non-browser environments like tests and React Native.\n */\nexport function createMemoryHistory(\n  options: MemoryHistoryOptions = {}\n): MemoryHistory {\n  let { initialEntries = [\"/\"], initialIndex, v5Compat = false } = options;\n  let entries: Location[]; // Declare so we can access from createMemoryLocation\n  entries = initialEntries.map((entry, index) =>\n    createMemoryLocation(\n      entry,\n      typeof entry === \"string\" ? null : entry.state,\n      index === 0 ? \"default\" : undefined\n    )\n  );\n  let index = clampIndex(\n    initialIndex == null ? entries.length - 1 : initialIndex\n  );\n  let action = Action.Pop;\n  let listener: Listener | null = null;\n\n  function clampIndex(n: number): number {\n    return Math.min(Math.max(n, 0), entries.length - 1);\n  }\n  function getCurrentLocation(): Location {\n    return entries[index];\n  }\n  function createMemoryLocation(\n    to: To,\n    state: any = null,\n    key?: string\n  ): Location {\n    let location = createLocation(\n      entries ? getCurrentLocation().pathname : \"/\",\n      to,\n      state,\n      key\n    );\n    warning(\n      location.pathname.charAt(0) === \"/\",\n      `relative pathnames are not supported in memory history: ${JSON.stringify(\n        to\n      )}`\n    );\n    return location;\n  }\n\n  function createHref(to: To) {\n    return typeof to === \"string\" ? to : createPath(to);\n  }\n\n  let history: MemoryHistory = {\n    get index() {\n      return index;\n    },\n    get action() {\n      return action;\n    },\n    get location() {\n      return getCurrentLocation();\n    },\n    createHref,\n    createURL(to) {\n      return new URL(createHref(to), \"http://localhost\");\n    },\n    encodeLocation(to: To) {\n      let path = typeof to === \"string\" ? parsePath(to) : to;\n      return {\n        pathname: path.pathname || \"\",\n        search: path.search || \"\",\n        hash: path.hash || \"\",\n      };\n    },\n    push(to, state) {\n      action = Action.Push;\n      let nextLocation = createMemoryLocation(to, state);\n      index += 1;\n      entries.splice(index, entries.length, nextLocation);\n      if (v5Compat && listener) {\n        listener({ action, location: nextLocation, delta: 1 });\n      }\n    },\n    replace(to, state) {\n      action = Action.Replace;\n      let nextLocation = createMemoryLocation(to, state);\n      entries[index] = nextLocation;\n      if (v5Compat && listener) {\n        listener({ action, location: nextLocation, delta: 0 });\n      }\n    },\n    go(delta) {\n      action = Action.Pop;\n      let nextIndex = clampIndex(index + delta);\n      let nextLocation = entries[nextIndex];\n      index = nextIndex;\n      if (listener) {\n        listener({ action, location: nextLocation, delta });\n      }\n    },\n    listen(fn: Listener) {\n      listener = fn;\n      return () => {\n        listener = null;\n      };\n    },\n  };\n\n  return history;\n}\n//#endregion\n\n////////////////////////////////////////////////////////////////////////////////\n//#region Browser History\n////////////////////////////////////////////////////////////////////////////////\n\n/**\n * A browser history stores the current location in regular URLs in a web\n * browser environment. This is the standard for most web apps and provides the\n * cleanest URLs the browser's address bar.\n *\n * @see https://github.com/remix-run/history/tree/main/docs/api-reference.md#browserhistory\n */\nexport interface BrowserHistory extends UrlHistory {}\n\nexport type BrowserHistoryOptions = UrlHistoryOptions;\n\n/**\n * Browser history stores the location in regular URLs. This is the standard for\n * most web apps, but it requires some configuration on the server to ensure you\n * serve the same app at multiple URLs.\n *\n * @see https://github.com/remix-run/history/tree/main/docs/api-reference.md#createbrowserhistory\n */\nexport function createBrowserHistory(\n  options: BrowserHistoryOptions = {}\n): BrowserHistory {\n  function createBrowserLocation(\n    window: Window,\n    globalHistory: Window[\"history\"]\n  ) {\n    let { pathname, search, hash } = window.location;\n    return createLocation(\n      \"\",\n      { pathname, search, hash },\n      // state defaults to `null` because `window.history.state` does\n      (globalHistory.state && globalHistory.state.usr) || null,\n      (globalHistory.state && globalHistory.state.key) || \"default\"\n    );\n  }\n\n  function createBrowserHref(window: Window, to: To) {\n    return typeof to === \"string\" ? to : createPath(to);\n  }\n\n  return getUrlBasedHistory(\n    createBrowserLocation,\n    createBrowserHref,\n    null,\n    options\n  );\n}\n//#endregion\n\n////////////////////////////////////////////////////////////////////////////////\n//#region Hash History\n////////////////////////////////////////////////////////////////////////////////\n\n/**\n * A hash history stores the current location in the fragment identifier portion\n * of the URL in a web browser environment.\n *\n * This is ideal for apps that do not control the server for some reason\n * (because the fragment identifier is never sent to the server), including some\n * shared hosting environments that do not provide fine-grained controls over\n * which pages are served at which URLs.\n *\n * @see https://github.com/remix-run/history/tree/main/docs/api-reference.md#hashhistory\n */\nexport interface HashHistory extends UrlHistory {}\n\nexport type HashHistoryOptions = UrlHistoryOptions;\n\n/**\n * Hash history stores the location in window.location.hash. This makes it ideal\n * for situations where you don't want to send the location to the server for\n * some reason, either because you do cannot configure it or the URL space is\n * reserved for something else.\n *\n * @see https://github.com/remix-run/history/tree/main/docs/api-reference.md#createhashhistory\n */\nexport function createHashHistory(\n  options: HashHistoryOptions = {}\n): HashHistory {\n  function createHashLocation(\n    window: Window,\n    globalHistory: Window[\"history\"]\n  ) {\n    let {\n      pathname = \"/\",\n      search = \"\",\n      hash = \"\",\n    } = parsePath(window.location.hash.substr(1));\n    return createLocation(\n      \"\",\n      { pathname, search, hash },\n      // state defaults to `null` because `window.history.state` does\n      (globalHistory.state && globalHistory.state.usr) || null,\n      (globalHistory.state && globalHistory.state.key) || \"default\"\n    );\n  }\n\n  function createHashHref(window: Window, to: To) {\n    let base = window.document.querySelector(\"base\");\n    let href = \"\";\n\n    if (base && base.getAttribute(\"href\")) {\n      let url = window.location.href;\n      let hashIndex = url.indexOf(\"#\");\n      href = hashIndex === -1 ? url : url.slice(0, hashIndex);\n    }\n\n    return href + \"#\" + (typeof to === \"string\" ? to : createPath(to));\n  }\n\n  function validateHashLocation(location: Location, to: To) {\n    warning(\n      location.pathname.charAt(0) === \"/\",\n      `relative pathnames are not supported in hash history.push(${JSON.stringify(\n        to\n      )})`\n    );\n  }\n\n  return getUrlBasedHistory(\n    createHashLocation,\n    createHashHref,\n    validateHashLocation,\n    options\n  );\n}\n//#endregion\n\n////////////////////////////////////////////////////////////////////////////////\n//#region UTILS\n////////////////////////////////////////////////////////////////////////////////\n\n/**\n * @private\n */\nexport function invariant(value: boolean, message?: string): asserts value;\nexport function invariant<T>(\n  value: T | null | undefined,\n  message?: string\n): asserts value is T;\nexport function invariant(value: any, message?: string) {\n  if (value === false || value === null || typeof value === \"undefined\") {\n    throw new Error(message);\n  }\n}\n\nfunction warning(cond: any, message: string) {\n  if (!cond) {\n    // eslint-disable-next-line no-console\n    if (typeof console !== \"undefined\") console.warn(message);\n\n    try {\n      // Welcome to debugging history!\n      //\n      // This error is thrown as a convenience so you can more easily\n      // find the source for a warning that appears in the console by\n      // enabling \"pause on exceptions\" in your JavaScript debugger.\n      throw new Error(message);\n      // eslint-disable-next-line no-empty\n    } catch (e) {}\n  }\n}\n\nfunction createKey() {\n  return Math.random().toString(36).substr(2, 8);\n}\n\n/**\n * For browser-based histories, we combine the state and key into an object\n */\nfunction getHistoryState(location: Location, index: number): HistoryState {\n  return {\n    usr: location.state,\n    key: location.key,\n    idx: index,\n  };\n}\n\n/**\n * Creates a Location object with a unique key from the given Path\n */\nexport function createLocation(\n  current: string | Location,\n  to: To,\n  state: any = null,\n  key?: string\n): Readonly<Location> {\n  let location: Readonly<Location> = {\n    pathname: typeof current === \"string\" ? current : current.pathname,\n    search: \"\",\n    hash: \"\",\n    ...(typeof to === \"string\" ? parsePath(to) : to),\n    state,\n    // TODO: This could be cleaned up.  push/replace should probably just take\n    // full Locations now and avoid the need to run through this flow at all\n    // But that's a pretty big refactor to the current test suite so going to\n    // keep as is for the time being and just let any incoming keys take precedence\n    key: (to && (to as Location).key) || key || createKey(),\n  };\n  return location;\n}\n\n/**\n * Creates a string URL path from the given pathname, search, and hash components.\n */\nexport function createPath({\n  pathname = \"/\",\n  search = \"\",\n  hash = \"\",\n}: Partial<Path>) {\n  if (search && search !== \"?\")\n    pathname += search.charAt(0) === \"?\" ? search : \"?\" + search;\n  if (hash && hash !== \"#\")\n    pathname += hash.charAt(0) === \"#\" ? hash : \"#\" + hash;\n  return pathname;\n}\n\n/**\n * Parses a string URL path into its separate pathname, search, and hash components.\n */\nexport function parsePath(path: string): Partial<Path> {\n  let parsedPath: Partial<Path> = {};\n\n  if (path) {\n    let hashIndex = path.indexOf(\"#\");\n    if (hashIndex >= 0) {\n      parsedPath.hash = path.substr(hashIndex);\n      path = path.substr(0, hashIndex);\n    }\n\n    let searchIndex = path.indexOf(\"?\");\n    if (searchIndex >= 0) {\n      parsedPath.search = path.substr(searchIndex);\n      path = path.substr(0, searchIndex);\n    }\n\n    if (path) {\n      parsedPath.pathname = path;\n    }\n  }\n\n  return parsedPath;\n}\n\nexport interface UrlHistory extends History {}\n\nexport type UrlHistoryOptions = {\n  window?: Window;\n  v5Compat?: boolean;\n};\n\nfunction getUrlBasedHistory(\n  getLocation: (window: Window, globalHistory: Window[\"history\"]) => Location,\n  createHref: (window: Window, to: To) => string,\n  validateLocation: ((location: Location, to: To) => void) | null,\n  options: UrlHistoryOptions = {}\n): UrlHistory {\n  let { window = document.defaultView!, v5Compat = false } = options;\n  let globalHistory = window.history;\n  let action = Action.Pop;\n  let listener: Listener | null = null;\n\n  let index = getIndex()!;\n  // Index should only be null when we initialize. If not, it's because the\n  // user called history.pushState or history.replaceState directly, in which\n  // case we should log a warning as it will result in bugs.\n  if (index == null) {\n    index = 0;\n    globalHistory.replaceState({ ...globalHistory.state, idx: index }, \"\");\n  }\n\n  function getIndex(): number {\n    let state = globalHistory.state || { idx: null };\n    return state.idx;\n  }\n\n  function handlePop() {\n    action = Action.Pop;\n    let nextIndex = getIndex();\n    let delta = nextIndex == null ? null : nextIndex - index;\n    index = nextIndex;\n    if (listener) {\n      listener({ action, location: history.location, delta });\n    }\n  }\n\n  function push(to: To, state?: any) {\n    action = Action.Push;\n    let location = createLocation(history.location, to, state);\n    if (validateLocation) validateLocation(location, to);\n\n    index = getIndex() + 1;\n    let historyState = getHistoryState(location, index);\n    let url = history.createHref(location);\n\n    // try...catch because iOS limits us to 100 pushState calls :/\n    try {\n      globalHistory.pushState(historyState, \"\", url);\n    } catch (error) {\n      // They are going to lose state here, but there is no real\n      // way to warn them about it since the page will refresh...\n      window.location.assign(url);\n    }\n\n    if (v5Compat && listener) {\n      listener({ action, location: history.location, delta: 1 });\n    }\n  }\n\n  function replace(to: To, state?: any) {\n    action = Action.Replace;\n    let location = createLocation(history.location, to, state);\n    if (validateLocation) validateLocation(location, to);\n\n    index = getIndex();\n    let historyState = getHistoryState(location, index);\n    let url = history.createHref(location);\n    globalHistory.replaceState(historyState, \"\", url);\n\n    if (v5Compat && listener) {\n      listener({ action, location: history.location, delta: 0 });\n    }\n  }\n\n  function createURL(to: To): URL {\n    // window.location.origin is \"null\" (the literal string value) in Firefox\n    // under certain conditions, notably when serving from a local HTML file\n    // See https://bugzilla.mozilla.org/show_bug.cgi?id=878297\n    let base =\n      window.location.origin !== \"null\"\n        ? window.location.origin\n        : window.location.href;\n\n    let href = typeof to === \"string\" ? to : createPath(to);\n    invariant(\n      base,\n      `No window.location.(origin|href) available to create URL for href: ${href}`\n    );\n    return new URL(href, base);\n  }\n\n  let history: History = {\n    get action() {\n      return action;\n    },\n    get location() {\n      return getLocation(window, globalHistory);\n    },\n    listen(fn: Listener) {\n      if (listener) {\n        throw new Error(\"A history only accepts one active listener\");\n      }\n      window.addEventListener(PopStateEventType, handlePop);\n      listener = fn;\n\n      return () => {\n        window.removeEventListener(PopStateEventType, handlePop);\n        listener = null;\n      };\n    },\n    createHref(to) {\n      return createHref(window, to);\n    },\n    createURL,\n    encodeLocation(to) {\n      // Encode a Location the same way window.location would\n      let url = createURL(to);\n      return {\n        pathname: url.pathname,\n        search: url.search,\n        hash: url.hash,\n      };\n    },\n    push,\n    replace,\n    go(n) {\n      return globalHistory.go(n);\n    },\n  };\n\n  return history;\n}\n\n//#endregion\n",
         "import type { Location, Path, To } from \"./history\";\nimport { invariant, parsePath } from \"./history\";\n\n/**\n * Map of routeId -> data returned from a loader/action/error\n */\nexport interface RouteData {\n  [routeId: string]: any;\n}\n\nexport enum ResultType {\n  data = \"data\",\n  deferred = \"deferred\",\n  redirect = \"redirect\",\n  error = \"error\",\n}\n\n/**\n * Successful result from a loader or action\n */\nexport interface SuccessResult {\n  type: ResultType.data;\n  data: any;\n  statusCode?: number;\n  headers?: Headers;\n}\n\n/**\n * Successful defer() result from a loader or action\n */\nexport interface DeferredResult {\n  type: ResultType.deferred;\n  deferredData: DeferredData;\n  statusCode?: number;\n  headers?: Headers;\n}\n\n/**\n * Redirect result from a loader or action\n */\nexport interface RedirectResult {\n  type: ResultType.redirect;\n  status: number;\n  location: string;\n  revalidate: boolean;\n}\n\n/**\n * Unsuccessful result from a loader or action\n */\nexport interface ErrorResult {\n  type: ResultType.error;\n  error: any;\n  headers?: Headers;\n}\n\n/**\n * Result from a loader or action - potentially successful or unsuccessful\n */\nexport type DataResult =\n  | SuccessResult\n  | DeferredResult\n  | RedirectResult\n  | ErrorResult;\n\nexport type MutationFormMethod = \"post\" | \"put\" | \"patch\" | \"delete\";\nexport type FormMethod = \"get\" | MutationFormMethod;\n\nexport type FormEncType =\n  | \"application/x-www-form-urlencoded\"\n  | \"multipart/form-data\";\n\n/**\n * @private\n * Internal interface to pass around for action submissions, not intended for\n * external consumption\n */\nexport interface Submission {\n  formMethod: FormMethod;\n  formAction: string;\n  formEncType: FormEncType;\n  formData: FormData;\n}\n\n/**\n * @private\n * Arguments passed to route loader/action functions.  Same for now but we keep\n * this as a private implementation detail in case they diverge in the future.\n */\ninterface DataFunctionArgs {\n  request: Request;\n  params: Params;\n  context?: any;\n}\n\n/**\n * Arguments passed to loader functions\n */\nexport interface LoaderFunctionArgs extends DataFunctionArgs {}\n\n/**\n * Arguments passed to action functions\n */\nexport interface ActionFunctionArgs extends DataFunctionArgs {}\n\n/**\n * Route loader function signature\n */\nexport interface LoaderFunction {\n  (args: LoaderFunctionArgs): Promise<Response> | Response | Promise<any> | any;\n}\n\n/**\n * Route action function signature\n */\nexport interface ActionFunction {\n  (args: ActionFunctionArgs): Promise<Response> | Response | Promise<any> | any;\n}\n\n/**\n * Route shouldRevalidate function signature.  This runs after any submission\n * (navigation or fetcher), so we flatten the navigation/fetcher submission\n * onto the arguments.  It shouldn't matter whether it came from a navigation\n * or a fetcher, what really matters is the URLs and the formData since loaders\n * have to re-run based on the data models that were potentially mutated.\n */\nexport interface ShouldRevalidateFunction {\n  (args: {\n    currentUrl: URL;\n    currentParams: AgnosticDataRouteMatch[\"params\"];\n    nextUrl: URL;\n    nextParams: AgnosticDataRouteMatch[\"params\"];\n    formMethod?: Submission[\"formMethod\"];\n    formAction?: Submission[\"formAction\"];\n    formEncType?: Submission[\"formEncType\"];\n    formData?: Submission[\"formData\"];\n    actionResult?: DataResult;\n    defaultShouldRevalidate: boolean;\n  }): boolean;\n}\n\n/**\n * Base RouteObject with common props shared by all types of routes\n */\ntype AgnosticBaseRouteObject = {\n  caseSensitive?: boolean;\n  path?: string;\n  id?: string;\n  loader?: LoaderFunction;\n  action?: ActionFunction;\n  hasErrorBoundary?: boolean;\n  shouldRevalidate?: ShouldRevalidateFunction;\n  handle?: any;\n};\n\n/**\n * Index routes must not have children\n */\nexport type AgnosticIndexRouteObject = AgnosticBaseRouteObject & {\n  children?: undefined;\n  index: true;\n};\n\n/**\n * Non-index routes may have children, but cannot have index\n */\nexport type AgnosticNonIndexRouteObject = AgnosticBaseRouteObject & {\n  children?: AgnosticRouteObject[];\n  index?: false;\n};\n\n/**\n * A route object represents a logical route, with (optionally) its child\n * routes organized in a tree-like structure.\n */\nexport type AgnosticRouteObject =\n  | AgnosticIndexRouteObject\n  | AgnosticNonIndexRouteObject;\n\nexport type AgnosticDataIndexRouteObject = AgnosticIndexRouteObject & {\n  id: string;\n};\n\nexport type AgnosticDataNonIndexRouteObject = AgnosticNonIndexRouteObject & {\n  children?: AgnosticDataRouteObject[];\n  id: string;\n};\n\n/**\n * A data route object, which is just a RouteObject with a required unique ID\n */\nexport type AgnosticDataRouteObject =\n  | AgnosticDataIndexRouteObject\n  | AgnosticDataNonIndexRouteObject;\n\n// Recursive helper for finding path parameters in the absence of wildcards\ntype _PathParam<Path extends string> =\n  // split path into individual path segments\n  Path extends `${infer L}/${infer R}`\n    ? _PathParam<L> | _PathParam<R>\n    : // find params after `:`\n    Path extends `:${infer Param}`\n    ? Param extends `${infer Optional}?`\n      ? Optional\n      : Param\n    : // otherwise, there aren't any params present\n      never;\n\n/**\n * Examples:\n * \"/a/b/*\" -> \"*\"\n * \":a\" -> \"a\"\n * \"/a/:b\" -> \"b\"\n * \"/a/blahblahblah:b\" -> \"b\"\n * \"/:a/:b\" -> \"a\" | \"b\"\n * \"/:a/b/:c/*\" -> \"a\" | \"c\" | \"*\"\n */\ntype PathParam<Path extends string> =\n  // check if path is just a wildcard\n  Path extends \"*\"\n    ? \"*\"\n    : // look for wildcard at the end of the path\n    Path extends `${infer Rest}/*`\n    ? \"*\" | _PathParam<Rest>\n    : // look for params in the absence of wildcards\n      _PathParam<Path>;\n\n// Attempt to parse the given string segment. If it fails, then just return the\n// plain string type as a default fallback. Otherwise return the union of the\n// parsed string literals that were referenced as dynamic segments in the route.\nexport type ParamParseKey<Segment extends string> =\n  // if could not find path params, fallback to `string`\n  [PathParam<Segment>] extends [never] ? string : PathParam<Segment>;\n\n/**\n * The parameters that were parsed from the URL path.\n */\nexport type Params<Key extends string = string> = {\n  readonly [key in Key]: string | undefined;\n};\n\n/**\n * A RouteMatch contains info about how a route matched a URL.\n */\nexport interface AgnosticRouteMatch<\n  ParamKey extends string = string,\n  RouteObjectType extends AgnosticRouteObject = AgnosticRouteObject\n> {\n  /**\n   * The names and values of dynamic parameters in the URL.\n   */\n  params: Params<ParamKey>;\n  /**\n   * The portion of the URL pathname that was matched.\n   */\n  pathname: string;\n  /**\n   * The portion of the URL pathname that was matched before child routes.\n   */\n  pathnameBase: string;\n  /**\n   * The route object that was used to match.\n   */\n  route: RouteObjectType;\n}\n\nexport interface AgnosticDataRouteMatch\n  extends AgnosticRouteMatch<string, AgnosticDataRouteObject> {}\n\nfunction isIndexRoute(\n  route: AgnosticRouteObject\n): route is AgnosticIndexRouteObject {\n  return route.index === true;\n}\n\n// Walk the route tree generating unique IDs where necessary so we are working\n// solely with AgnosticDataRouteObject's within the Router\nexport function convertRoutesToDataRoutes(\n  routes: AgnosticRouteObject[],\n  parentPath: number[] = [],\n  allIds: Set<string> = new Set<string>()\n): AgnosticDataRouteObject[] {\n  return routes.map((route, index) => {\n    let treePath = [...parentPath, index];\n    let id = typeof route.id === \"string\" ? route.id : treePath.join(\"-\");\n    invariant(\n      route.index !== true || !route.children,\n      `Cannot specify children on an index route`\n    );\n    invariant(\n      !allIds.has(id),\n      `Found a route id collision on id \"${id}\".  Route ` +\n        \"id's must be globally unique within Data Router usages\"\n    );\n    allIds.add(id);\n\n    if (isIndexRoute(route)) {\n      let indexRoute: AgnosticDataIndexRouteObject = { ...route, id };\n      return indexRoute;\n    } else {\n      let pathOrLayoutRoute: AgnosticDataNonIndexRouteObject = {\n        ...route,\n        id,\n        children: route.children\n          ? convertRoutesToDataRoutes(route.children, treePath, allIds)\n          : undefined,\n      };\n      return pathOrLayoutRoute;\n    }\n  });\n}\n\n/**\n * Matches the given routes to a location and returns the match data.\n *\n * @see https://reactrouter.com/utils/match-routes\n */\nexport function matchRoutes<\n  RouteObjectType extends AgnosticRouteObject = AgnosticRouteObject\n>(\n  routes: RouteObjectType[],\n  locationArg: Partial<Location> | string,\n  basename = \"/\"\n): AgnosticRouteMatch<string, RouteObjectType>[] | null {\n  let location =\n    typeof locationArg === \"string\" ? parsePath(locationArg) : locationArg;\n\n  let pathname = stripBasename(location.pathname || \"/\", basename);\n\n  if (pathname == null) {\n    return null;\n  }\n\n  let branches = flattenRoutes(routes);\n  rankRouteBranches(branches);\n\n  let matches = null;\n  for (let i = 0; matches == null && i < branches.length; ++i) {\n    matches = matchRouteBranch<string, RouteObjectType>(\n      branches[i],\n      // Incoming pathnames are generally encoded from either window.location\n      // or from router.navigate, but we want to match against the unencoded\n      // paths in the route definitions.  Memory router locations won't be\n      // encoded here but there also shouldn't be anything to decode so this\n      // should be a safe operation.  This avoids needing matchRoutes to be\n      // history-aware.\n      safelyDecodeURI(pathname)\n    );\n  }\n\n  return matches;\n}\n\ninterface RouteMeta<\n  RouteObjectType extends AgnosticRouteObject = AgnosticRouteObject\n> {\n  relativePath: string;\n  caseSensitive: boolean;\n  childrenIndex: number;\n  route: RouteObjectType;\n}\n\ninterface RouteBranch<\n  RouteObjectType extends AgnosticRouteObject = AgnosticRouteObject\n> {\n  path: string;\n  score: number;\n  routesMeta: RouteMeta<RouteObjectType>[];\n}\n\nfunction flattenRoutes<\n  RouteObjectType extends AgnosticRouteObject = AgnosticRouteObject\n>(\n  routes: RouteObjectType[],\n  branches: RouteBranch<RouteObjectType>[] = [],\n  parentsMeta: RouteMeta<RouteObjectType>[] = [],\n  parentPath = \"\"\n): RouteBranch<RouteObjectType>[] {\n  let flattenRoute = (\n    route: RouteObjectType,\n    index: number,\n    relativePath?: string\n  ) => {\n    let meta: RouteMeta<RouteObjectType> = {\n      relativePath:\n        relativePath === undefined ? route.path || \"\" : relativePath,\n      caseSensitive: route.caseSensitive === true,\n      childrenIndex: index,\n      route,\n    };\n\n    if (meta.relativePath.startsWith(\"/\")) {\n      invariant(\n        meta.relativePath.startsWith(parentPath),\n        `Absolute route path \"${meta.relativePath}\" nested under path ` +\n          `\"${parentPath}\" is not valid. An absolute child route path ` +\n          `must start with the combined path of all its parent routes.`\n      );\n\n      meta.relativePath = meta.relativePath.slice(parentPath.length);\n    }\n\n    let path = joinPaths([parentPath, meta.relativePath]);\n    let routesMeta = parentsMeta.concat(meta);\n\n    // Add the children before adding this route to the array so we traverse the\n    // route tree depth-first and child routes appear before their parents in\n    // the \"flattened\" version.\n    if (route.children && route.children.length > 0) {\n      invariant(\n        // Our types know better, but runtime JS may not!\n        // @ts-expect-error\n        route.index !== true,\n        `Index routes must not have child routes. Please remove ` +\n          `all child routes from route path \"${path}\".`\n      );\n\n      flattenRoutes(route.children, branches, routesMeta, path);\n    }\n\n    // Routes without a path shouldn't ever match by themselves unless they are\n    // index routes, so don't add them to the list of possible branches.\n    if (route.path == null && !route.index) {\n      return;\n    }\n\n    branches.push({\n      path,\n      score: computeScore(path, route.index),\n      routesMeta,\n    });\n  };\n  routes.forEach((route, index) => {\n    // coarse-grain check for optional params\n    if (route.path === \"\" || !route.path?.includes(\"?\")) {\n      flattenRoute(route, index);\n    } else {\n      for (let exploded of explodeOptionalSegments(route.path)) {\n        flattenRoute(route, index, exploded);\n      }\n    }\n  });\n\n  return branches;\n}\n\n/**\n * Computes all combinations of optional path segments for a given path,\n * excluding combinations that are ambiguous and of lower priority.\n *\n * For example, `/one/:two?/three/:four?/:five?` explodes to:\n * - `/one/three`\n * - `/one/:two/three`\n * - `/one/three/:four`\n * - `/one/three/:five`\n * - `/one/:two/three/:four`\n * - `/one/:two/three/:five`\n * - `/one/three/:four/:five`\n * - `/one/:two/three/:four/:five`\n */\nfunction explodeOptionalSegments(path: string): string[] {\n  let segments = path.split(\"/\");\n  if (segments.length === 0) return [];\n\n  let [first, ...rest] = segments;\n\n  // Optional path segments are denoted by a trailing `?`\n  let isOptional = first.endsWith(\"?\");\n  // Compute the corresponding required segment: `foo?` -> `foo`\n  let required = first.replace(/\\?$/, \"\");\n\n  if (rest.length === 0) {\n    // Intepret empty string as omitting an optional segment\n    // `[\"one\", \"\", \"three\"]` corresponds to omitting `:two` from `/one/:two?/three` -> `/one/three`\n    return isOptional ? [required, \"\"] : [required];\n  }\n\n  let restExploded = explodeOptionalSegments(rest.join(\"/\"));\n\n  let result: string[] = [];\n\n  // All child paths with the prefix.  Do this for all children before the\n  // optional version for all children so we get consistent ordering where the\n  // parent optional aspect is preferred as required.  Otherwise, we can get\n  // child sections interspersed where deeper optional segments are higher than\n  // parent optional segments, where for example, /:two would explodes _earlier_\n  // then /:one.  By always including the parent as required _for all children_\n  // first, we avoid this issue\n  result.push(\n    ...restExploded.map((subpath) =>\n      subpath === \"\" ? required : [required, subpath].join(\"/\")\n    )\n  );\n\n  // Then if this is an optional value, add all child versions without\n  if (isOptional) {\n    result.push(...restExploded);\n  }\n\n  // for absolute paths, ensure `/` instead of empty segment\n  return result.map((exploded) =>\n    path.startsWith(\"/\") && exploded === \"\" ? \"/\" : exploded\n  );\n}\n\nfunction rankRouteBranches(branches: RouteBranch[]): void {\n  branches.sort((a, b) =>\n    a.score !== b.score\n      ? b.score - a.score // Higher score first\n      : compareIndexes(\n          a.routesMeta.map((meta) => meta.childrenIndex),\n          b.routesMeta.map((meta) => meta.childrenIndex)\n        )\n  );\n}\n\nconst paramRe = /^:\\w+$/;\nconst dynamicSegmentValue = 3;\nconst indexRouteValue = 2;\nconst emptySegmentValue = 1;\nconst staticSegmentValue = 10;\nconst splatPenalty = -2;\nconst isSplat = (s: string) => s === \"*\";\n\nfunction computeScore(path: string, index: boolean | undefined): number {\n  let segments = path.split(\"/\");\n  let initialScore = segments.length;\n  if (segments.some(isSplat)) {\n    initialScore += splatPenalty;\n  }\n\n  if (index) {\n    initialScore += indexRouteValue;\n  }\n\n  return segments\n    .filter((s) => !isSplat(s))\n    .reduce(\n      (score, segment) =>\n        score +\n        (paramRe.test(segment)\n          ? dynamicSegmentValue\n          : segment === \"\"\n          ? emptySegmentValue\n          : staticSegmentValue),\n      initialScore\n    );\n}\n\nfunction compareIndexes(a: number[], b: number[]): number {\n  let siblings =\n    a.length === b.length && a.slice(0, -1).every((n, i) => n === b[i]);\n\n  return siblings\n    ? // If two routes are siblings, we should try to match the earlier sibling\n      // first. This allows people to have fine-grained control over the matching\n      // behavior by simply putting routes with identical paths in the order they\n      // want them tried.\n      a[a.length - 1] - b[b.length - 1]\n    : // Otherwise, it doesn't really make sense to rank non-siblings by index,\n      // so they sort equally.\n      0;\n}\n\nfunction matchRouteBranch<\n  ParamKey extends string = string,\n  RouteObjectType extends AgnosticRouteObject = AgnosticRouteObject\n>(\n  branch: RouteBranch<RouteObjectType>,\n  pathname: string\n): AgnosticRouteMatch<ParamKey, RouteObjectType>[] | null {\n  let { routesMeta } = branch;\n\n  let matchedParams = {};\n  let matchedPathname = \"/\";\n  let matches: AgnosticRouteMatch<ParamKey, RouteObjectType>[] = [];\n  for (let i = 0; i < routesMeta.length; ++i) {\n    let meta = routesMeta[i];\n    let end = i === routesMeta.length - 1;\n    let remainingPathname =\n      matchedPathname === \"/\"\n        ? pathname\n        : pathname.slice(matchedPathname.length) || \"/\";\n    let match = matchPath(\n      { path: meta.relativePath, caseSensitive: meta.caseSensitive, end },\n      remainingPathname\n    );\n\n    if (!match) return null;\n\n    Object.assign(matchedParams, match.params);\n\n    let route = meta.route;\n\n    matches.push({\n      // TODO: Can this as be avoided?\n      params: matchedParams as Params<ParamKey>,\n      pathname: joinPaths([matchedPathname, match.pathname]),\n      pathnameBase: normalizePathname(\n        joinPaths([matchedPathname, match.pathnameBase])\n      ),\n      route,\n    });\n\n    if (match.pathnameBase !== \"/\") {\n      matchedPathname = joinPaths([matchedPathname, match.pathnameBase]);\n    }\n  }\n\n  return matches;\n}\n\n/**\n * Returns a path with params interpolated.\n *\n * @see https://reactrouter.com/utils/generate-path\n */\nexport function generatePath<Path extends string>(\n  originalPath: Path,\n  params: {\n    [key in PathParam<Path>]: string | null;\n  } = {} as any\n): string {\n  let path = originalPath;\n  if (path.endsWith(\"*\") && path !== \"*\" && !path.endsWith(\"/*\")) {\n    warning(\n      false,\n      `Route path \"${path}\" will be treated as if it were ` +\n        `\"${path.replace(/\\*$/, \"/*\")}\" because the \\`*\\` character must ` +\n        `always follow a \\`/\\` in the pattern. To get rid of this warning, ` +\n        `please change the route path to \"${path.replace(/\\*$/, \"/*\")}\".`\n    );\n    path = path.replace(/\\*$/, \"/*\") as Path;\n  }\n\n  return (\n    path\n      .replace(\n        /^:(\\w+)(\\??)/g,\n        (_, key: PathParam<Path>, optional: string | undefined) => {\n          let param = params[key];\n          if (optional === \"?\") {\n            return param == null ? \"\" : param;\n          }\n          if (param == null) {\n            invariant(false, `Missing \":${key}\" param`);\n          }\n          return param;\n        }\n      )\n      .replace(\n        /\\/:(\\w+)(\\??)/g,\n        (_, key: PathParam<Path>, optional: string | undefined) => {\n          let param = params[key];\n          if (optional === \"?\") {\n            return param == null ? \"\" : `/${param}`;\n          }\n          if (param == null) {\n            invariant(false, `Missing \":${key}\" param`);\n          }\n          return `/${param}`;\n        }\n      )\n      // Remove any optional markers from optional static segments\n      .replace(/\\?/g, \"\")\n      .replace(/(\\/?)\\*/, (_, prefix, __, str) => {\n        const star = \"*\" as PathParam<Path>;\n\n        if (params[star] == null) {\n          // If no splat was provided, trim the trailing slash _unless_ it's\n          // the entire path\n          return str === \"/*\" ? \"/\" : \"\";\n        }\n\n        // Apply the splat\n        return `${prefix}${params[star]}`;\n      })\n  );\n}\n\n/**\n * A PathPattern is used to match on some portion of a URL pathname.\n */\nexport interface PathPattern<Path extends string = string> {\n  /**\n   * A string to match against a URL pathname. May contain `:id`-style segments\n   * to indicate placeholders for dynamic parameters. May also end with `/*` to\n   * indicate matching the rest of the URL pathname.\n   */\n  path: Path;\n  /**\n   * Should be `true` if the static portions of the `path` should be matched in\n   * the same case.\n   */\n  caseSensitive?: boolean;\n  /**\n   * Should be `true` if this pattern should match the entire URL pathname.\n   */\n  end?: boolean;\n}\n\n/**\n * A PathMatch contains info about how a PathPattern matched on a URL pathname.\n */\nexport interface PathMatch<ParamKey extends string = string> {\n  /**\n   * The names and values of dynamic parameters in the URL.\n   */\n  params: Params<ParamKey>;\n  /**\n   * The portion of the URL pathname that was matched.\n   */\n  pathname: string;\n  /**\n   * The portion of the URL pathname that was matched before child routes.\n   */\n  pathnameBase: string;\n  /**\n   * The pattern that was used to match.\n   */\n  pattern: PathPattern;\n}\n\ntype Mutable<T> = {\n  -readonly [P in keyof T]: T[P];\n};\n\n/**\n * Performs pattern matching on a URL pathname and returns information about\n * the match.\n *\n * @see https://reactrouter.com/utils/match-path\n */\nexport function matchPath<\n  ParamKey extends ParamParseKey<Path>,\n  Path extends string\n>(\n  pattern: PathPattern<Path> | Path,\n  pathname: string\n): PathMatch<ParamKey> | null {\n  if (typeof pattern === \"string\") {\n    pattern = { path: pattern, caseSensitive: false, end: true };\n  }\n\n  let [matcher, paramNames] = compilePath(\n    pattern.path,\n    pattern.caseSensitive,\n    pattern.end\n  );\n\n  let match = pathname.match(matcher);\n  if (!match) return null;\n\n  let matchedPathname = match[0];\n  let pathnameBase = matchedPathname.replace(/(.)\\/+$/, \"$1\");\n  let captureGroups = match.slice(1);\n  let params: Params = paramNames.reduce<Mutable<Params>>(\n    (memo, paramName, index) => {\n      // We need to compute the pathnameBase here using the raw splat value\n      // instead of using params[\"*\"] later because it will be decoded then\n      if (paramName === \"*\") {\n        let splatValue = captureGroups[index] || \"\";\n        pathnameBase = matchedPathname\n          .slice(0, matchedPathname.length - splatValue.length)\n          .replace(/(.)\\/+$/, \"$1\");\n      }\n\n      memo[paramName] = safelyDecodeURIComponent(\n        captureGroups[index] || \"\",\n        paramName\n      );\n      return memo;\n    },\n    {}\n  );\n\n  return {\n    params,\n    pathname: matchedPathname,\n    pathnameBase,\n    pattern,\n  };\n}\n\nfunction compilePath(\n  path: string,\n  caseSensitive = false,\n  end = true\n): [RegExp, string[]] {\n  warning(\n    path === \"*\" || !path.endsWith(\"*\") || path.endsWith(\"/*\"),\n    `Route path \"${path}\" will be treated as if it were ` +\n      `\"${path.replace(/\\*$/, \"/*\")}\" because the \\`*\\` character must ` +\n      `always follow a \\`/\\` in the pattern. To get rid of this warning, ` +\n      `please change the route path to \"${path.replace(/\\*$/, \"/*\")}\".`\n  );\n\n  let paramNames: string[] = [];\n  let regexpSource =\n    \"^\" +\n    path\n      .replace(/\\/*\\*?$/, \"\") // Ignore trailing / and /*, we'll handle it below\n      .replace(/^\\/*/, \"/\") // Make sure it has a leading /\n      .replace(/[\\\\.*+^$?{}|()[\\]]/g, \"\\\\$&\") // Escape special regex chars\n      .replace(/\\/:(\\w+)/g, (_: string, paramName: string) => {\n        paramNames.push(paramName);\n        return \"/([^\\\\/]+)\";\n      });\n\n  if (path.endsWith(\"*\")) {\n    paramNames.push(\"*\");\n    regexpSource +=\n      path === \"*\" || path === \"/*\"\n        ? \"(.*)$\" // Already matched the initial /, just match the rest\n        : \"(?:\\\\/(.+)|\\\\/*)$\"; // Don't include the / in params[\"*\"]\n  } else if (end) {\n    // When matching to the end, ignore trailing slashes\n    regexpSource += \"\\\\/*$\";\n  } else if (path !== \"\" && path !== \"/\") {\n    // If our path is non-empty and contains anything beyond an initial slash,\n    // then we have _some_ form of path in our regex so we should expect to\n    // match only if we find the end of this path segment.  Look for an optional\n    // non-captured trailing slash (to match a portion of the URL) or the end\n    // of the path (if we've matched to the end).  We used to do this with a\n    // word boundary but that gives false positives on routes like\n    // /user-preferences since `-` counts as a word boundary.\n    regexpSource += \"(?:(?=\\\\/|$))\";\n  } else {\n    // Nothing to match for \"\" or \"/\"\n  }\n\n  let matcher = new RegExp(regexpSource, caseSensitive ? undefined : \"i\");\n\n  return [matcher, paramNames];\n}\n\nfunction safelyDecodeURI(value: string) {\n  try {\n    return decodeURI(value);\n  } catch (error) {\n    warning(\n      false,\n      `The URL path \"${value}\" could not be decoded because it is is a ` +\n        `malformed URL segment. This is probably due to a bad percent ` +\n        `encoding (${error}).`\n    );\n\n    return value;\n  }\n}\n\nfunction safelyDecodeURIComponent(value: string, paramName: string) {\n  try {\n    return decodeURIComponent(value);\n  } catch (error) {\n    warning(\n      false,\n      `The value for the URL param \"${paramName}\" will not be decoded because` +\n        ` the string \"${value}\" is a malformed URL segment. This is probably` +\n        ` due to a bad percent encoding (${error}).`\n    );\n\n    return value;\n  }\n}\n\n/**\n * @private\n */\nexport function stripBasename(\n  pathname: string,\n  basename: string\n): string | null {\n  if (basename === \"/\") return pathname;\n\n  if (!pathname.toLowerCase().startsWith(basename.toLowerCase())) {\n    return null;\n  }\n\n  // We want to leave trailing slash behavior in the user's control, so if they\n  // specify a basename with a trailing slash, we should support it\n  let startIndex = basename.endsWith(\"/\")\n    ? basename.length - 1\n    : basename.length;\n  let nextChar = pathname.charAt(startIndex);\n  if (nextChar && nextChar !== \"/\") {\n    // pathname does not start with basename/\n    return null;\n  }\n\n  return pathname.slice(startIndex) || \"/\";\n}\n\n/**\n * @private\n */\nexport function warning(cond: any, message: string): void {\n  if (!cond) {\n    // eslint-disable-next-line no-console\n    if (typeof console !== \"undefined\") console.warn(message);\n\n    try {\n      // Welcome to debugging @remix-run/router!\n      //\n      // This error is thrown as a convenience so you can more easily\n      // find the source for a warning that appears in the console by\n      // enabling \"pause on exceptions\" in your JavaScript debugger.\n      throw new Error(message);\n      // eslint-disable-next-line no-empty\n    } catch (e) {}\n  }\n}\n\n/**\n * Returns a resolved path object relative to the given pathname.\n *\n * @see https://reactrouter.com/utils/resolve-path\n */\nexport function resolvePath(to: To, fromPathname = \"/\"): Path {\n  let {\n    pathname: toPathname,\n    search = \"\",\n    hash = \"\",\n  } = typeof to === \"string\" ? parsePath(to) : to;\n\n  let pathname = toPathname\n    ? toPathname.startsWith(\"/\")\n      ? toPathname\n      : resolvePathname(toPathname, fromPathname)\n    : fromPathname;\n\n  return {\n    pathname,\n    search: normalizeSearch(search),\n    hash: normalizeHash(hash),\n  };\n}\n\nfunction resolvePathname(relativePath: string, fromPathname: string): string {\n  let segments = fromPathname.replace(/\\/+$/, \"\").split(\"/\");\n  let relativeSegments = relativePath.split(\"/\");\n\n  relativeSegments.forEach((segment) => {\n    if (segment === \"..\") {\n      // Keep the root \"\" segment so the pathname starts at /\n      if (segments.length > 1) segments.pop();\n    } else if (segment !== \".\") {\n      segments.push(segment);\n    }\n  });\n\n  return segments.length > 1 ? segments.join(\"/\") : \"/\";\n}\n\nfunction getInvalidPathError(\n  char: string,\n  field: string,\n  dest: string,\n  path: Partial<Path>\n) {\n  return (\n    `Cannot include a '${char}' character in a manually specified ` +\n    `\\`to.${field}\\` field [${JSON.stringify(\n      path\n    )}].  Please separate it out to the ` +\n    `\\`to.${dest}\\` field. Alternatively you may provide the full path as ` +\n    `a string in <Link to=\"...\"> and the router will parse it for you.`\n  );\n}\n\n/**\n * @private\n *\n * When processing relative navigation we want to ignore ancestor routes that\n * do not contribute to the path, such that index/pathless layout routes don't\n * interfere.\n *\n * For example, when moving a route element into an index route and/or a\n * pathless layout route, relative link behavior contained within should stay\n * the same.  Both of the following examples should link back to the root:\n *\n *   <Route path=\"/\">\n *     <Route path=\"accounts\" element={<Link to=\"..\"}>\n *   </Route>\n *\n *   <Route path=\"/\">\n *     <Route path=\"accounts\">\n *       <Route element={<AccountsLayout />}>       // <-- Does not contribute\n *         <Route index element={<Link to=\"..\"} />  // <-- Does not contribute\n *       </Route\n *     </Route>\n *   </Route>\n */\nexport function getPathContributingMatches<\n  T extends AgnosticRouteMatch = AgnosticRouteMatch\n>(matches: T[]) {\n  return matches.filter(\n    (match, index) =>\n      index === 0 || (match.route.path && match.route.path.length > 0)\n  );\n}\n\n/**\n * @private\n */\nexport function resolveTo(\n  toArg: To,\n  routePathnames: string[],\n  locationPathname: string,\n  isPathRelative = false\n): Path {\n  let to: Partial<Path>;\n  if (typeof toArg === \"string\") {\n    to = parsePath(toArg);\n  } else {\n    to = { ...toArg };\n\n    invariant(\n      !to.pathname || !to.pathname.includes(\"?\"),\n      getInvalidPathError(\"?\", \"pathname\", \"search\", to)\n    );\n    invariant(\n      !to.pathname || !to.pathname.includes(\"#\"),\n      getInvalidPathError(\"#\", \"pathname\", \"hash\", to)\n    );\n    invariant(\n      !to.search || !to.search.includes(\"#\"),\n      getInvalidPathError(\"#\", \"search\", \"hash\", to)\n    );\n  }\n\n  let isEmptyPath = toArg === \"\" || to.pathname === \"\";\n  let toPathname = isEmptyPath ? \"/\" : to.pathname;\n\n  let from: string;\n\n  // Routing is relative to the current pathname if explicitly requested.\n  //\n  // If a pathname is explicitly provided in `to`, it should be relative to the\n  // route context. This is explained in `Note on `<Link to>` values` in our\n  // migration guide from v5 as a means of disambiguation between `to` values\n  // that begin with `/` and those that do not. However, this is problematic for\n  // `to` values that do not provide a pathname. `to` can simply be a search or\n  // hash string, in which case we should assume that the navigation is relative\n  // to the current location's pathname and *not* the route pathname.\n  if (isPathRelative || toPathname == null) {\n    from = locationPathname;\n  } else {\n    let routePathnameIndex = routePathnames.length - 1;\n\n    if (toPathname.startsWith(\"..\")) {\n      let toSegments = toPathname.split(\"/\");\n\n      // Each leading .. segment means \"go up one route\" instead of \"go up one\n      // URL segment\".  This is a key difference from how <a href> works and a\n      // major reason we call this a \"to\" value instead of a \"href\".\n      while (toSegments[0] === \"..\") {\n        toSegments.shift();\n        routePathnameIndex -= 1;\n      }\n\n      to.pathname = toSegments.join(\"/\");\n    }\n\n    // If there are more \"..\" segments than parent routes, resolve relative to\n    // the root / URL.\n    from = routePathnameIndex >= 0 ? routePathnames[routePathnameIndex] : \"/\";\n  }\n\n  let path = resolvePath(to, from);\n\n  // Ensure the pathname has a trailing slash if the original \"to\" had one\n  let hasExplicitTrailingSlash =\n    toPathname && toPathname !== \"/\" && toPathname.endsWith(\"/\");\n  // Or if this was a link to the current path which has a trailing slash\n  let hasCurrentTrailingSlash =\n    (isEmptyPath || toPathname === \".\") && locationPathname.endsWith(\"/\");\n  if (\n    !path.pathname.endsWith(\"/\") &&\n    (hasExplicitTrailingSlash || hasCurrentTrailingSlash)\n  ) {\n    path.pathname += \"/\";\n  }\n\n  return path;\n}\n\n/**\n * @private\n */\nexport function getToPathname(to: To): string | undefined {\n  // Empty strings should be treated the same as / paths\n  return to === \"\" || (to as Path).pathname === \"\"\n    ? \"/\"\n    : typeof to === \"string\"\n    ? parsePath(to).pathname\n    : to.pathname;\n}\n\n/**\n * @private\n */\nexport const joinPaths = (paths: string[]): string =>\n  paths.join(\"/\").replace(/\\/\\/+/g, \"/\");\n\n/**\n * @private\n */\nexport const normalizePathname = (pathname: string): string =>\n  pathname.replace(/\\/+$/, \"\").replace(/^\\/*/, \"/\");\n\n/**\n * @private\n */\nexport const normalizeSearch = (search: string): string =>\n  !search || search === \"?\"\n    ? \"\"\n    : search.startsWith(\"?\")\n    ? search\n    : \"?\" + search;\n\n/**\n * @private\n */\nexport const normalizeHash = (hash: string): string =>\n  !hash || hash === \"#\" ? \"\" : hash.startsWith(\"#\") ? hash : \"#\" + hash;\n\nexport type JsonFunction = <Data>(\n  data: Data,\n  init?: number | ResponseInit\n) => Response;\n\n/**\n * This is a shortcut for creating `application/json` responses. Converts `data`\n * to JSON and sets the `Content-Type` header.\n */\nexport const json: JsonFunction = (data, init = {}) => {\n  let responseInit = typeof init === \"number\" ? { status: init } : init;\n\n  let headers = new Headers(responseInit.headers);\n  if (!headers.has(\"Content-Type\")) {\n    headers.set(\"Content-Type\", \"application/json; charset=utf-8\");\n  }\n\n  return new Response(JSON.stringify(data), {\n    ...responseInit,\n    headers,\n  });\n};\n\nexport interface TrackedPromise extends Promise<any> {\n  _tracked?: boolean;\n  _data?: any;\n  _error?: any;\n}\n\nexport class AbortedDeferredError extends Error {}\n\nexport class DeferredData {\n  private pendingKeysSet: Set<string> = new Set<string>();\n  private controller: AbortController;\n  private abortPromise: Promise<void>;\n  private unlistenAbortSignal: () => void;\n  private subscribers: Set<(aborted: boolean, settledKey?: string) => void> =\n    new Set();\n  data: Record<string, unknown>;\n  init?: ResponseInit;\n  deferredKeys: string[] = [];\n\n  constructor(data: Record<string, unknown>, responseInit?: ResponseInit) {\n    invariant(\n      data && typeof data === \"object\" && !Array.isArray(data),\n      \"defer() only accepts plain objects\"\n    );\n\n    // Set up an AbortController + Promise we can race against to exit early\n    // cancellation\n    let reject: (e: AbortedDeferredError) => void;\n    this.abortPromise = new Promise((_, r) => (reject = r));\n    this.controller = new AbortController();\n    let onAbort = () =>\n      reject(new AbortedDeferredError(\"Deferred data aborted\"));\n    this.unlistenAbortSignal = () =>\n      this.controller.signal.removeEventListener(\"abort\", onAbort);\n    this.controller.signal.addEventListener(\"abort\", onAbort);\n\n    this.data = Object.entries(data).reduce(\n      (acc, [key, value]) =>\n        Object.assign(acc, {\n          [key]: this.trackPromise(key, value),\n        }),\n      {}\n    );\n\n    if (this.done) {\n      // All incoming values were resolved\n      this.unlistenAbortSignal();\n    }\n\n    this.init = responseInit;\n  }\n\n  private trackPromise(\n    key: string,\n    value: Promise<unknown> | unknown\n  ): TrackedPromise | unknown {\n    if (!(value instanceof Promise)) {\n      return value;\n    }\n\n    this.deferredKeys.push(key);\n    this.pendingKeysSet.add(key);\n\n    // We store a little wrapper promise that will be extended with\n    // _data/_error props upon resolve/reject\n    let promise: TrackedPromise = Promise.race([value, this.abortPromise]).then(\n      (data) => this.onSettle(promise, key, null, data as unknown),\n      (error) => this.onSettle(promise, key, error as unknown)\n    );\n\n    // Register rejection listeners to avoid uncaught promise rejections on\n    // errors or aborted deferred values\n    promise.catch(() => {});\n\n    Object.defineProperty(promise, \"_tracked\", { get: () => true });\n    return promise;\n  }\n\n  private onSettle(\n    promise: TrackedPromise,\n    key: string,\n    error: unknown,\n    data?: unknown\n  ): unknown {\n    if (\n      this.controller.signal.aborted &&\n      error instanceof AbortedDeferredError\n    ) {\n      this.unlistenAbortSignal();\n      Object.defineProperty(promise, \"_error\", { get: () => error });\n      return Promise.reject(error);\n    }\n\n    this.pendingKeysSet.delete(key);\n\n    if (this.done) {\n      // Nothing left to abort!\n      this.unlistenAbortSignal();\n    }\n\n    if (error) {\n      Object.defineProperty(promise, \"_error\", { get: () => error });\n      this.emit(false, key);\n      return Promise.reject(error);\n    }\n\n    Object.defineProperty(promise, \"_data\", { get: () => data });\n    this.emit(false, key);\n    return data;\n  }\n\n  private emit(aborted: boolean, settledKey?: string) {\n    this.subscribers.forEach((subscriber) => subscriber(aborted, settledKey));\n  }\n\n  subscribe(fn: (aborted: boolean, settledKey?: string) => void) {\n    this.subscribers.add(fn);\n    return () => this.subscribers.delete(fn);\n  }\n\n  cancel() {\n    this.controller.abort();\n    this.pendingKeysSet.forEach((v, k) => this.pendingKeysSet.delete(k));\n    this.emit(true);\n  }\n\n  async resolveData(signal: AbortSignal) {\n    let aborted = false;\n    if (!this.done) {\n      let onAbort = () => this.cancel();\n      signal.addEventListener(\"abort\", onAbort);\n      aborted = await new Promise((resolve) => {\n        this.subscribe((aborted) => {\n          signal.removeEventListener(\"abort\", onAbort);\n          if (aborted || this.done) {\n            resolve(aborted);\n          }\n        });\n      });\n    }\n    return aborted;\n  }\n\n  get done() {\n    return this.pendingKeysSet.size === 0;\n  }\n\n  get unwrappedData() {\n    invariant(\n      this.data !== null && this.done,\n      \"Can only unwrap data on initialized and settled deferreds\"\n    );\n\n    return Object.entries(this.data).reduce(\n      (acc, [key, value]) =>\n        Object.assign(acc, {\n          [key]: unwrapTrackedPromise(value),\n        }),\n      {}\n    );\n  }\n\n  get pendingKeys() {\n    return Array.from(this.pendingKeysSet);\n  }\n}\n\nfunction isTrackedPromise(value: any): value is TrackedPromise {\n  return (\n    value instanceof Promise && (value as TrackedPromise)._tracked === true\n  );\n}\n\nfunction unwrapTrackedPromise(value: any) {\n  if (!isTrackedPromise(value)) {\n    return value;\n  }\n\n  if (value._error) {\n    throw value._error;\n  }\n  return value._data;\n}\n\nexport type DeferFunction = (\n  data: Record<string, unknown>,\n  init?: number | ResponseInit\n) => DeferredData;\n\nexport const defer: DeferFunction = (data, init = {}) => {\n  let responseInit = typeof init === \"number\" ? { status: init } : init;\n\n  return new DeferredData(data, responseInit);\n};\n\nexport type RedirectFunction = (\n  url: string,\n  init?: number | ResponseInit\n) => Response;\n\n/**\n * A redirect response. Sets the status code and the `Location` header.\n * Defaults to \"302 Found\".\n */\nexport const redirect: RedirectFunction = (url, init = 302) => {\n  let responseInit = init;\n  if (typeof responseInit === \"number\") {\n    responseInit = { status: responseInit };\n  } else if (typeof responseInit.status === \"undefined\") {\n    responseInit.status = 302;\n  }\n\n  let headers = new Headers(responseInit.headers);\n  headers.set(\"Location\", url);\n\n  return new Response(null, {\n    ...responseInit,\n    headers,\n  });\n};\n\n/**\n * @private\n * Utility class we use to hold auto-unwrapped 4xx/5xx Response bodies\n */\nexport class ErrorResponse {\n  status: number;\n  statusText: string;\n  data: any;\n  error?: Error;\n  internal: boolean;\n\n  constructor(\n    status: number,\n    statusText: string | undefined,\n    data: any,\n    internal = false\n  ) {\n    this.status = status;\n    this.statusText = statusText || \"\";\n    this.internal = internal;\n    if (data instanceof Error) {\n      this.data = data.toString();\n      this.error = data;\n    } else {\n      this.data = data;\n    }\n  }\n}\n\n/**\n * Check if the given error is an ErrorResponse generated from a 4xx/5xx\n * Response thrown from an action/loader\n */\nexport function isRouteErrorResponse(error: any): error is ErrorResponse {\n  return (\n    error != null &&\n    typeof error.status === \"number\" &&\n    typeof error.statusText === \"string\" &&\n    typeof error.internal === \"boolean\" &&\n    \"data\" in error\n  );\n}\n",
-        "export default function _defineProperty(obj, key, value) {\n  if (key in obj) {\n    Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: true,\n      configurable: true,\n      writable: true\n    });\n  } else {\n    obj[key] = value;\n  }\n\n  return obj;\n}",
         "import arrayWithHoles from \"@babel/runtime/helpers/esm/arrayWithHoles\";\nimport iterableToArrayLimit from \"@babel/runtime/helpers/esm/iterableToArrayLimit\";\nimport unsupportedIterableToArray from \"@babel/runtime/helpers/esm/unsupportedIterableToArray\";\nimport nonIterableRest from \"@babel/runtime/helpers/esm/nonIterableRest\";\nexport default function _slicedToArray(arr, i) {\n  return arrayWithHoles(arr) || iterableToArrayLimit(arr, i) || unsupportedIterableToArray(arr, i) || nonIterableRest();\n}",
         "export default function _iterableToArrayLimit(arr, i) {\n  if (typeof Symbol === \"undefined\" || !(Symbol.iterator in Object(arr))) return;\n  var _arr = [];\n  var _n = true;\n  var _d = false;\n  var _e = undefined;\n\n  try {\n    for (var _i = arr[Symbol.iterator](), _s; !(_n = (_s = _i.next()).done); _n = true) {\n      _arr.push(_s.value);\n\n      if (i && _arr.length === i) break;\n    }\n  } catch (err) {\n    _d = true;\n    _e = err;\n  } finally {\n    try {\n      if (!_n && _i[\"return\"] != null) _i[\"return\"]();\n    } finally {\n      if (_d) throw _e;\n    }\n  }\n\n  return _arr;\n}",
+        "export default function _defineProperty(obj, key, value) {\n  if (key in obj) {\n    Object.defineProperty(obj, key, {\n      value: value,\n      enumerable: true,\n      configurable: true,\n      writable: true\n    });\n  } else {\n    obj[key] = value;\n  }\n\n  return obj;\n}",
         "export default function _extends() {\n  _extends = Object.assign || function (target) {\n    for (var i = 1; i < arguments.length; i++) {\n      var source = arguments[i];\n\n      for (var key in source) {\n        if (Object.prototype.hasOwnProperty.call(source, key)) {\n          target[key] = source[key];\n        }\n      }\n    }\n\n    return target;\n  };\n\n  return _extends.apply(this, arguments);\n}",
         "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n */\n\nimport * as React from \"react\";\n\n/**\n * inlined Object.is polyfill to avoid requiring consumers ship their own\n * https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/is\n */\nfunction isPolyfill(x: any, y: any) {\n  return (\n    (x === y && (x !== 0 || 1 / x === 1 / y)) || (x !== x && y !== y) // eslint-disable-line no-self-compare\n  );\n}\n\nconst is: (x: any, y: any) => boolean =\n  typeof Object.is === \"function\" ? Object.is : isPolyfill;\n\n// Intentionally not using named imports because Rollup uses dynamic\n// dispatch for CommonJS interop named imports.\nconst { useState, useEffect, useLayoutEffect, useDebugValue } = React;\n\nlet didWarnOld18Alpha = false;\nlet didWarnUncachedGetSnapshot = false;\n\n// Disclaimer: This shim breaks many of the rules of React, and only works\n// because of a very particular set of implementation details and assumptions\n// -- change any one of them and it will break. The most important assumption\n// is that updates are always synchronous, because concurrent rendering is\n// only available in versions of React that also have a built-in\n// useSyncExternalStore API. And we only use this shim when the built-in API\n// does not exist.\n//\n// Do not assume that the clever hacks used by this hook also work in general.\n// The point of this shim is to replace the need for hacks by other libraries.\nexport function useSyncExternalStore<T>(\n  subscribe: (fn: () => void) => () => void,\n  getSnapshot: () => T,\n  // Note: The shim does not use getServerSnapshot, because pre-18 versions of\n  // React do not expose a way to check if we're hydrating. So users of the shim\n  // will need to track that themselves and return the correct value\n  // from `getSnapshot`.\n  getServerSnapshot?: () => T\n): T {\n  if (__DEV__) {\n    if (!didWarnOld18Alpha) {\n      if (\"startTransition\" in React) {\n        didWarnOld18Alpha = true;\n        console.error(\n          \"You are using an outdated, pre-release alpha of React 18 that \" +\n            \"does not support useSyncExternalStore. The \" +\n            \"use-sync-external-store shim will not work correctly. Upgrade \" +\n            \"to a newer pre-release.\"\n        );\n      }\n    }\n  }\n\n  // Read the current snapshot from the store on every render. Again, this\n  // breaks the rules of React, and only works here because of specific\n  // implementation details, most importantly that updates are\n  // always synchronous.\n  const value = getSnapshot();\n  if (__DEV__) {\n    if (!didWarnUncachedGetSnapshot) {\n      const cachedValue = getSnapshot();\n      if (!is(value, cachedValue)) {\n        console.error(\n          \"The result of getSnapshot should be cached to avoid an infinite loop\"\n        );\n        didWarnUncachedGetSnapshot = true;\n      }\n    }\n  }\n\n  // Because updates are synchronous, we don't queue them. Instead we force a\n  // re-render whenever the subscribed state changes by updating an some\n  // arbitrary useState hook. Then, during render, we call getSnapshot to read\n  // the current value.\n  //\n  // Because we don't actually use the state returned by the useState hook, we\n  // can save a bit of memory by storing other stuff in that slot.\n  //\n  // To implement the early bailout, we need to track some things on a mutable\n  // object. Usually, we would put that in a useRef hook, but we can stash it in\n  // our useState hook instead.\n  //\n  // To force a re-render, we call forceUpdate({inst}). That works because the\n  // new object always fails an equality check.\n  const [{ inst }, forceUpdate] = useState({ inst: { value, getSnapshot } });\n\n  // Track the latest getSnapshot function with a ref. This needs to be updated\n  // in the layout phase so we can access it during the tearing check that\n  // happens on subscribe.\n  useLayoutEffect(() => {\n    inst.value = value;\n    inst.getSnapshot = getSnapshot;\n\n    // Whenever getSnapshot or subscribe changes, we need to check in the\n    // commit phase if there was an interleaved mutation. In concurrent mode\n    // this can happen all the time, but even in synchronous mode, an earlier\n    // effect may have mutated the store.\n    if (checkIfSnapshotChanged(inst)) {\n      // Force a re-render.\n      forceUpdate({ inst });\n    }\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [subscribe, value, getSnapshot]);\n\n  useEffect(() => {\n    // Check for changes right before subscribing. Subsequent changes will be\n    // detected in the subscription handler.\n    if (checkIfSnapshotChanged(inst)) {\n      // Force a re-render.\n      forceUpdate({ inst });\n    }\n    const handleStoreChange = () => {\n      // TODO: Because there is no cross-renderer API for batching updates, it's\n      // up to the consumer of this library to wrap their subscription event\n      // with unstable_batchedUpdates. Should we try to detect when this isn't\n      // the case and print a warning in development?\n\n      // The store changed. Check if the snapshot changed since the last time we\n      // read from the store.\n      if (checkIfSnapshotChanged(inst)) {\n        // Force a re-render.\n        forceUpdate({ inst });\n      }\n    };\n    // Subscribe to the store and return a clean-up function.\n    return subscribe(handleStoreChange);\n    // eslint-disable-next-line react-hooks/exhaustive-deps\n  }, [subscribe]);\n\n  useDebugValue(value);\n  return value;\n}\n\nfunction checkIfSnapshotChanged(inst: any) {\n  const latestGetSnapshot = inst.getSnapshot;\n  const prevValue = inst.value;\n  try {\n    const nextValue = latestGetSnapshot();\n    return !is(prevValue, nextValue);\n  } catch (error) {\n    return true;\n  }\n}\n",
         "/**\n * Inlined into the react-router repo since use-sync-external-store does not\n * provide a UMD-compatible package, so we need this to be able to distribute\n * UMD react-router bundles\n */\n\n/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @flow\n */\n\nimport * as React from \"react\";\n\nimport { useSyncExternalStore as client } from \"./useSyncExternalStoreShimClient\";\nimport { useSyncExternalStore as server } from \"./useSyncExternalStoreShimServer\";\n\nconst canUseDOM: boolean = !!(\n  typeof window !== \"undefined\" &&\n  typeof window.document !== \"undefined\" &&\n  typeof window.document.createElement !== \"undefined\"\n);\nconst isServerEnvironment = !canUseDOM;\nconst shim = isServerEnvironment ? server : client;\n\nexport const useSyncExternalStore =\n  \"useSyncExternalStore\" in React\n    ? ((module) => module.useSyncExternalStore)(React)\n    : shim;\n",
         "/**\n * Copyright (c) Facebook, Inc. and its affiliates.\n *\n * This source code is licensed under the MIT license found in the\n * LICENSE file in the root directory of this source tree.\n *\n * @flow\n */\n\nexport function useSyncExternalStore<T>(\n  subscribe: (fn: () => void) => () => void,\n  getSnapshot: () => T,\n  getServerSnapshot?: () => T\n): T {\n  // Note: The shim does not use getServerSnapshot, because pre-18 versions of\n  // React do not expose a way to check if we're hydrating. So users of the shim\n  // will need to track that themselves and return the correct value\n  // from `getSnapshot`.\n  return getSnapshot();\n}\n",
         "import * as React from \"react\";\nimport type {\n  AgnosticRouteMatch,\n  AgnosticIndexRouteObject,\n  AgnosticNonIndexRouteObject,\n  History,\n  Location,\n  Router,\n  StaticHandlerContext,\n  To,\n  TrackedPromise,\n} from \"@remix-run/router\";\nimport type { Action as NavigationType } from \"@remix-run/router\";\n\n// Create react-specific types from the agnostic types in @remix-run/router to\n// export from react-router\nexport interface IndexRouteObject {\n  caseSensitive?: AgnosticIndexRouteObject[\"caseSensitive\"];\n  path?: AgnosticIndexRouteObject[\"path\"];\n  id?: AgnosticIndexRouteObject[\"id\"];\n  loader?: AgnosticIndexRouteObject[\"loader\"];\n  action?: AgnosticIndexRouteObject[\"action\"];\n  hasErrorBoundary?: AgnosticIndexRouteObject[\"hasErrorBoundary\"];\n  shouldRevalidate?: AgnosticIndexRouteObject[\"shouldRevalidate\"];\n  handle?: AgnosticIndexRouteObject[\"handle\"];\n  index: true;\n  children?: undefined;\n  element?: React.ReactNode | null;\n  errorElement?: React.ReactNode | null;\n}\n\nexport interface NonIndexRouteObject {\n  caseSensitive?: AgnosticNonIndexRouteObject[\"caseSensitive\"];\n  path?: AgnosticNonIndexRouteObject[\"path\"];\n  id?: AgnosticNonIndexRouteObject[\"id\"];\n  loader?: AgnosticNonIndexRouteObject[\"loader\"];\n  action?: AgnosticNonIndexRouteObject[\"action\"];\n  hasErrorBoundary?: AgnosticNonIndexRouteObject[\"hasErrorBoundary\"];\n  shouldRevalidate?: AgnosticNonIndexRouteObject[\"shouldRevalidate\"];\n  handle?: AgnosticNonIndexRouteObject[\"handle\"];\n  index?: false;\n  children?: RouteObject[];\n  element?: React.ReactNode | null;\n  errorElement?: React.ReactNode | null;\n}\n\nexport type RouteObject = IndexRouteObject | NonIndexRouteObject;\n\nexport type DataRouteObject = RouteObject & {\n  children?: DataRouteObject[];\n  id: string;\n};\n\nexport interface RouteMatch<\n  ParamKey extends string = string,\n  RouteObjectType extends RouteObject = RouteObject\n> extends AgnosticRouteMatch<ParamKey, RouteObjectType> {}\n\nexport interface DataRouteMatch extends RouteMatch<string, DataRouteObject> {}\n\nexport interface DataRouterContextObject extends NavigationContextObject {\n  router: Router;\n  staticContext?: StaticHandlerContext;\n}\n\nexport const DataRouterContext =\n  React.createContext<DataRouterContextObject | null>(null);\nif (__DEV__) {\n  DataRouterContext.displayName = \"DataRouter\";\n}\n\nexport const DataRouterStateContext = React.createContext<\n  Router[\"state\"] | null\n>(null);\nif (__DEV__) {\n  DataRouterStateContext.displayName = \"DataRouterState\";\n}\n\nexport const AwaitContext = React.createContext<TrackedPromise | null>(null);\nif (__DEV__) {\n  AwaitContext.displayName = \"Await\";\n}\n\nexport type RelativeRoutingType = \"route\" | \"path\";\n\nexport interface NavigateOptions {\n  replace?: boolean;\n  state?: any;\n  preventScrollReset?: boolean;\n  relative?: RelativeRoutingType;\n}\n\n/**\n * A Navigator is a \"location changer\"; it's how you get to different locations.\n *\n * Every history instance conforms to the Navigator interface, but the\n * distinction is useful primarily when it comes to the low-level <Router> API\n * where both the location and a navigator must be provided separately in order\n * to avoid \"tearing\" that may occur in a suspense-enabled app if the action\n * and/or location were to be read directly from the history instance.\n */\nexport interface Navigator {\n  createHref: History[\"createHref\"];\n  // Optional for backwards-compat with Router/HistoryRouter usage (edge case)\n  encodeLocation?: History[\"encodeLocation\"];\n  go: History[\"go\"];\n  push(to: To, state?: any, opts?: NavigateOptions): void;\n  replace(to: To, state?: any, opts?: NavigateOptions): void;\n}\n\ninterface NavigationContextObject {\n  basename: string;\n  navigator: Navigator;\n  static: boolean;\n}\n\nexport const NavigationContext = React.createContext<NavigationContextObject>(\n  null!\n);\n\nif (__DEV__) {\n  NavigationContext.displayName = \"Navigation\";\n}\n\ninterface LocationContextObject {\n  location: Location;\n  navigationType: NavigationType;\n}\n\nexport const LocationContext = React.createContext<LocationContextObject>(\n  null!\n);\n\nif (__DEV__) {\n  LocationContext.displayName = \"Location\";\n}\n\nexport interface RouteContextObject {\n  outlet: React.ReactElement | null;\n  matches: RouteMatch[];\n}\n\nexport const RouteContext = React.createContext<RouteContextObject>({\n  outlet: null,\n  matches: [],\n});\n\nif (__DEV__) {\n  RouteContext.displayName = \"Route\";\n}\n\nexport const RouteErrorContext = React.createContext<any>(null);\n\nif (__DEV__) {\n  RouteErrorContext.displayName = \"RouteError\";\n}\n",
         "import * as React from \"react\";\nimport type {\n  Blocker,\n  BlockerFunction,\n  Location,\n  ParamParseKey,\n  Params,\n  Path,\n  PathMatch,\n  PathPattern,\n  Router as RemixRouter,\n  To,\n} from \"@remix-run/router\";\nimport {\n  Action as NavigationType,\n  invariant,\n  isRouteErrorResponse,\n  joinPaths,\n  matchPath,\n  matchRoutes,\n  parsePath,\n  resolveTo,\n  warning,\n  UNSAFE_getPathContributingMatches as getPathContributingMatches,\n} from \"@remix-run/router\";\n\nimport type {\n  NavigateOptions,\n  RouteContextObject,\n  RouteMatch,\n  RouteObject,\n  DataRouteMatch,\n  RelativeRoutingType,\n} from \"./context\";\nimport {\n  DataRouterContext,\n  DataRouterStateContext,\n  LocationContext,\n  NavigationContext,\n  RouteContext,\n  RouteErrorContext,\n  AwaitContext,\n} from \"./context\";\n\n/**\n * Returns the full href for the given \"to\" value. This is useful for building\n * custom links that are also accessible and preserve right-click behavior.\n *\n * @see https://reactrouter.com/hooks/use-href\n */\nexport function useHref(\n  to: To,\n  { relative }: { relative?: RelativeRoutingType } = {}\n): string {\n  invariant(\n    useInRouterContext(),\n    // TODO: This error is probably because they somehow have 2 versions of the\n    // router loaded. We can help them understand how to avoid that.\n    `useHref() may be used only in the context of a <Router> component.`\n  );\n\n  let { basename, navigator } = React.useContext(NavigationContext);\n  let { hash, pathname, search } = useResolvedPath(to, { relative });\n\n  let joinedPathname = pathname;\n\n  // If we're operating within a basename, prepend it to the pathname prior\n  // to creating the href.  If this is a root navigation, then just use the raw\n  // basename which allows the basename to have full control over the presence\n  // of a trailing slash on root links\n  if (basename !== \"/\") {\n    joinedPathname =\n      pathname === \"/\" ? basename : joinPaths([basename, pathname]);\n  }\n\n  return navigator.createHref({ pathname: joinedPathname, search, hash });\n}\n\n/**\n * Returns true if this component is a descendant of a <Router>.\n *\n * @see https://reactrouter.com/hooks/use-in-router-context\n */\nexport function useInRouterContext(): boolean {\n  return React.useContext(LocationContext) != null;\n}\n\n/**\n * Returns the current location object, which represents the current URL in web\n * browsers.\n *\n * Note: If you're using this it may mean you're doing some of your own\n * \"routing\" in your app, and we'd like to know what your use case is. We may\n * be able to provide something higher-level to better suit your needs.\n *\n * @see https://reactrouter.com/hooks/use-location\n */\nexport function useLocation(): Location {\n  invariant(\n    useInRouterContext(),\n    // TODO: This error is probably because they somehow have 2 versions of the\n    // router loaded. We can help them understand how to avoid that.\n    `useLocation() may be used only in the context of a <Router> component.`\n  );\n\n  return React.useContext(LocationContext).location;\n}\n\n/**\n * Returns the current navigation action which describes how the router came to\n * the current location, either by a pop, push, or replace on the history stack.\n *\n * @see https://reactrouter.com/hooks/use-navigation-type\n */\nexport function useNavigationType(): NavigationType {\n  return React.useContext(LocationContext).navigationType;\n}\n\n/**\n * Returns a PathMatch object if the given pattern matches the current URL.\n * This is useful for components that need to know \"active\" state, e.g.\n * <NavLink>.\n *\n * @see https://reactrouter.com/hooks/use-match\n */\nexport function useMatch<\n  ParamKey extends ParamParseKey<Path>,\n  Path extends string\n>(pattern: PathPattern<Path> | Path): PathMatch<ParamKey> | null {\n  invariant(\n    useInRouterContext(),\n    // TODO: This error is probably because they somehow have 2 versions of the\n    // router loaded. We can help them understand how to avoid that.\n    `useMatch() may be used only in the context of a <Router> component.`\n  );\n\n  let { pathname } = useLocation();\n  return React.useMemo(\n    () => matchPath<ParamKey, Path>(pattern, pathname),\n    [pathname, pattern]\n  );\n}\n\n/**\n * The interface for the navigate() function returned from useNavigate().\n */\nexport interface NavigateFunction {\n  (to: To, options?: NavigateOptions): void;\n  (delta: number): void;\n}\n\n/**\n * Returns an imperative method for changing the location. Used by <Link>s, but\n * may also be used by other elements to change the location.\n *\n * @see https://reactrouter.com/hooks/use-navigate\n */\nexport function useNavigate(): NavigateFunction {\n  invariant(\n    useInRouterContext(),\n    // TODO: This error is probably because they somehow have 2 versions of the\n    // router loaded. We can help them understand how to avoid that.\n    `useNavigate() may be used only in the context of a <Router> component.`\n  );\n\n  let { basename, navigator } = React.useContext(NavigationContext);\n  let { matches } = React.useContext(RouteContext);\n  let { pathname: locationPathname } = useLocation();\n\n  let routePathnamesJson = JSON.stringify(\n    getPathContributingMatches(matches).map((match) => match.pathnameBase)\n  );\n\n  let activeRef = React.useRef(false);\n  React.useEffect(() => {\n    activeRef.current = true;\n  });\n\n  let navigate: NavigateFunction = React.useCallback(\n    (to: To | number, options: NavigateOptions = {}) => {\n      warning(\n        activeRef.current,\n        `You should call navigate() in a React.useEffect(), not when ` +\n          `your component is first rendered.`\n      );\n\n      if (!activeRef.current) return;\n\n      if (typeof to === \"number\") {\n        navigator.go(to);\n        return;\n      }\n\n      let path = resolveTo(\n        to,\n        JSON.parse(routePathnamesJson),\n        locationPathname,\n        options.relative === \"path\"\n      );\n\n      // If we're operating within a basename, prepend it to the pathname prior\n      // to handing off to history.  If this is a root navigation, then we\n      // navigate to the raw basename which allows the basename to have full\n      // control over the presence of a trailing slash on root links\n      if (basename !== \"/\") {\n        path.pathname =\n          path.pathname === \"/\"\n            ? basename\n            : joinPaths([basename, path.pathname]);\n      }\n\n      (!!options.replace ? navigator.replace : navigator.push)(\n        path,\n        options.state,\n        options\n      );\n    },\n    [basename, navigator, routePathnamesJson, locationPathname]\n  );\n\n  return navigate;\n}\n\nconst OutletContext = React.createContext<unknown>(null);\n\n/**\n * Returns the context (if provided) for the child route at this level of the route\n * hierarchy.\n * @see https://reactrouter.com/hooks/use-outlet-context\n */\nexport function useOutletContext<Context = unknown>(): Context {\n  return React.useContext(OutletContext) as Context;\n}\n\n/**\n * Returns the element for the child route at this level of the route\n * hierarchy. Used internally by <Outlet> to render child routes.\n *\n * @see https://reactrouter.com/hooks/use-outlet\n */\nexport function useOutlet(context?: unknown): React.ReactElement | null {\n  let outlet = React.useContext(RouteContext).outlet;\n  if (outlet) {\n    return (\n      <OutletContext.Provider value={context}>{outlet}</OutletContext.Provider>\n    );\n  }\n  return outlet;\n}\n\n/**\n * Returns an object of key/value pairs of the dynamic params from the current\n * URL that were matched by the route path.\n *\n * @see https://reactrouter.com/hooks/use-params\n */\nexport function useParams<\n  ParamsOrKey extends string | Record<string, string | undefined> = string\n>(): Readonly<\n  [ParamsOrKey] extends [string] ? Params<ParamsOrKey> : Partial<ParamsOrKey>\n> {\n  let { matches } = React.useContext(RouteContext);\n  let routeMatch = matches[matches.length - 1];\n  return routeMatch ? (routeMatch.params as any) : {};\n}\n\n/**\n * Resolves the pathname of the given `to` value against the current location.\n *\n * @see https://reactrouter.com/hooks/use-resolved-path\n */\nexport function useResolvedPath(\n  to: To,\n  { relative }: { relative?: RelativeRoutingType } = {}\n): Path {\n  let { matches } = React.useContext(RouteContext);\n  let { pathname: locationPathname } = useLocation();\n\n  let routePathnamesJson = JSON.stringify(\n    getPathContributingMatches(matches).map((match) => match.pathnameBase)\n  );\n\n  return React.useMemo(\n    () =>\n      resolveTo(\n        to,\n        JSON.parse(routePathnamesJson),\n        locationPathname,\n        relative === \"path\"\n      ),\n    [to, routePathnamesJson, locationPathname, relative]\n  );\n}\n\n/**\n * Returns the element of the route that matched the current location, prepared\n * with the correct context to render the remainder of the route tree. Route\n * elements in the tree must render an <Outlet> to render their child route's\n * element.\n *\n * @see https://reactrouter.com/hooks/use-routes\n */\nexport function useRoutes(\n  routes: RouteObject[],\n  locationArg?: Partial<Location> | string\n): React.ReactElement | null {\n  invariant(\n    useInRouterContext(),\n    // TODO: This error is probably because they somehow have 2 versions of the\n    // router loaded. We can help them understand how to avoid that.\n    `useRoutes() may be used only in the context of a <Router> component.`\n  );\n\n  let { navigator } = React.useContext(NavigationContext);\n  let dataRouterStateContext = React.useContext(DataRouterStateContext);\n  let { matches: parentMatches } = React.useContext(RouteContext);\n  let routeMatch = parentMatches[parentMatches.length - 1];\n  let parentParams = routeMatch ? routeMatch.params : {};\n  let parentPathname = routeMatch ? routeMatch.pathname : \"/\";\n  let parentPathnameBase = routeMatch ? routeMatch.pathnameBase : \"/\";\n  let parentRoute = routeMatch && routeMatch.route;\n\n  if (__DEV__) {\n    // You won't get a warning about 2 different <Routes> under a <Route>\n    // without a trailing *, but this is a best-effort warning anyway since we\n    // cannot even give the warning unless they land at the parent route.\n    //\n    // Example:\n    //\n    // <Routes>\n    //   {/* This route path MUST end with /* because otherwise\n    //       it will never match /blog/post/123 */}\n    //   <Route path=\"blog\" element={<Blog />} />\n    //   <Route path=\"blog/feed\" element={<BlogFeed />} />\n    // </Routes>\n    //\n    // function Blog() {\n    //   return (\n    //     <Routes>\n    //       <Route path=\"post/:id\" element={<Post />} />\n    //     </Routes>\n    //   );\n    // }\n    let parentPath = (parentRoute && parentRoute.path) || \"\";\n    warningOnce(\n      parentPathname,\n      !parentRoute || parentPath.endsWith(\"*\"),\n      `You rendered descendant <Routes> (or called \\`useRoutes()\\`) at ` +\n        `\"${parentPathname}\" (under <Route path=\"${parentPath}\">) but the ` +\n        `parent route path has no trailing \"*\". This means if you navigate ` +\n        `deeper, the parent won't match anymore and therefore the child ` +\n        `routes will never render.\\n\\n` +\n        `Please change the parent <Route path=\"${parentPath}\"> to <Route ` +\n        `path=\"${parentPath === \"/\" ? \"*\" : `${parentPath}/*`}\">.`\n    );\n  }\n\n  let locationFromContext = useLocation();\n\n  let location;\n  if (locationArg) {\n    let parsedLocationArg =\n      typeof locationArg === \"string\" ? parsePath(locationArg) : locationArg;\n\n    invariant(\n      parentPathnameBase === \"/\" ||\n        parsedLocationArg.pathname?.startsWith(parentPathnameBase),\n      `When overriding the location using \\`<Routes location>\\` or \\`useRoutes(routes, location)\\`, ` +\n        `the location pathname must begin with the portion of the URL pathname that was ` +\n        `matched by all parent routes. The current pathname base is \"${parentPathnameBase}\" ` +\n        `but pathname \"${parsedLocationArg.pathname}\" was given in the \\`location\\` prop.`\n    );\n\n    location = parsedLocationArg;\n  } else {\n    location = locationFromContext;\n  }\n\n  let pathname = location.pathname || \"/\";\n  let remainingPathname =\n    parentPathnameBase === \"/\"\n      ? pathname\n      : pathname.slice(parentPathnameBase.length) || \"/\";\n\n  let matches = matchRoutes(routes, { pathname: remainingPathname });\n\n  if (__DEV__) {\n    warning(\n      parentRoute || matches != null,\n      `No routes matched location \"${location.pathname}${location.search}${location.hash}\" `\n    );\n\n    warning(\n      matches == null ||\n        matches[matches.length - 1].route.element !== undefined,\n      `Matched leaf route at location \"${location.pathname}${location.search}${location.hash}\" does not have an element. ` +\n        `This means it will render an <Outlet /> with a null value by default resulting in an \"empty\" page.`\n    );\n  }\n\n  let renderedMatches = _renderMatches(\n    matches &&\n      matches.map((match) =>\n        Object.assign({}, match, {\n          params: Object.assign({}, parentParams, match.params),\n          pathname: joinPaths([\n            parentPathnameBase,\n            // Re-encode pathnames that were decoded inside matchRoutes\n            navigator.encodeLocation\n              ? navigator.encodeLocation(match.pathname).pathname\n              : match.pathname,\n          ]),\n          pathnameBase:\n            match.pathnameBase === \"/\"\n              ? parentPathnameBase\n              : joinPaths([\n                  parentPathnameBase,\n                  // Re-encode pathnames that were decoded inside matchRoutes\n                  navigator.encodeLocation\n                    ? navigator.encodeLocation(match.pathnameBase).pathname\n                    : match.pathnameBase,\n                ]),\n        })\n      ),\n    parentMatches,\n    dataRouterStateContext || undefined\n  );\n\n  // When a user passes in a `locationArg`, the associated routes need to\n  // be wrapped in a new `LocationContext.Provider` in order for `useLocation`\n  // to use the scoped location instead of the global location.\n  if (locationArg && renderedMatches) {\n    return (\n      <LocationContext.Provider\n        value={{\n          location: {\n            pathname: \"/\",\n            search: \"\",\n            hash: \"\",\n            state: null,\n            key: \"default\",\n            ...location,\n          },\n          navigationType: NavigationType.Pop,\n        }}\n      >\n        {renderedMatches}\n      </LocationContext.Provider>\n    );\n  }\n\n  return renderedMatches;\n}\n\nfunction DefaultErrorElement() {\n  let error = useRouteError();\n  let message = isRouteErrorResponse(error)\n    ? `${error.status} ${error.statusText}`\n    : error instanceof Error\n    ? error.message\n    : JSON.stringify(error);\n  let stack = error instanceof Error ? error.stack : null;\n  let lightgrey = \"rgba(200,200,200, 0.5)\";\n  let preStyles = { padding: \"0.5rem\", backgroundColor: lightgrey };\n  let codeStyles = { padding: \"2px 4px\", backgroundColor: lightgrey };\n\n  let devInfo = null;\n  if (__DEV__) {\n    devInfo = (\n      <>\n        <p>\ud83d\udcbf Hey developer \ud83d\udc4b</p>\n        <p>\n          You can provide a way better UX than this when your app throws errors\n          by providing your own&nbsp;\n          <code style={codeStyles}>errorElement</code> props on&nbsp;\n          <code style={codeStyles}>&lt;Route&gt;</code>\n        </p>\n      </>\n    );\n  }\n\n  return (\n    <>\n      <h2>Unexpected Application Error!</h2>\n      <h3 style={{ fontStyle: \"italic\" }}>{message}</h3>\n      {stack ? <pre style={preStyles}>{stack}</pre> : null}\n      {devInfo}\n    </>\n  );\n}\n\ntype RenderErrorBoundaryProps = React.PropsWithChildren<{\n  location: Location;\n  error: any;\n  component: React.ReactNode;\n  routeContext: RouteContextObject;\n}>;\n\ntype RenderErrorBoundaryState = {\n  location: Location;\n  error: any;\n};\n\nexport class RenderErrorBoundary extends React.Component<\n  RenderErrorBoundaryProps,\n  RenderErrorBoundaryState\n> {\n  constructor(props: RenderErrorBoundaryProps) {\n    super(props);\n    this.state = {\n      location: props.location,\n      error: props.error,\n    };\n  }\n\n  static getDerivedStateFromError(error: any) {\n    return { error: error };\n  }\n\n  static getDerivedStateFromProps(\n    props: RenderErrorBoundaryProps,\n    state: RenderErrorBoundaryState\n  ) {\n    // When we get into an error state, the user will likely click \"back\" to the\n    // previous page that didn't have an error. Because this wraps the entire\n    // application, that will have no effect--the error page continues to display.\n    // This gives us a mechanism to recover from the error when the location changes.\n    //\n    // Whether we're in an error state or not, we update the location in state\n    // so that when we are in an error state, it gets reset when a new location\n    // comes in and the user recovers from the error.\n    if (state.location !== props.location) {\n      return {\n        error: props.error,\n        location: props.location,\n      };\n    }\n\n    // If we're not changing locations, preserve the location but still surface\n    // any new errors that may come through. We retain the existing error, we do\n    // this because the error provided from the app state may be cleared without\n    // the location changing.\n    return {\n      error: props.error || state.error,\n      location: state.location,\n    };\n  }\n\n  componentDidCatch(error: any, errorInfo: any) {\n    console.error(\n      \"React Router caught the following error during render\",\n      error,\n      errorInfo\n    );\n  }\n\n  render() {\n    return this.state.error ? (\n      <RouteContext.Provider value={this.props.routeContext}>\n        <RouteErrorContext.Provider\n          value={this.state.error}\n          children={this.props.component}\n        />\n      </RouteContext.Provider>\n    ) : (\n      this.props.children\n    );\n  }\n}\n\ninterface RenderedRouteProps {\n  routeContext: RouteContextObject;\n  match: RouteMatch<string, RouteObject>;\n  children: React.ReactNode | null;\n}\n\nfunction RenderedRoute({ routeContext, match, children }: RenderedRouteProps) {\n  let dataRouterContext = React.useContext(DataRouterContext);\n\n  // Track how deep we got in our render pass to emulate SSR componentDidCatch\n  // in a DataStaticRouter\n  if (\n    dataRouterContext &&\n    dataRouterContext.static &&\n    dataRouterContext.staticContext &&\n    match.route.errorElement\n  ) {\n    dataRouterContext.staticContext._deepestRenderedBoundaryId = match.route.id;\n  }\n\n  return (\n    <RouteContext.Provider value={routeContext}>\n      {children}\n    </RouteContext.Provider>\n  );\n}\n\nexport function _renderMatches(\n  matches: RouteMatch[] | null,\n  parentMatches: RouteMatch[] = [],\n  dataRouterState?: RemixRouter[\"state\"]\n): React.ReactElement | null {\n  if (matches == null) {\n    if (dataRouterState?.errors) {\n      // Don't bail if we have data router errors so we can render them in the\n      // boundary.  Use the pre-matched (or shimmed) matches\n      matches = dataRouterState.matches as DataRouteMatch[];\n    } else {\n      return null;\n    }\n  }\n\n  let renderedMatches = matches;\n\n  // If we have data errors, trim matches to the highest error boundary\n  let errors = dataRouterState?.errors;\n  if (errors != null) {\n    let errorIndex = renderedMatches.findIndex(\n      (m) => m.route.id && errors?.[m.route.id]\n    );\n    invariant(\n      errorIndex >= 0,\n      `Could not find a matching route for the current errors: ${errors}`\n    );\n    renderedMatches = renderedMatches.slice(\n      0,\n      Math.min(renderedMatches.length, errorIndex + 1)\n    );\n  }\n\n  return renderedMatches.reduceRight((outlet, match, index) => {\n    let error = match.route.id ? errors?.[match.route.id] : null;\n    // Only data routers handle errors\n    let errorElement = dataRouterState\n      ? match.route.errorElement || <DefaultErrorElement />\n      : null;\n    let matches = parentMatches.concat(renderedMatches.slice(0, index + 1));\n    let getChildren = () => (\n      <RenderedRoute match={match} routeContext={{ outlet, matches }}>\n        {error\n          ? errorElement\n          : match.route.element !== undefined\n          ? match.route.element\n          : outlet}\n      </RenderedRoute>\n    );\n    // Only wrap in an error boundary within data router usages when we have an\n    // errorElement on this route.  Otherwise let it bubble up to an ancestor\n    // errorElement\n    return dataRouterState && (match.route.errorElement || index === 0) ? (\n      <RenderErrorBoundary\n        location={dataRouterState.location}\n        component={errorElement}\n        error={error}\n        children={getChildren()}\n        routeContext={{ outlet: null, matches }}\n      />\n    ) : (\n      getChildren()\n    );\n  }, null as React.ReactElement | null);\n}\n\nenum DataRouterHook {\n  UseBlocker = \"useBlocker\",\n  UseRevalidator = \"useRevalidator\",\n}\n\nenum DataRouterStateHook {\n  UseLoaderData = \"useLoaderData\",\n  UseActionData = \"useActionData\",\n  UseRouteError = \"useRouteError\",\n  UseNavigation = \"useNavigation\",\n  UseRouteLoaderData = \"useRouteLoaderData\",\n  UseMatches = \"useMatches\",\n  UseRevalidator = \"useRevalidator\",\n}\n\nfunction getDataRouterConsoleError(\n  hookName: DataRouterHook | DataRouterStateHook\n) {\n  return `${hookName} must be used within a data router.  See https://reactrouter.com/routers/picking-a-router.`;\n}\n\nfunction useDataRouterContext(hookName: DataRouterHook) {\n  let ctx = React.useContext(DataRouterContext);\n  invariant(ctx, getDataRouterConsoleError(hookName));\n  return ctx;\n}\n\nfunction useDataRouterState(hookName: DataRouterStateHook) {\n  let state = React.useContext(DataRouterStateContext);\n  invariant(state, getDataRouterConsoleError(hookName));\n  return state;\n}\n\nfunction useRouteContext(hookName: DataRouterStateHook) {\n  let route = React.useContext(RouteContext);\n  invariant(route, getDataRouterConsoleError(hookName));\n  return route;\n}\n\nfunction useCurrentRouteId(hookName: DataRouterStateHook) {\n  let route = useRouteContext(hookName);\n  let thisRoute = route.matches[route.matches.length - 1];\n  invariant(\n    thisRoute.route.id,\n    `${hookName} can only be used on routes that contain a unique \"id\"`\n  );\n  return thisRoute.route.id;\n}\n\n/**\n * Returns the current navigation, defaulting to an \"idle\" navigation when\n * no navigation is in progress\n */\nexport function useNavigation() {\n  let state = useDataRouterState(DataRouterStateHook.UseNavigation);\n  return state.navigation;\n}\n\n/**\n * Returns a revalidate function for manually triggering revalidation, as well\n * as the current state of any manual revalidations\n */\nexport function useRevalidator() {\n  let dataRouterContext = useDataRouterContext(DataRouterHook.UseRevalidator);\n  let state = useDataRouterState(DataRouterStateHook.UseRevalidator);\n  return {\n    revalidate: dataRouterContext.router.revalidate,\n    state: state.revalidation,\n  };\n}\n\n/**\n * Returns the active route matches, useful for accessing loaderData for\n * parent/child routes or the route \"handle\" property\n */\nexport function useMatches() {\n  let { matches, loaderData } = useDataRouterState(\n    DataRouterStateHook.UseMatches\n  );\n  return React.useMemo(\n    () =>\n      matches.map((match) => {\n        let { pathname, params } = match;\n        // Note: This structure matches that created by createUseMatchesMatch\n        // in the @remix-run/router , so if you change this please also change\n        // that :)  Eventually we'll DRY this up\n        return {\n          id: match.route.id,\n          pathname,\n          params,\n          data: loaderData[match.route.id] as unknown,\n          handle: match.route.handle as unknown,\n        };\n      }),\n    [matches, loaderData]\n  );\n}\n\n/**\n * Returns the loader data for the nearest ancestor Route loader\n */\nexport function useLoaderData(): unknown {\n  let state = useDataRouterState(DataRouterStateHook.UseLoaderData);\n  let routeId = useCurrentRouteId(DataRouterStateHook.UseLoaderData);\n\n  if (state.errors && state.errors[routeId] != null) {\n    console.error(\n      `You cannot \\`useLoaderData\\` in an errorElement (routeId: ${routeId})`\n    );\n    return undefined;\n  }\n  return state.loaderData[routeId];\n}\n\n/**\n * Returns the loaderData for the given routeId\n */\nexport function useRouteLoaderData(routeId: string): unknown {\n  let state = useDataRouterState(DataRouterStateHook.UseRouteLoaderData);\n  return state.loaderData[routeId];\n}\n\n/**\n * Returns the action data for the nearest ancestor Route action\n */\nexport function useActionData(): unknown {\n  let state = useDataRouterState(DataRouterStateHook.UseActionData);\n\n  let route = React.useContext(RouteContext);\n  invariant(route, `useActionData must be used inside a RouteContext`);\n\n  return Object.values(state?.actionData || {})[0];\n}\n\n/**\n * Returns the nearest ancestor Route error, which could be a loader/action\n * error or a render error.  This is intended to be called from your\n * errorElement to display a proper error message.\n */\nexport function useRouteError(): unknown {\n  let error = React.useContext(RouteErrorContext);\n  let state = useDataRouterState(DataRouterStateHook.UseRouteError);\n  let routeId = useCurrentRouteId(DataRouterStateHook.UseRouteError);\n\n  // If this was a render error, we put it in a RouteError context inside\n  // of RenderErrorBoundary\n  if (error) {\n    return error;\n  }\n\n  // Otherwise look for errors from our data router state\n  return state.errors?.[routeId];\n}\n\n/**\n * Returns the happy-path data from the nearest ancestor <Await /> value\n */\nexport function useAsyncValue(): unknown {\n  let value = React.useContext(AwaitContext);\n  return value?._data;\n}\n\n/**\n * Returns the error from the nearest ancestor <Await /> value\n */\nexport function useAsyncError(): unknown {\n  let value = React.useContext(AwaitContext);\n  return value?._error;\n}\n\nlet blockerId = 0;\n\n/**\n * Allow the application to block navigations within the SPA and present the\n * user a confirmation dialog to confirm the navigation.  Mostly used to avoid\n * using half-filled form data.  This does not handle hard-reloads or\n * cross-origin navigations.\n */\nexport function useBlocker(shouldBlock: boolean | BlockerFunction): Blocker {\n  let { router } = useDataRouterContext(DataRouterHook.UseBlocker);\n  let [blockerKey] = React.useState(() => String(++blockerId));\n\n  let blockerFunction = React.useCallback<BlockerFunction>(\n    (args) => {\n      return typeof shouldBlock === \"function\"\n        ? !!shouldBlock(args)\n        : !!shouldBlock;\n    },\n    [shouldBlock]\n  );\n\n  let blocker = router.getBlocker(blockerKey, blockerFunction);\n\n  // Cleanup on unmount\n  React.useEffect(\n    () => () => router.deleteBlocker(blockerKey),\n    [router, blockerKey]\n  );\n\n  return blocker;\n}\n\nconst alreadyWarned: Record<string, boolean> = {};\n\nfunction warningOnce(key: string, cond: boolean, message: string) {\n  if (!cond && !alreadyWarned[key]) {\n    alreadyWarned[key] = true;\n    warning(false, message);\n  }\n}\n",
```

### Comparing `mercury-2.3.1/mercury/frontend-dist/static/js/main.9c1f23c5.chunk.js` & `mercury-2.3.2/mercury/frontend-dist/static/js/main.55ba4c52.chunk.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 (this.webpackJsonpfrontend = this.webpackJsonpfrontend || []).push([
     [0], {
         193: function(e, t, a) {},
         293: function(e, t, a) {},
-        295: function(e, t, a) {
+        294: function(e, t, a) {
             "use strict";
             a.r(t);
             var n = a(1),
                 o = a(39),
                 i = a(313),
                 s = a(5),
                 r = a(11),
                 c = a(20),
                 l = a(6),
                 d = a.n(l),
                 u = a(13),
-                b = a(25),
+                b = a(26),
                 p = a(21),
                 j = a(126),
                 h = a(75),
                 v = a.n(h),
                 f = function() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0],
                         t = sessionStorage.getItem("sessionId");
@@ -64,25 +64,25 @@
                         }
                     }
                 }),
                 w = y.reducer,
                 k = y.actions,
                 N = k.setToken,
                 S = k.setUsername,
-                P = k.setUserInfo,
-                T = function(e) {
+                T = k.setUserInfo,
+                C = function(e) {
                     return e.auth.token
                 },
-                _ = function(e) {
+                P = function(e) {
                     return e.auth.username
                 },
-                C = function(e) {
+                _ = function(e) {
                     return e.auth.user
                 },
-                R = a(9),
+                R = a(8),
                 E = (a(193), a(0));
 
             function A() {
                 return Object(E.jsx)("div", {
                     style: {
                         color: "white",
                         padding: "5px",
@@ -175,35 +175,42 @@
                         })]
                     })
                 })
             }
 
             function D(e) {
                 var t = e.isSitePublic,
-                    a = e.username;
-                return Object(E.jsxs)("header", {
-                    className: "navbar navbar-dark sticky-top bg-dark flex-md-nowrap p-0",
+                    a = e.username,
+                    n = e.logoSrc,
+                    o = e.navbarColor,
+                    i = "",
+                    s = {};
+                return "" === o ? i = "bg-dark" : s = {
+                    backgroundColor: o
+                }, Object(E.jsxs)("header", {
+                    className: "navbar navbar-dark sticky-top ".concat(i, " flex-md-nowrap p-0"),
+                    style: s,
                     children: [Object(E.jsx)(c.b, {
                         className: "navbar-brand col-md-3 col-lg-3 me-0 px-3",
                         to: "/",
-                        children: Object(E.jsx)("img", {
-                            alt: "Mercury",
-                            src: "/static/mercury_logo.svg",
+                        children: "" !== n && "loading" !== n && Object(E.jsx)("img", {
+                            alt: "",
+                            src: n,
                             style: {
                                 height: "28px",
                                 paddingLeft: "10px"
                             }
                         })
                     }), !t && "" === a && Object(E.jsx)(A, {}), "" !== a && Object(E.jsx)(L, {
                         username: a
                     })]
                 })
             }
             var F = a(14),
-                U = a(27),
+                U = a(28),
                 W = Object(b.b)({
                     name: "app",
                     initialState: {
                         view: "app",
                         files: [],
                         filesState: "unknown",
                         showSideBar: !0,
@@ -370,15 +377,30 @@
                 },
                 Oe = function(e) {
                     return e.sites.site.welcome
                 },
                 ge = function(e) {
                     return "PUBLIC" === e.sites.site.share
                 },
-                ye = function() {
+                ye = function(e) {
+                    if (void 0 === e.sites.site.info || "" === e.sites.site.info) return "";
+                    var t = JSON.parse(e.sites.site.info);
+                    return void 0 === (null === t || void 0 === t ? void 0 : t.logoFilename) ? "" : null === t || void 0 === t ? void 0 : t.logoFilename
+                },
+                we = function(e) {
+                    if (void 0 === e.sites.site.info || "" === e.sites.site.info) return "";
+                    var t = JSON.parse(e.sites.site.info);
+                    return void 0 === (null === t || void 0 === t ? void 0 : t.navbarColor) ? "" : null === t || void 0 === t ? void 0 : t.navbarColor
+                },
+                ke = function(e) {
+                    if (void 0 === e.sites.site.info || "" === e.sites.site.info) return "";
+                    var t = JSON.parse(e.sites.site.info);
+                    return void 0 === (null === t || void 0 === t ? void 0 : t.footerText) ? "" : null === t || void 0 === t ? void 0 : t.footerText
+                },
+                Ne = function() {
                     return function() {
                         var e = Object(u.a)(d.a.mark((function e(t) {
                             var a, n, o, s, r;
                             return d.a.wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.prev = 0, t(ve({})), t(fe(ue.Unknown)), a = "single-site", Object({
@@ -404,31 +426,31 @@
                             ])
                         })));
                         return function(t) {
                             return e.apply(this, arguments)
                         }
                     }()
                 },
-                we = {
+                Se = {
                     notebooks: [],
                     loadingState: "loading",
                     selectedNotebook: {},
                     selectedNotebookId: void 0,
                     loadingStateSelected: "loading",
                     watchModeCounter: 0,
                     slidesHash: "",
                     widgets: {},
                     widgetsUrlValues: {},
                     nbIframes: {},
                     widgetsInitialized: !1,
                     urlValuesUsed: !1
                 },
-                ke = Object(b.b)({
+                Te = Object(b.b)({
                     name: "notebooks",
-                    initialState: we,
+                    initialState: Se,
                     reducers: {
                         setWidgetValue: function(e, t) {
                             var a = t.payload,
                                 n = a.key,
                                 o = a.value;
                             e.widgets[n] = o
                         },
@@ -512,66 +534,66 @@
                             e.widgetsInitialized = t.payload
                         },
                         setUrlValuesUsed: function(e, t) {
                             e.urlValuesUsed = t.payload
                         }
                     }
                 }),
-                Ne = ke.reducer,
-                Se = ke.actions,
-                Pe = Se.setNotebooks,
-                Te = Se.setLoadingState,
-                _e = Se.setSelectedNotebook,
-                Ce = Se.setLoadingStateSelected,
-                Re = Se.setSlidesHash,
-                Ee = Se.updateWidgetsParams,
-                Ae = Se.hideWidgets,
-                Le = Se.setWidgetValue,
-                De = Se.setWidgetUrlValue,
-                Fe = (Se.clearWidgets, Se.clearWidgetsUrlValues),
-                Ue = Se.initWidgets,
-                We = Se.updateTitle,
-                Ie = Se.updateShowCode,
-                Me = (Se.setNbIframes, Se.setWidgetsInitialized),
-                He = Se.setUrlValuesUsed,
-                ze = function(e) {
+                Ce = Te.reducer,
+                Pe = Te.actions,
+                _e = Pe.setNotebooks,
+                Re = Pe.setLoadingState,
+                Ee = Pe.setSelectedNotebook,
+                Ae = Pe.setLoadingStateSelected,
+                Le = Pe.setSlidesHash,
+                De = Pe.updateWidgetsParams,
+                Fe = Pe.hideWidgets,
+                Ue = Pe.setWidgetValue,
+                We = Pe.setWidgetUrlValue,
+                Me = Pe.initWidgets,
 
 
 
 