# Comparing `tmp/edc-0.5.8.tar.gz` & `tmp/edc-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.5.8.tar", last modified: Tue Jul 18 02:12:34 2023, max compression
+gzip compressed data, was "edc-0.5.9.tar", last modified: Thu Jul 20 02:51:26 2023, max compression
```

## Comparing `edc-0.5.8.tar` & `edc-0.5.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.871976 edc-0.5.8/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    42968 2023-07-18 02:12:25.000000 edc-0.5.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-18 02:12:34.872106 edc-0.5.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37646 2023-07-12 23:55:42.000000 edc-0.5.8/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.858391 edc-0.5.8/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.860989 edc-0.5.8/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.8/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.8/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.8/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.861816 edc-0.5.8/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.8/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.8/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.8/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.8/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.863085 edc-0.5.8/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.8/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.867430 edc-0.5.8/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.8/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.8/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.8/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.8/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.8/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.8/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.8/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.8/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.8/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.8/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.8/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.8/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.8/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.8/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.8/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.8/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.8/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.8/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.8/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.868381 edc-0.5.8/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.8/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1916 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-18 02:12:34.000000 edc-0.5.8/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.868514 edc-0.5.8/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.8/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.8/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.871418 edc-0.5.8/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.8/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.8/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.8/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.8/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.8/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.8/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.8/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.8/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.8/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.8/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.8/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2959 2023-07-18 02:12:34.872485 edc-0.5.8/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-18 02:12:34.871742 edc-0.5.8/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.8/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.8/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.717582 edc-0.5.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.5.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.5.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.5.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    43780 2023-07-20 02:51:18.000000 edc-0.5.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.5.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.5.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-20 02:51:26.717726 edc-0.5.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37646 2023-07-12 23:55:42.000000 edc-0.5.9/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.704697 edc-0.5.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.707540 edc-0.5.9/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.5.9/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.5.9/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.5.9/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.708212 edc-0.5.9/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.5.9/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.5.9/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.5.9/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.5.9/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.709308 edc-0.5.9/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.5.9/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.713077 edc-0.5.9/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.5.9/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.5.9/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.5.9/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.5.9/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.5.9/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.5.9/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.5.9/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.5.9/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.5.9/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.5.9/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.5.9/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.5.9/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.5.9/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.5.9/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.5.9/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.5.9/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.5.9/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.5.9/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.5.9/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.714023 edc-0.5.9/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38469 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.5.9/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1917 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-07-20 02:51:26.000000 edc-0.5.9/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.714126 edc-0.5.9/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.5.9/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.5.9/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.716982 edc-0.5.9/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.5.9/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.5.9/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.5.9/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.5.9/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.5.9/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.5.9/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.5.9/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.5.9/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.5.9/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.5.9/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.5.9/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2960 2023-07-20 02:51:26.718140 edc-0.5.9/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-07-20 02:51:26.717373 edc-0.5.9/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.5.9/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.5.9/utils/get_edc_requirements.py
```

### Comparing `edc-0.5.8/.gitignore` & `edc-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/.pre-commit-config.yaml` & `edc-0.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/CHANGES` & `edc-0.5.9/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Changes
 -------
 
+0.5.9
+-----
+- limit data export to the sites listed in userprofile; use protocol
+  name for zip archive `base_dir`; update modeladmin classes
+  (edc-export)
+- add func to get all sites for user (edc-sites)
+- filter data by site using sites param (edc-pdutils)
+- add unregister method for site_action_items (edc-action-item)
+- add verbose_name_plural; move ModelAdmin functionality to
+  SubjectLocatorModelAdminMixin (edc-locator)
+- add ModelAdmin mixin to remove PII/encrypted fields from changelist
+  and search for users not in PII/PII_VIEW permission groups;
+  move dashboard functionality to ModelAdminDashboardMixin.
+  (edc-model-admin)
+- add unregister method for site_prn_forms (edc-prn)
+- use `get_locator_model` instead of hardcoded locator model
+  (edc-subject-dashboard, edc-subject-model-wrappers)
+
+
 0.5.8
 -----
 - use SQLAlchemy to prepare sql text for pandas, upgrade pandas
   to latest, require SQLAlchemy (edc-pdutils)
 - typing hints (edc-pdutils, edc-export)
 - check settings before loading load_data (edc-list-data)
 - add func to get all sites for country (edc-sites)
