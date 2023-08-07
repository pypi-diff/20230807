# Comparing `tmp/aurori-1.1.0.tar.gz` & `tmp/aurori-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurori-1.1.0.tar", last modified: Mon Aug  7 08:21:45 2023, max compression
+gzip compressed data, was "aurori-1.1.1.tar", last modified: Mon Aug  7 10:11:12 2023, max compression
```

## Comparing `aurori-1.1.0.tar` & `aurori-1.1.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.282291 aurori-1.1.0/
--rw-rw-rw-   0        0        0      100 2023-07-17 04:28:08.000000 aurori-1.1.0/.gitignore
--rw-rw-rw-   0        0        0     1575 2022-07-26 21:50:23.000000 aurori-1.1.0/.gitlab-ci.yml
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:44.880291 aurori-1.1.0/.vscode/
--rw-rw-rw-   0        0        0      986 2022-07-28 10:26:45.000000 aurori-1.1.0/.vscode/launch.json
--rw-rw-rw-   0        0        0    35005 2022-08-05 13:57:15.000000 aurori-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      594 2023-08-07 08:21:45.282291 aurori-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-08-04 09:25:19.000000 aurori-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:44.929328 aurori-1.1.0/aurori/
--rw-rw-rw-   0        0        0    35005 2022-08-05 07:33:15.000000 aurori-1.1.0/aurori/LICENSE.md
--rw-rw-rw-   0        0        0       54 2023-08-04 09:25:21.000000 aurori-1.1.0/aurori/README.md
--rw-rw-rw-   0        0        0     2854 2023-07-28 05:52:22.000000 aurori-1.1.0/aurori/__init__.py
--rw-rw-rw-   0        0        0     2049 2022-01-25 10:07:21.000000 aurori-1.1.0/aurori/alembic.ini
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:44.971291 aurori-1.1.0/aurori/api/
--rw-rw-rw-   0        0        0       33 2023-07-27 08:48:58.000000 aurori-1.1.0/aurori/api/__init__.py
--rw-rw-rw-   0        0        0      259 2023-07-27 11:58:48.000000 aurori-1.1.0/aurori/api/dependencies.py
--rw-rw-rw-   0        0        0       56 2023-07-27 10:07:47.000000 aurori-1.1.0/aurori/api/security.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:44.982292 aurori-1.1.0/aurori/cli/
--rw-rw-rw-   0        0        0      154 2023-07-27 15:09:45.000000 aurori-1.1.0/aurori/cli/__init__.py
--rw-rw-rw-   0        0        0      216 2023-07-27 15:11:13.000000 aurori-1.1.0/aurori/cli/core.py
--rw-rw-rw-   0        0        0     5204 2023-07-18 07:21:56.000000 aurori-1.1.0/aurori/config.py
--rw-rw-rw-   0        0        0      909 2023-07-28 05:43:43.000000 aurori-1.1.0/aurori/database.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.023292 aurori-1.1.0/aurori/jobs/
--rw-rw-rw-   0        0        0     2648 2023-08-07 08:07:10.000000 aurori-1.1.0/aurori/jobs/__init__.py
--rw-rw-rw-   0        0        0     7649 2023-08-07 08:16:08.000000 aurori-1.1.0/aurori/jobs/job.py
--rw-rw-rw-   0        0        0     7119 2023-08-07 08:08:07.000000 aurori-1.1.0/aurori/jobs/jobManager.py
--rw-rw-rw-   0        0        0     1727 2023-08-04 12:16:14.000000 aurori-1.1.0/aurori/jobs/models.py
--rw-rw-rw-   0        0        0     1105 2023-07-27 06:50:14.000000 aurori-1.1.0/aurori/jobs/routes.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.031291 aurori-1.1.0/aurori/logs/
--rw-rw-rw-   0        0        0     1005 2023-07-27 15:29:46.000000 aurori-1.1.0/aurori/logs/__init__.py
--rw-rw-rw-   0        0        0     4899 2023-07-28 06:12:36.000000 aurori-1.1.0/aurori/logs/logManager.py
--rw-rw-rw-   0        0        0     3605 2023-07-28 06:10:15.000000 aurori-1.1.0/aurori/logs/logger.py
--rw-rw-rw-   0        0        0     1064 2023-07-17 04:33:39.000000 aurori-1.1.0/aurori/logs/routes.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.057294 aurori-1.1.0/aurori/migrations/
--rw-rw-rw-   0        0        0      323 2022-02-22 10:25:17.000000 aurori-1.1.0/aurori/migrations/README.md
--rw-rw-rw-   0        0        0     4804 2022-08-04 21:24:37.000000 aurori-1.1.0/aurori/migrations/env.py
--rw-rw-rw-   0        0        0      518 2022-01-25 10:07:21.000000 aurori-1.1.0/aurori/migrations/script.py.mako
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.062292 aurori-1.1.0/aurori/pages/
--rw-rw-rw-   0        0        0      936 2023-07-27 08:21:25.000000 aurori-1.1.0/aurori/pages/__init__.py
--rw-rw-rw-   0        0        0     5500 2023-07-27 08:16:14.000000 aurori-1.1.0/aurori/pages/menuBuilder.py
--rw-rw-rw-   0        0        0     1256 2023-07-18 05:52:08.000000 aurori-1.1.0/aurori/routes.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.102291 aurori-1.1.0/aurori/types/
--rw-rw-rw-   0        0        0      926 2022-08-05 14:12:46.000000 aurori-1.1.0/aurori/types/exceptions.py
--rw-rw-rw-   0        0        0     1567 2022-08-05 14:12:46.000000 aurori-1.1.0/aurori/types/intEnum.py
--rw-rw-rw-   0        0        0     1499 2022-08-05 14:12:46.000000 aurori-1.1.0/aurori/types/intFlag.py
--rw-rw-rw-   0        0        0     1437 2023-08-04 12:17:07.000000 aurori-1.1.0/aurori/types/jsonDict.py
--rw-rw-rw-   0        0        0     1579 2022-08-05 14:12:46.000000 aurori-1.1.0/aurori/types/objDict.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.131291 aurori-1.1.0/aurori/users/
--rw-rw-rw-   0        0        0     1036 2023-07-27 10:31:03.000000 aurori-1.1.0/aurori/users/__init__.py
--rw-rw-rw-   0        0        0     4896 2023-07-28 06:29:13.000000 aurori-1.1.0/aurori/users/basemodels.py
--rw-rw-rw-   0        0        0     1116 2023-07-17 21:05:05.000000 aurori-1.1.0/aurori/users/defaultmodels.py
--rw-rw-rw-   0        0        0     2083 2023-07-27 11:58:38.000000 aurori-1.1.0/aurori/users/dependencies.py
--rw-rw-rw-   0        0        0     2920 2023-07-27 13:53:11.000000 aurori-1.1.0/aurori/users/routes.py
--rw-rw-rw-   0        0        0      165 2023-07-27 13:52:21.000000 aurori-1.1.0/aurori/users/typemodels.py
--rw-rw-rw-   0        0        0     5437 2023-07-27 14:51:50.000000 aurori-1.1.0/aurori/users/userManager.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.153294 aurori-1.1.0/aurori/utils/
--rw-rw-rw-   0        0        0      879 2023-07-18 07:32:21.000000 aurori-1.1.0/aurori/utils/__init__.py
--rw-rw-rw-   0        0        0      183 2023-07-17 20:48:28.000000 aurori-1.1.0/aurori/utils/converter.py
--rw-rw-rw-   0        0        0     1193 2023-08-07 08:21:11.000000 aurori-1.1.0/aurori/version.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.208290 aurori-1.1.0/aurori/workspaces/
--rw-rw-rw-   0        0        0     1136 2023-07-27 06:56:41.000000 aurori-1.1.0/aurori/workspaces/__init__.py
--rw-rw-rw-   0        0        0     2707 2023-07-26 14:56:10.000000 aurori-1.1.0/aurori/workspaces/models.py
--rw-rw-rw-   0        0        0     1728 2022-08-05 14:12:46.000000 aurori-1.1.0/aurori/workspaces/page.py
--rw-rw-rw-   0        0        0     1056 2022-08-05 14:12:46.000000 aurori-1.1.0/aurori/workspaces/permission.py
--rw-rw-rw-   0        0        0      884 2023-07-17 04:48:54.000000 aurori-1.1.0/aurori/workspaces/routes.py
--rw-rw-rw-   0        0        0    18907 2023-08-04 12:00:40.000000 aurori-1.1.0/aurori/workspaces/workspace.py
--rw-rw-rw-   0        0        0    13495 2023-07-27 07:35:51.000000 aurori-1.1.0/aurori/workspaces/workspaceManager.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:44.966290 aurori-1.1.0/aurori.egg-info/
--rw-rw-rw-   0        0        0      594 2023-08-07 08:21:44.000000 aurori-1.1.0/aurori.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1754 2023-08-07 08:21:44.000000 aurori-1.1.0/aurori.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 08:21:44.000000 aurori-1.1.0/aurori.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-08-07 08:21:44.000000 aurori-1.1.0/aurori.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      158 2023-08-07 08:21:44.000000 aurori-1.1.0/aurori.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-07 08:21:44.000000 aurori-1.1.0/aurori.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4119 2022-08-04 21:04:02.000000 aurori-1.1.0/aurori_icon.inkscape.svg
--rw-rw-rw-   0        0        0     9474 2022-08-04 21:10:24.000000 aurori-1.1.0/aurori_logo.inkscape.svg
--rw-rw-rw-   0        0        0      563 2023-07-27 09:48:20.000000 aurori-1.1.0/config.ini.template
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.215292 aurori-1.1.0/dist/
--rw-rw-rw-   0        0        0      199 2023-08-04 09:18:47.000000 aurori-1.1.0/dist/DEPLOY.md
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.217292 aurori-1.1.0/examples/
--rw-rw-rw-   0        0        0        4 2022-09-02 13:45:54.000000 aurori-1.1.0/examples/.gitignore
--rw-rw-rw-   0        0        0     1439 2023-08-04 09:23:44.000000 aurori-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      184 2023-07-27 10:10:03.000000 aurori-1.1.0/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.228291 aurori-1.1.0/scripts/
--rw-rw-rw-   0        0        0     2439 2022-08-05 14:12:46.000000 aurori-1.1.0/scripts/quality_report.py
--rw-rw-rw-   0        0        0      516 2023-08-07 08:21:45.289291 aurori-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-07-28 09:17:51.000000 aurori-1.1.0/setup.py
--rw-rw-rw-   0        0        0       88 2022-07-26 22:13:52.000000 aurori-1.1.0/test.py
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:44.787293 aurori-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2023-08-07 08:21:45.281292 aurori-1.1.0/tests/api_test/
--rw-rw-rw-   0        0        0       80 2021-08-24 16:09:25.000000 aurori-1.1.0/tests/api_test/action.req
--rw-rw-rw-   0        0        0     2117 2022-07-26 21:50:23.000000 aurori-1.1.0/tests/api_test/action_test.py
--rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-1.1.0/tests/api_test/dashboard.req
--rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-1.1.0/tests/api_test/login.req
--rw-rw-rw-   0        0        0      135 2021-08-24 16:09:25.000000 aurori-1.1.0/tests/api_test/refresh.req
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.948515 aurori-1.1.1/
+-rw-rw-rw-   0        0        0      100 2023-07-17 04:28:08.000000 aurori-1.1.1/.gitignore
+-rw-rw-rw-   0        0        0     1575 2022-07-26 21:50:23.000000 aurori-1.1.1/.gitlab-ci.yml
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.787513 aurori-1.1.1/.vscode/
+-rw-rw-rw-   0        0        0      986 2022-07-28 10:26:45.000000 aurori-1.1.1/.vscode/launch.json
+-rw-rw-rw-   0        0        0    35005 2022-08-05 13:57:15.000000 aurori-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      594 2023-08-07 10:11:12.949515 aurori-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-08-04 09:25:19.000000 aurori-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.800515 aurori-1.1.1/aurori/
+-rw-rw-rw-   0        0        0    35005 2022-08-05 07:33:15.000000 aurori-1.1.1/aurori/LICENSE.md
+-rw-rw-rw-   0        0        0       54 2023-08-04 09:25:21.000000 aurori-1.1.1/aurori/README.md
+-rw-rw-rw-   0        0        0     2847 2023-08-07 09:57:29.000000 aurori-1.1.1/aurori/__init__.py
+-rw-rw-rw-   0        0        0     2049 2022-01-25 10:07:21.000000 aurori-1.1.1/aurori/alembic.ini
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.852516 aurori-1.1.1/aurori/api/
+-rw-rw-rw-   0        0        0       33 2023-07-27 08:48:58.000000 aurori-1.1.1/aurori/api/__init__.py
+-rw-rw-rw-   0        0        0      259 2023-07-27 11:58:48.000000 aurori-1.1.1/aurori/api/dependencies.py
+-rw-rw-rw-   0        0        0       56 2023-07-27 10:07:47.000000 aurori-1.1.1/aurori/api/security.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.856515 aurori-1.1.1/aurori/cli/
+-rw-rw-rw-   0        0        0      154 2023-07-27 15:09:45.000000 aurori-1.1.1/aurori/cli/__init__.py
+-rw-rw-rw-   0        0        0      216 2023-07-27 15:11:13.000000 aurori-1.1.1/aurori/cli/core.py
+-rw-rw-rw-   0        0        0     5204 2023-07-18 07:21:56.000000 aurori-1.1.1/aurori/config.py
+-rw-rw-rw-   0        0        0      909 2023-07-28 05:43:43.000000 aurori-1.1.1/aurori/database.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.865516 aurori-1.1.1/aurori/jobs/
+-rw-rw-rw-   0        0        0     2648 2023-08-07 08:07:10.000000 aurori-1.1.1/aurori/jobs/__init__.py
+-rw-rw-rw-   0        0        0     7649 2023-08-07 08:16:08.000000 aurori-1.1.1/aurori/jobs/job.py
+-rw-rw-rw-   0        0        0     7119 2023-08-07 08:08:07.000000 aurori-1.1.1/aurori/jobs/jobManager.py
+-rw-rw-rw-   0        0        0     1727 2023-08-04 12:16:14.000000 aurori-1.1.1/aurori/jobs/models.py
+-rw-rw-rw-   0        0        0     1105 2023-07-27 06:50:14.000000 aurori-1.1.1/aurori/jobs/routes.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.872514 aurori-1.1.1/aurori/logs/
+-rw-rw-rw-   0        0        0     1005 2023-07-27 15:29:46.000000 aurori-1.1.1/aurori/logs/__init__.py
+-rw-rw-rw-   0        0        0     4899 2023-07-28 06:12:36.000000 aurori-1.1.1/aurori/logs/logManager.py
+-rw-rw-rw-   0        0        0     3605 2023-07-28 06:10:15.000000 aurori-1.1.1/aurori/logs/logger.py
+-rw-rw-rw-   0        0        0     1064 2023-07-17 04:33:39.000000 aurori-1.1.1/aurori/logs/routes.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.877514 aurori-1.1.1/aurori/migrations/
+-rw-rw-rw-   0        0        0      323 2022-02-22 10:25:17.000000 aurori-1.1.1/aurori/migrations/README.md
+-rw-rw-rw-   0        0        0     4804 2022-08-04 21:24:37.000000 aurori-1.1.1/aurori/migrations/env.py
+-rw-rw-rw-   0        0        0      518 2022-01-25 10:07:21.000000 aurori-1.1.1/aurori/migrations/script.py.mako
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.881515 aurori-1.1.1/aurori/pages/
+-rw-rw-rw-   0        0        0      936 2023-07-27 08:21:25.000000 aurori-1.1.1/aurori/pages/__init__.py
+-rw-rw-rw-   0        0        0     5500 2023-07-27 08:16:14.000000 aurori-1.1.1/aurori/pages/menuBuilder.py
+-rw-rw-rw-   0        0        0     1256 2023-07-18 05:52:08.000000 aurori-1.1.1/aurori/routes.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.889513 aurori-1.1.1/aurori/types/
+-rw-rw-rw-   0        0        0      926 2022-08-05 14:12:46.000000 aurori-1.1.1/aurori/types/exceptions.py
+-rw-rw-rw-   0        0        0     1567 2022-08-05 14:12:46.000000 aurori-1.1.1/aurori/types/intEnum.py
+-rw-rw-rw-   0        0        0     1499 2022-08-05 14:12:46.000000 aurori-1.1.1/aurori/types/intFlag.py
+-rw-rw-rw-   0        0        0     1437 2023-08-04 12:17:07.000000 aurori-1.1.1/aurori/types/jsonDict.py
+-rw-rw-rw-   0        0        0     1579 2022-08-05 14:12:46.000000 aurori-1.1.1/aurori/types/objDict.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.900513 aurori-1.1.1/aurori/users/
+-rw-rw-rw-   0        0        0     1036 2023-07-27 10:31:03.000000 aurori-1.1.1/aurori/users/__init__.py
+-rw-rw-rw-   0        0        0     4896 2023-07-28 06:29:13.000000 aurori-1.1.1/aurori/users/basemodels.py
+-rw-rw-rw-   0        0        0     1116 2023-07-17 21:05:05.000000 aurori-1.1.1/aurori/users/defaultmodels.py
+-rw-rw-rw-   0        0        0     2083 2023-07-27 11:58:38.000000 aurori-1.1.1/aurori/users/dependencies.py
+-rw-rw-rw-   0        0        0     2920 2023-07-27 13:53:11.000000 aurori-1.1.1/aurori/users/routes.py
+-rw-rw-rw-   0        0        0      165 2023-07-27 13:52:21.000000 aurori-1.1.1/aurori/users/typemodels.py
+-rw-rw-rw-   0        0        0     5437 2023-07-27 14:51:50.000000 aurori-1.1.1/aurori/users/userManager.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.903512 aurori-1.1.1/aurori/utils/
+-rw-rw-rw-   0        0        0      879 2023-07-18 07:32:21.000000 aurori-1.1.1/aurori/utils/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-07-17 20:48:28.000000 aurori-1.1.1/aurori/utils/converter.py
+-rw-rw-rw-   0        0        0     1193 2023-08-07 10:10:39.000000 aurori-1.1.1/aurori/version.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.916516 aurori-1.1.1/aurori/workspaces/
+-rw-rw-rw-   0        0        0     1136 2023-07-27 06:56:41.000000 aurori-1.1.1/aurori/workspaces/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-07-26 14:56:10.000000 aurori-1.1.1/aurori/workspaces/models.py
+-rw-rw-rw-   0        0        0     1728 2022-08-05 14:12:46.000000 aurori-1.1.1/aurori/workspaces/page.py
+-rw-rw-rw-   0        0        0     1056 2022-08-05 14:12:46.000000 aurori-1.1.1/aurori/workspaces/permission.py
+-rw-rw-rw-   0        0        0      884 2023-07-17 04:48:54.000000 aurori-1.1.1/aurori/workspaces/routes.py
+-rw-rw-rw-   0        0        0    18885 2023-08-07 10:01:33.000000 aurori-1.1.1/aurori/workspaces/workspace.py
+-rw-rw-rw-   0        0        0    13478 2023-08-07 09:57:05.000000 aurori-1.1.1/aurori/workspaces/workspaceManager.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.845513 aurori-1.1.1/aurori.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-08-07 10:11:12.000000 aurori-1.1.1/aurori.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2023-08-07 10:11:12.000000 aurori-1.1.1/aurori.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 10:11:12.000000 aurori-1.1.1/aurori.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-08-07 10:11:12.000000 aurori-1.1.1/aurori.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      158 2023-08-07 10:11:12.000000 aurori-1.1.1/aurori.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-07 10:11:12.000000 aurori-1.1.1/aurori.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4119 2022-08-04 21:04:02.000000 aurori-1.1.1/aurori_icon.inkscape.svg
+-rw-rw-rw-   0        0        0     9474 2022-08-04 21:10:24.000000 aurori-1.1.1/aurori_logo.inkscape.svg
+-rw-rw-rw-   0        0        0      563 2023-07-27 09:48:20.000000 aurori-1.1.1/config.ini.template
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.917514 aurori-1.1.1/dist/
+-rw-rw-rw-   0        0        0      199 2023-08-07 10:11:05.000000 aurori-1.1.1/dist/DEPLOY.md
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.919513 aurori-1.1.1/examples/
+-rw-rw-rw-   0        0        0        4 2022-09-02 13:45:54.000000 aurori-1.1.1/examples/.gitignore
+-rw-rw-rw-   0        0        0     1439 2023-08-04 09:23:44.000000 aurori-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      184 2023-07-27 10:10:03.000000 aurori-1.1.1/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.922515 aurori-1.1.1/scripts/
+-rw-rw-rw-   0        0        0     2439 2022-08-05 14:12:46.000000 aurori-1.1.1/scripts/quality_report.py
+-rw-rw-rw-   0        0        0      516 2023-08-07 10:11:12.963515 aurori-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-07-28 09:17:51.000000 aurori-1.1.1/setup.py
+-rw-rw-rw-   0        0        0       88 2022-07-26 22:13:52.000000 aurori-1.1.1/test.py
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.765514 aurori-1.1.1/tests/
+drwxrwxrwx   0        0        0        0 2023-08-07 10:11:12.939514 aurori-1.1.1/tests/api_test/
+-rw-rw-rw-   0        0        0       80 2021-08-24 16:09:25.000000 aurori-1.1.1/tests/api_test/action.req
+-rw-rw-rw-   0        0        0     2117 2022-07-26 21:50:23.000000 aurori-1.1.1/tests/api_test/action_test.py
+-rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-1.1.1/tests/api_test/dashboard.req
+-rw-rw-rw-   0        0        0      130 2021-08-24 16:09:25.000000 aurori-1.1.1/tests/api_test/login.req
+-rw-rw-rw-   0        0        0      135 2021-08-24 16:09:25.000000 aurori-1.1.1/tests/api_test/refresh.req
```

### Comparing `aurori-1.1.0/.gitlab-ci.yml` & `aurori-1.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/.vscode/launch.json` & `aurori-1.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/LICENSE` & `aurori-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/PKG-INFO` & `aurori-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurori
-Version: 1.1.0
+Version: 1.1.1
 Summary: A flexible web framework based on FastApi.
 License: AGPLv3+
 Project-URL: Homepage, https://gitlab.com/aurori/aurori
 Project-URL: Bug Tracker, https://gitlab.com/aurori/aurori/-/issues
 Keywords: aurori
 Classifier: Framework :: FastAPI
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aurori-1.1.0/aurori/LICENSE.md` & `aurori-1.1.1/aurori/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/__init__.py` & `aurori-1.1.1/aurori/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from aurori.database import db, SQLModelBase
 from aurori.utils import unicode_string_to_bytes
 from aurori.pages import menu_builder
 
 __version__ = version
 
 
