# Comparing `tmp/spai-2023.8.7.post2.tar.gz` & `tmp/spai-2023.8.7.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.8.7.post2.tar", max compression
+gzip compressed data, was "spai-2023.8.7.post3.tar", max compression
```

## Comparing `spai-2023.8.7.post2.tar` & `spai-2023.8.7.post3.tar`

### file list

```diff
@@ -1,89 +1,73 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.8.7.post2/README.md
--rw-r--r--   0        0        0      508 2023-08-07 10:44:23.432139 spai-2023.8.7.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.8.7.post2/spai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.8.7.post2/spai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.8.7.post2/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.8.7.post2/spai/cli/commands/auth.py
--rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.8.7.post2/spai/cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.8.7.post2/spai/cli/src/errors/auth.py
--rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.8.7.post2/spai/cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.8.7.post2/spai/cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.8.7.post2/spai/cli/src/repos/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.8.7.post2/spai/cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      364 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.8.7.post2/spai/cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.8.7.post2/spai/cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.8.7.post2/spai/cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.8.7.post2/spai/cli/src/usecases/project/GetLogs.py
--rw-r--r--   0        0        0      669 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/GetServices.py
--rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.8.7.post2/spai/cli/src/usecases/project/RunService.py
--rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.8.7.post2/spai/cli/src/usecases/project/ScheduleService.py
--rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.8.7.post2/spai/cli/src/usecases/project/StopService.py
--rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.8.7.post2/spai/cli/src/usecases/project/__init__.py
--rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.8.7.post2/spai/cli/src/usecases/project/init_project.py
--rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.8.7.post2/spai/cli/src/usecases/project/main.py
--rw-r--r--   0        0        0     5617 2023-07-17 09:12:37.329759 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/README.md
--rw-r--r--   0        0        0      860 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       20 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1798 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       72 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0     5617 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/README.md
--rw-r--r--   0        0        0      860 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/apis/analytics/main.py
--rw-r--r--   0        0        0       20 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1798 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/apis/xyz/main.py
--rw-r--r--   0        0        0       72 2023-08-07 10:35:32.102270 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   780104 2023-08-07 10:35:32.106269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   479926 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       31 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0       54 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1083 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/downloader/main.py
--rw-r--r--   0        0        0       64 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      524 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/ndvi/main.py
--rw-r--r--   0        0        0       30 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/ndvi/requirements.txt
--rw-r--r--   0        0        0      941 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/spai.config.yml
--rw-r--r--   0        0        0     1689 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/uis/map/main.py
--rw-r--r--   0        0        0       23 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/uis/map/requirements.txt
--rw-r--r--   0        0        0   780104 2023-07-17 09:12:37.333760 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   479926 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       31 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0       54 2023-07-17 09:12:37.329759 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1083 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       64 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      524 2023-07-17 09:12:37.329759 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0       30 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/scripts/ndvi/requirements.txt
--rw-r--r--   0        0        0      941 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/spai.config.yml
--rw-r--r--   0        0        0     1689 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.8.7.post2/spai/cli/src/usecases/run/__init__.py
--rw-r--r--   0        0        0     3646 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/run/cloud.py
--rw-r--r--   0        0        0     3458 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/run/local.py
--rw-r--r--   0        0        0     3780 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/cli/src/usecases/run/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.8.7.post2/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.8.7.post2/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1188 2023-08-07 10:35:32.110269 spai-2023.8.7.post2/spai/data/satellite/download.py
--rw-r--r--   0        0        0      647 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3448 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2538 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.8.7.post2/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     6112 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.8.7.post2/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.8.7.post2/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.8.7.post2/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.8.7.post2/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.8.7.post2/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.8.7.post2/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     2298 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/main.py
--rw-r--r--   0        0        0        0 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/pulses/__init__.py
--rw-r--r--   0        0        0       41 2023-08-07 10:35:32.114270 spai-2023.8.7.post2/spai/pulses/forest-monitoring.py
--rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.8.7.post2/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.8.7.post2/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.8.7.post2/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.8.7.post2/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.8.7.post2/spai/storage/minio.py
--rw-r--r--   0        0        0     2287 1970-01-01 00:00:00.000000 spai-2023.8.7.post2/setup.py
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 spai-2023.8.7.post2/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.8.7.post3/README.md
+-rw-r--r--   0        0        0      508 2023-08-07 10:52:17.609773 spai-2023.8.7.post3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.8.7.post3/spai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.8.7.post3/spai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.8.7.post3/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.8.7.post3/spai/cli/commands/auth.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.8.7.post3/spai/cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.8.7.post3/spai/cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.8.7.post3/spai/cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.8.7.post3/spai/cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.8.7.post3/spai/cli/src/repos/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.8.7.post3/spai/cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      364 2023-08-07 10:35:32.102270 spai-2023.8.7.post3/spai/cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.8.7.post3/spai/cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.8.7.post3/spai/cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.8.7.post3/spai/cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.8.7.post3/spai/cli/src/usecases/project/GetLogs.py
+-rw-r--r--   0        0        0      669 2023-08-07 10:35:32.102270 spai-2023.8.7.post3/spai/cli/src/usecases/project/GetServices.py
+-rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.8.7.post3/spai/cli/src/usecases/project/RunService.py
+-rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.8.7.post3/spai/cli/src/usecases/project/ScheduleService.py
+-rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.8.7.post3/spai/cli/src/usecases/project/StopService.py
+-rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.8.7.post3/spai/cli/src/usecases/project/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.8.7.post3/spai/cli/src/usecases/project/init_project.py
+-rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.8.7.post3/spai/cli/src/usecases/project/main.py
+-rw-r--r--   0        0        0     5617 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/README.md
+-rw-r--r--   0        0        0      860 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0       20 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/apis/analytics/requirements.txt
+-rw-r--r--   0        0        0     1798 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0       72 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/apis/xyz/requirements.txt
+-rw-r--r--   0        0        0   780104 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   479926 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0       31 2023-08-07 10:51:44.517658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/notebooks/analytics/requirements.txt
+-rw-r--r--   0        0        0       54 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
+-rw-r--r--   0        0        0     1083 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0       64 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/downloader/requirements.txt
+-rw-r--r--   0        0        0      524 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0       30 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/ndvi/requirements.txt
+-rw-r--r--   0        0        0      941 2023-08-07 10:51:44.509658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1689 2023-08-07 10:51:44.589658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0       23 2023-08-07 10:51:44.589658 spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/uis/map/requirements.txt
+-rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.8.7.post3/spai/cli/src/usecases/run/__init__.py
+-rw-r--r--   0        0        0     3646 2023-08-07 10:35:32.110269 spai-2023.8.7.post3/spai/cli/src/usecases/run/cloud.py
+-rw-r--r--   0        0        0     3458 2023-08-07 10:35:32.110269 spai-2023.8.7.post3/spai/cli/src/usecases/run/local.py
+-rw-r--r--   0        0        0     3780 2023-08-07 10:35:32.110269 spai-2023.8.7.post3/spai/cli/src/usecases/run/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.8.7.post3/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.8.7.post3/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1188 2023-08-07 10:35:32.110269 spai-2023.8.7.post3/spai/data/satellite/download.py
+-rw-r--r--   0        0        0      647 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3448 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2538 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1264 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.8.7.post3/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0     6112 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/data/satellite/utils.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.8.7.post3/spai/image/__init__.py
+-rw-r--r--   0        0        0     1350 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.8.7.post3/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.8.7.post3/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.8.7.post3/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.8.7.post3/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.8.7.post3/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     2298 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/main.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/pulses/__init__.py
+-rw-r--r--   0        0        0       41 2023-08-07 10:35:32.114270 spai-2023.8.7.post3/spai/pulses/forest-monitoring.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.8.7.post3/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.8.7.post3/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.8.7.post3/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.8.7.post3/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.8.7.post3/spai/storage/minio.py
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 spai-2023.8.7.post3/setup.py
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 spai-2023.8.7.post3/PKG-INFO
```

### Comparing `spai-2023.8.7.post2/spai/cli/commands/auth.py` & `spai-2023.8.7.post3/spai/cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/repos/APIRepo.py` & `spai-2023.8.7.post3/spai/cli/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/repos/AuthRepo.py` & `spai-2023.8.7.post3/spai/cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/auth/Auth.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/auth/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/GetServices.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/GetServices.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/README.md` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/apis/analytics/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/apis/analytics/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/apis/xyz/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/apis/xyz/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/notebooks/analytics/main.ipynb` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/notebooks/analytics/output.ipynb` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/downloader/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/scripts/ndvi/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/spai.config.yml` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/spai.config.yml`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/project/project-template/getting-started/uis/map/main.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/project/project-template/uis/map/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/run/cloud.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/run/cloud.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/run/local.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/run/local.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/cli/src/usecases/run/validate.py` & `spai-2023.8.7.post3/spai/cli/src/usecases/run/validate.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/download.py` & `spai-2023.8.7.post3/spai/data/satellite/download.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/explore.py` & `spai-2023.8.7.post3/spai/data/satellite/explore.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.8.7.post3/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/data/satellite/utils.py` & `spai-2023.8.7.post3/spai/data/satellite/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/image/utils.py` & `spai-2023.8.7.post3/spai/image/utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/image/xyz/cache.py` & `spai-2023.8.7.post3/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/image/xyz/errors.py` & `spai-2023.8.7.post3/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/image/xyz/get_image_tile.py` & `spai-2023.8.7.post3/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/image/xyz/image_utils.py` & `spai-2023.8.7.post3/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/main.py` & `spai-2023.8.7.post3/spai/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/storage/BaseStorage.py` & `spai-2023.8.7.post3/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/storage/CloudStorage.py` & `spai-2023.8.7.post3/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/storage/Storage.py` & `spai-2023.8.7.post3/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/spai/storage/minio.py` & `spai-2023.8.7.post3/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.8.7.post2/setup.py` & `spai-2023.8.7.post3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,19 +7,14 @@
  'spai.cli.commands',
  'spai.cli.src.errors',
  'spai.cli.src.repos',
  'spai.cli.src.usecases.auth',
  'spai.cli.src.usecases.project',
  'spai.cli.src.usecases.project.project-template.apis.analytics',
  'spai.cli.src.usecases.project.project-template.apis.xyz',
- 'spai.cli.src.usecases.project.project-template.getting-started.apis.analytics',
- 'spai.cli.src.usecases.project.project-template.getting-started.apis.xyz',
- 'spai.cli.src.usecases.project.project-template.getting-started.scripts.downloader',
- 'spai.cli.src.usecases.project.project-template.getting-started.scripts.ndvi',
- 'spai.cli.src.usecases.project.project-template.getting-started.uis.map',
  'spai.cli.src.usecases.project.project-template.scripts.downloader',
  'spai.cli.src.usecases.project.project-template.scripts.ndvi',
  'spai.cli.src.usecases.project.project-template.uis.map',
  'spai.cli.src.usecases.run',
  'spai.data',
  'spai.data.satellite',
  'spai.data.satellite.sentinelhub',
@@ -27,16 +22,14 @@
  'spai.image.xyz',
  'spai.pulses',
  'spai.storage']
 
 package_data = \
 {'': ['*'],
  'spai.cli.src.usecases.project': ['project-template/*',
-                                   'project-template/getting-started/*',
-                                   'project-template/getting-started/notebooks/analytics/*',
                                    'project-template/notebooks/analytics/*']}
 
 install_requires = \
 ['PyJWT>=2.7.0,<3.0.0',
  'PyYAML>=6.0.0,<7.0.0',
  'minio>=7.1.15,<8.0.0',
  'overpy>=0.6,<0.7',
@@ -47,15 +40,15 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.8.7.post2',
+    'version': '2023.8.7.post3',
     'description': '',
     'long_description': '# SPAI CLI\n\n## Create new project\n\n```bash\nspai init\n```\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spai-2023.8.7.post2/PKG-INFO` & `spai-2023.8.7.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2023.8.7.post2
+Version: 2023.8.7.post3
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