```

### Comparing `edc-0.5.8/LICENSE` & `edc-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/PKG-INFO` & `edc-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.8
+Version: 0.5.9
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.8/README.rst` & `edc-0.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/bin/nginx/edc-uat.conf` & `edc-0.5.9/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/bin/nginx/edc.conf` & `edc-0.5.9/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/bin/scripts/dev_repos.sh` & `edc-0.5.9/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/bin/scripts/update_edc.sh` & `edc-0.5.9/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/bin/systemd/celery-uat.service` & `edc-0.5.9/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/bin/systemd/celery.service` & `edc-0.5.9/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/Makefile` & `edc-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/README.rst` & `edc-0.5.9/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/backup.rst` & `edc-0.5.9/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/celery.rst` & `edc-0.5.9/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/conda.rst` & `edc-0.5.9/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/conf.py` & `edc-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/configure_web_services.rst` & `edc-0.5.9/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/deploy_new_droplet.rst` & `edc-0.5.9/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/exporting_encrypted_data.rst` & `edc-0.5.9/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/forms_reference.md` & `edc-0.5.9/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/landing_page.rst` & `edc-0.5.9/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/make.bat` & `edc-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/prepare_database.rst` & `edc-0.5.9/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/printing.rst` & `edc-0.5.9/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/docs/update_deployment.rst` & `edc-0.5.9/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/edc.egg-info/PKG-INFO` & `edc-0.5.9/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.5.8
+Version: 0.5.9
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.5.8/edc.egg-info/SOURCES.txt` & `edc-0.5.9/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/edc.egg-info/requires.txt` & `edc-0.5.9/edc.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,77 +18,77 @@
 django-extensions
 django-logentry-admin
 django-multisite-edc==2.0.0
 django-revision==0.3.6
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
-edc-action-item==0.3.53
+edc-action-item==0.3.55
 edc-adherence==0.1.21
 edc-adverse-event==0.3.55
 edc-appointment==0.3.74
 edc-auth==0.3.63
 edc-consent==0.3.47
 edc-constants==0.3.49
 edc-crf==0.3.44
 edc-dashboard==0.3.45
 edc-data-manager==0.3.56
 edc-device==0.3.11
 edc-document-status==0.1.4
 edc-dx==0.1.20
 edc-dx-review==0.1.39
 edc-egfr==0.1.11
-edc-export==0.3.28
+edc-export==0.3.31
 edc-facility==0.3.15
 edc-fieldsets==0.3.13
 edc-form-describer==0.3.16
 edc-form-label==0.3.9
 edc-form-validators==0.3.34
 edc-glucose==0.1.30
-edc-he==0.1.8
+edc-he==0.1.9
 edc-identifier==0.3.24
 edc-lab==0.3.44
 edc-lab-dashboard==0.3.11
 edc-lab-panel==0.1.15
 edc-lab-results==0.1.38
 edc-label==0.3.13
 edc-list-data==0.3.19
 edc-listboard==0.1.11
-edc-locator==0.3.24
+edc-locator==0.3.25
 edc-ltfu==0.3.24
 edc-metadata==0.3.54
 edc-mnsi==0.1.17
 edc-model==0.3.32
-edc-model-admin==0.3.47
+edc-model-admin==0.3.48
 edc-model-fields==0.3.7
 edc-model-form==0.1.12
 edc-model-wrapper==0.3.10
 edc-navbar==0.3.16
 edc-notification==0.3.18
 edc-offstudy==0.3.33
 edc-pdf-reports==0.3.14
-edc-pdutils==0.3.23
+edc-pdutils==0.3.24
 edc-pharmacy==0.1.39
 edc-pharmacy-dashboard==0.1.3
-edc-prn==0.3.13
-edc-protocol==0.3.9
+edc-prn==0.3.14
+edc-protocol==0.3.10
 edc-protocol-incident==0.1.26
 edc-qol==0.1.15
 edc-randomization==0.3.47
 edc-reference==0.3.20
 edc-refusal==0.1.13
 edc-registration==0.3.30
 edc-reportable==0.3.31
 edc-review-dashboard==0.3.19
 edc-rx==0.1.7
 edc-screening==0.3.35
 edc-search==0.3.7