-def create_app(config, fastapi_config=None, minimal=False, api_prefix="/api/v1", title="Aurori App", version="0.1.0"):
+def create_app(config, fastapi_config=None, minimal=False, api_prefix="", title="Aurori App", version="0.1.0"):
     config_manager.init_manager(config, fastapi_config)
     app = FastAPI(title=title, version=version)
 
     db.init_app(config)
 
     from aurori import app_router
     app.include_router(app_router, tags=["Core"])
```

### Comparing `aurori-1.1.0/aurori/alembic.ini` & `aurori-1.1.1/aurori/alembic.ini`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/config.py` & `aurori-1.1.1/aurori/config.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/database.py` & `aurori-1.1.1/aurori/database.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/jobs/__init__.py` & `aurori-1.1.1/aurori/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/jobs/job.py` & `aurori-1.1.1/aurori/jobs/job.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/jobs/jobManager.py` & `aurori-1.1.1/aurori/jobs/jobManager.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/jobs/models.py` & `aurori-1.1.1/aurori/jobs/models.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/jobs/routes.py` & `aurori-1.1.1/aurori/jobs/routes.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/logs/__init__.py` & `aurori-1.1.1/aurori/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/logs/logManager.py` & `aurori-1.1.1/aurori/logs/logManager.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/logs/logger.py` & `aurori-1.1.1/aurori/logs/logger.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/logs/routes.py` & `aurori-1.1.1/aurori/logs/routes.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/migrations/env.py` & `aurori-1.1.1/aurori/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/migrations/script.py.mako` & `aurori-1.1.1/aurori/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/pages/__init__.py` & `aurori-1.1.1/aurori/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/pages/menuBuilder.py` & `aurori-1.1.1/aurori/pages/menuBuilder.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/routes.py` & `aurori-1.1.1/aurori/routes.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/types/exceptions.py` & `aurori-1.1.1/aurori/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/types/intEnum.py` & `aurori-1.1.1/aurori/types/intEnum.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/types/intFlag.py` & `aurori-1.1.1/aurori/types/intFlag.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/types/jsonDict.py` & `aurori-1.1.1/aurori/types/jsonDict.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/types/objDict.py` & `aurori-1.1.1/aurori/types/objDict.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/users/__init__.py` & `aurori-1.1.1/aurori/users/__init__.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/users/basemodels.py` & `aurori-1.1.1/aurori/users/basemodels.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/users/defaultmodels.py` & `aurori-1.1.1/aurori/users/defaultmodels.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/users/dependencies.py` & `aurori-1.1.1/aurori/users/dependencies.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/users/routes.py` & `aurori-1.1.1/aurori/users/routes.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/users/userManager.py` & `aurori-1.1.1/aurori/users/userManager.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/utils/__init__.py` & `aurori-1.1.1/aurori/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/version.py` & `aurori-1.1.1/aurori/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 __authors__ = ["Marcus Drobisch"]
 __contact__ = "aurori@fabba.space"
 __credits__ = []
 __license__ = "AGPLv3+"
 
 import subprocess
 
-version = "1.1.0"
+version = "1.1.1"
 # WARNING: will be overwritten by CI, see docker/.gitlab-ci.yml
 # try:
 #    label = subprocess.check_output(["git", "describe"]).strip()
 #    version = label.decode(encoding='UTF-8')
 # except Exception as e:
 #    print("Unable to get version", e)
 # WARNING: will be overwritten by CI, see docker/.gitlab-ci.yml
```