-edc-sites==0.3.26
-edc-subject-dashboard==0.3.38
-edc-subject-model-wrappers==0.3.15
+edc-sites==0.3.27
+edc-subject-dashboard==0.3.39
+edc-subject-model-wrappers==0.3.16
 edc-timepoint==0.3.11
 edc-transfer==0.3.14
 edc-unblinding==0.1.15
 edc-utils==0.3.20
 edc-visit-schedule==0.3.62
 edc-visit-tracking==0.3.53
 edc-vitals==0.1.11
```

### Comparing `edc-0.5.8/image/icon-pycharm.png` & `edc-0.5.9/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/requirements.tests/edc.txt` & `edc-0.5.9/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/requirements.tests/edc_dev.txt` & `edc-0.5.9/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.5.8/setup.cfg` & `edc-0.5.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -46,77 +46,77 @@
 	django-extensions
 	django-logentry-admin
 	django-multisite-edc==2.0.0
 	django-revision==0.3.6
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
-	edc-action-item==0.3.53
+	edc-action-item==0.3.55
 	edc-adherence==0.1.21
 	edc-adverse-event==0.3.55
 	edc-appointment==0.3.74
 	edc-auth==0.3.63
 	edc-consent==0.3.47
 	edc-constants==0.3.49
 	edc-crf==0.3.44
 	edc-dashboard==0.3.45
 	edc-data-manager==0.3.56
 	edc-device==0.3.11
 	edc-document-status==0.1.4
 	edc-dx==0.1.20
 	edc-dx-review==0.1.39
 	edc-egfr==0.1.11
-	edc-export==0.3.28
+	edc-export==0.3.31
 	edc-facility==0.3.15
 	edc-fieldsets==0.3.13
 	edc-form-describer==0.3.16
 	edc-form-label==0.3.9
 	edc-form-validators==0.3.34
 	edc-glucose==0.1.30
-	edc-he==0.1.8
+	edc-he==0.1.9
 	edc-identifier==0.3.24
 	edc-lab==0.3.44
 	edc-lab-dashboard==0.3.11
 	edc-lab-panel==0.1.15
 	edc-lab-results==0.1.38
 	edc-label==0.3.13
 	edc-list-data==0.3.19
 	edc-listboard==0.1.11
-	edc-locator==0.3.24
+	edc-locator==0.3.25
 	edc-ltfu==0.3.24
 	edc-metadata==0.3.54
 	edc-mnsi==0.1.17
 	edc-model==0.3.32
-	edc-model-admin==0.3.47
+	edc-model-admin==0.3.48
 	edc-model-fields==0.3.7
 	edc-model-form==0.1.12
 	edc-model-wrapper==0.3.10
 	edc-navbar==0.3.16
 	edc-notification==0.3.18
 	edc-offstudy==0.3.33
 	edc-pdf-reports==0.3.14
-	edc-pdutils==0.3.23
+	edc-pdutils==0.3.24
 	edc-pharmacy==0.1.39
 	edc-pharmacy-dashboard==0.1.3
-	edc-prn==0.3.13
-	edc-protocol==0.3.9
+	edc-prn==0.3.14
+	edc-protocol==0.3.10
 	edc-protocol-incident==0.1.26
 	edc-qol==0.1.15
 	edc-randomization==0.3.47
 	edc-reference==0.3.20
 	edc-refusal==0.1.13
 	edc-registration==0.3.30
 	edc-reportable==0.3.31
 	edc-review-dashboard==0.3.19
 	edc-rx==0.1.7
 	edc-screening==0.3.35
 	edc-search==0.3.7
-	edc-sites==0.3.26
-	edc-subject-dashboard==0.3.38
-	edc-subject-model-wrappers==0.3.15
+	edc-sites==0.3.27
+	edc-subject-dashboard==0.3.39
+	edc-subject-model-wrappers==0.3.16
 	edc-timepoint==0.3.11
 	edc-transfer==0.3.14
 	edc-unblinding==0.1.15
 	edc-utils==0.3.20
 	edc-visit-schedule==0.3.62
 	edc-visit-tracking==0.3.53
 	edc-vitals==0.1.11
```

### Comparing `edc-0.5.8/utils/get_edc_requirements.py` & `edc-0.5.9/utils/get_edc_requirements.py`

 * *Files identical despite different names*