### Comparing `aurori-1.1.0/aurori/workspaces/__init__.py` & `aurori-1.1.1/aurori/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/workspaces/models.py` & `aurori-1.1.1/aurori/workspaces/models.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/workspaces/page.py` & `aurori-1.1.1/aurori/workspaces/page.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/workspaces/permission.py` & `aurori-1.1.1/aurori/workspaces/permission.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/workspaces/routes.py` & `aurori-1.1.1/aurori/workspaces/routes.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori/workspaces/workspace.py` & `aurori-1.1.1/aurori/workspaces/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 for (_, c) in clsmembers:
                     if issubclass(c, Job) & (c is not Job):
                         if c.disable is False:
                             logManager.info(
                                 f'    Job registered from "{c.__module__}"')
                             jobManager.register_job(self, c, True)
 
-    def discover_apis(self, workspace_source_path, api_prefix):
+    def discover_apis(self, workspace_source_path):
         api_workspace_path = workspace_source_path + '.' + self.name + '.api'
         api_source = __import__(api_workspace_path, fromlist=['blah'])
         for _, modulename, ispkg in pkgutil.iter_modules(
                 api_source.__path__, api_source.__name__ + '.'):
             if not ispkg:
                 api_module = __import__(modulename,
                                                fromlist=['blah'])
@@ -112,15 +112,15 @@
                     if isinstance(c, APIRouter):
                         logManager.info(
                             f'    API "{api_name}" loaded from "{modulename}"'
                         )
                         if c.prefix != "":
                             self.app.include_router(c, tags=["App." + self.name])
                         else:
-                            self.app.include_router(c,prefix=api_prefix+"/" + self.uri, tags=["App." + self.name])
+                            self.app.include_router(c,prefix= "/" + self.uri, tags=["App." + self.name])
 
 
     def discover_permissions(self, workspace_source):
         permissionsSource = workspace_source + '.' + self.name
         imported_source = __import__(permissionsSource, fromlist=['blah'])
 
         for _, permissionname, ispkg in pkgutil.iter_modules(
```

### Comparing `aurori-1.1.0/aurori/workspaces/workspaceManager.py` & `aurori-1.1.1/aurori/workspaces/workspaceManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
         for w in self.workspaces:
             logManager.info(f'  For workspace: "{w.name}"')
             workspace_config_section_name = pathlib.Path(
                 w.path).resolve().name.upper()
             
             try:
-                w.discover_apis(self.workspace_source_path, self.api_prefix)
+                w.discover_apis(self.workspace_source_path)
             except Exception as exception:
                 traceback.print_exc(file=sys.stdout)
                 logManager.error(
                     f'  Workspace "{w.name}" unable to apis pages  ({str(type(exception).__name__)}:{exception})'
                 )
                 
     def discover_models(self):
```

### Comparing `aurori-1.1.0/aurori.egg-info/PKG-INFO` & `aurori-1.1.1/aurori.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurori
-Version: 1.1.0
+Version: 1.1.1
 Summary: A flexible web framework based on FastApi.
 License: AGPLv3+
 Project-URL: Homepage, https://gitlab.com/aurori/aurori
 Project-URL: Bug Tracker, https://gitlab.com/aurori/aurori/-/issues
 Keywords: aurori
 Classifier: Framework :: FastAPI
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aurori-1.1.0/aurori.egg-info/SOURCES.txt` & `aurori-1.1.1/aurori.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori_icon.inkscape.svg` & `aurori-1.1.1/aurori_icon.inkscape.svg`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/aurori_logo.inkscape.svg` & `aurori-1.1.1/aurori_logo.inkscape.svg`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/config.ini.template` & `aurori-1.1.1/config.ini.template`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/pyproject.toml` & `aurori-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/scripts/quality_report.py` & `aurori-1.1.1/scripts/quality_report.py`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/setup.cfg` & `aurori-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aurori-1.1.0/tests/api_test/action_test.py` & `aurori-1.1.1/tests/api_test/action_test.py`

 * *Files identical despite different names*

