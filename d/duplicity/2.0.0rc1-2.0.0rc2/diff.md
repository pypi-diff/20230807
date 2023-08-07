# Comparing `tmp/duplicity-2.0.0rc1.tar.gz` & `tmp/duplicity-2.0.0rc2.tar.gz`

## Comparing `duplicity-2.0.0rc1.tar` & `duplicity-2.0.0rc2.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/
--rw-r--r--   0 ken       (1000) ken       (1000)   110066 2023-07-17 16:28:42.000000 duplicity-2.0.0rc1/CHANGELOG.md
--rw-r--r--   0 ken       (1000) ken       (1000)      101 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/setup.cfg
--rw-r--r--   0 ken       (1000) ken       (1000)     1390 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0 ken       (1000) ken       (1000)     2783 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/tox.ini
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/bin/
--rwxr-xr-x   0 ken       (1000) ken       (1000)     4186 2023-07-04 20:13:43.000000 duplicity-2.0.0rc1/bin/duplicity
--rw-r--r--   0 ken       (1000) ken       (1000)    97668 2023-07-17 16:38:35.000000 duplicity-2.0.0rc1/bin/duplicity.1
--rw-r--r--   0 ken       (1000) ken       (1000)      753 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/requirements.txt
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/snap/
--rw-r--r--   0 ken       (1000) ken       (1000)     4386 2023-07-17 16:38:35.000000 duplicity-2.0.0rc1/snap/snapcraft.yaml
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/snap/local/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      186 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/snap/local/debug.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      110 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/snap/local/launcher.sh
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/
--rw-r--r--   0 ken       (1000) ken       (1000)   319661 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/testfiles.tar.gz
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/unit/
--rw-r--r--   0 ken       (1000) ken       (1000)     8120 2023-07-09 16:03:55.000000 duplicity-2.0.0rc1/testing/unit/test_gpginterface.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11294 2023-07-08 15:56:58.000000 duplicity-2.0.0rc1/testing/unit/test_patchdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6077 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/unit/test_dup_time.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11572 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_lazy.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11157 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_cli_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5578 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/unit/test_statistics.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13945 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/unit/test_globmatch.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5703 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_manifest.py
--rw-r--r--   0 ken       (1000) ken       (1000)      918 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/unit/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11690 2023-07-08 16:29:35.000000 duplicity-2.0.0rc1/testing/unit/test_collections.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2447 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_dup_temp.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5402 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/unit/test_file_naming.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1178 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_tarfile.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12711 2023-07-08 19:32:57.000000 duplicity-2.0.0rc1/testing/unit/test_diffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2483 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_tempdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10385 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/unit/test_backend_instance.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2887 2023-07-08 16:58:12.000000 duplicity-2.0.0rc1/testing/unit/test_path.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1432 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_util.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8284 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/unit/test_gpg.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12151 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    65210 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/unit/test_selection.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/overrides/
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/overrides/bin/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      155 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/bin/ncftpget
--rwxr-xr-x   0 ken       (1000) ken       (1000)      512 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/bin/lftp
--rwxr-xr-x   0 ken       (1000) ken       (1000)      155 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/bin/ncftpput
--rwxr-xr-x   0 ken       (1000) ken       (1000)      423 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/bin/hsi
--rwxr-xr-x   0 ken       (1000) ken       (1000)      416 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/bin/tahoe
--rwxr-xr-x   0 ken       (1000) ken       (1000)      558 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/bin/ncftpls
--rw-r--r--   0 ken       (1000) ken       (1000)       75 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/testing/overrides/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4634 2023-07-08 15:56:58.000000 duplicity-2.0.0rc1/testing/__init__.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)      878 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/run-tests
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/functional/
--rw-r--r--   0 ken       (1000) ken       (1000)     2385 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/functional/test_log.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9537 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/functional/test_final.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1612 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/functional/test_badupload.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3287 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/functional/test_cleanup.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8328 2023-07-08 18:48:11.000000 duplicity-2.0.0rc1/testing/functional/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8640 2023-07-07 20:21:14.000000 duplicity-2.0.0rc1/testing/functional/test_verify.py
--rw-r--r--   0 ken       (1000) ken       (1000)    18677 2023-07-09 17:25:58.000000 duplicity-2.0.0rc1/testing/functional/test_restart.py
--rw-r--r--   0 ken       (1000) ken       (1000)    96829 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/functional/test_selection.py
--rw-r--r--   0 ken       (1000) ken       (1000)      941 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/testing/conftest.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3196 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/testing/test_code.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/gnupg/
--rw-r--r--   0 ken       (1000) ken       (1000)      145 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/gnupg/gpg-agent.conf
--rw-r--r--   0 ken       (1000) ken       (1000)     3567 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/gnupg/pubring.gpg
--rw-r--r--   0 ken       (1000) ken       (1000)     7549 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/gnupg/secring.gpg
--rw-r--r--   0 ken       (1000) ken       (1000)      425 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/gnupg/gpg.conf
--rw-r--r--   0 ken       (1000) ken       (1000)      255 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/gnupg/README
--rw-r--r--   0 ken       (1000) ken       (1000)     1440 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/testing/gnupg/trustdb.gpg
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/testing/regression/
--rw-r--r--   0 ken       (1000) ken       (1000)      295 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue103.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1087 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue79.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      278 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue110-test.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      457 2023-07-17 16:26:16.000000 duplicity-2.0.0rc1/testing/regression/bug930151.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      503 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/bug1526557.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1621 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue103.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1312 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue125.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      685 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue25.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      516 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/bug1919017.sh
--rw-r--r--   0 ken       (1000) ken       (1000)     8328 2023-07-11 18:07:32.000000 duplicity-2.0.0rc1/testing/regression/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)      144 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue73.env
--rwxr-xr-x   0 ken       (1000) ken       (1000)      680 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/bug1860200.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue25.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)      554 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue110-setup.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      192 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/bug1846678.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)     1001 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue98.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      417 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue100.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue79.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)      418 2023-07-11 17:46:50.000000 duplicity-2.0.0rc1/testing/regression/issue73.sh
--rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/bug1919017.json
--rwxr-xr-x   0 ken       (1000) ken       (1000)      905 2023-07-17 16:26:16.000000 duplicity-2.0.0rc1/testing/regression/bug487720.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      464 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue683.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      466 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue26.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      280 2023-07-10 19:32:00.000000 duplicity-2.0.0rc1/testing/regression/issue147.sh
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity/
--rw-r--r--   0 ken       (1000) ken       (1000)    34532 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/cli_data.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10701 2023-07-09 16:18:42.000000 duplicity-2.0.0rc1/duplicity/dup_time.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity/backends/
--rw-r--r--   0 ken       (1000) ken       (1000)     3040 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/backends/localbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16080 2023-07-09 17:15:07.000000 duplicity-2.0.0rc1/duplicity/backends/onedrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16591 2023-07-09 17:11:10.000000 duplicity-2.0.0rc1/duplicity/backends/adbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8565 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/megav2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10233 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/swiftbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4284 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/backends/rclonebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8757 2023-07-09 17:03:47.000000 duplicity-2.0.0rc1/duplicity/backends/b2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2572 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/backends/tahoebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16132 2023-07-09 16:25:43.000000 duplicity-2.0.0rc1/duplicity/backends/gdrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12971 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/ssh_pexpect_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9159 2023-07-09 17:16:51.000000 duplicity-2.0.0rc1/duplicity/backends/gdocsbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8117 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/backends/giobackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6624 2023-07-09 16:25:43.000000 duplicity-2.0.0rc1/duplicity/backends/megabackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12793 2023-07-09 17:10:30.000000 duplicity-2.0.0rc1/duplicity/backends/pydrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5652 2023-07-09 17:03:47.000000 duplicity-2.0.0rc1/duplicity/backends/azurebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1115 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/backends/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19138 2023-07-09 17:03:47.000000 duplicity-2.0.0rc1/duplicity/backends/idrivedbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15477 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/multibackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19777 2023-07-09 16:51:34.000000 duplicity-2.0.0rc1/duplicity/backends/dpbxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7103 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/backends/boxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1152 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/backends/cfbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19213 2023-07-09 17:03:47.000000 duplicity-2.0.0rc1/duplicity/backends/webdavbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10028 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/megav3backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2399 2023-07-09 16:51:34.000000 duplicity-2.0.0rc1/duplicity/backends/hubicbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9387 2023-07-09 17:03:47.000000 duplicity-2.0.0rc1/duplicity/backends/lftpbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6455 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/backends/rsyncbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5393 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/ncftpbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4719 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/duplicity/backends/mediafirebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2628 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/duplicity/backends/hsibackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8822 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/par2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19474 2023-07-09 16:44:03.000000 duplicity-2.0.0rc1/duplicity/backends/ssh_paramiko_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12468 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/pcabackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10535 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/duplicity/backends/s3_boto3_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5695 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/duplicity/backends/jottacloudbackend.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity/backends/pyrax_identity/
--rw-r--r--   0 ken       (1000) ken       (1000)     9699 2023-07-09 17:03:47.000000 duplicity-2.0.0rc1/duplicity/backends/pyrax_identity/hubic.py
--rw-r--r--   0 ken       (1000) ken       (1000)      903 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/duplicity/backends/pyrax_identity/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9732 2023-07-09 16:42:24.000000 duplicity-2.0.0rc1/duplicity/backends/imapbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3905 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/backends/_cf_cloudfiles.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5141 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/backends/_cf_pyrax.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2579 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/duplicity/backends/README
--rw-r--r--   0 ken       (1000) ken       (1000)     2310 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/backends/sxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12227 2023-07-07 20:19:43.000000 duplicity-2.0.0rc1/duplicity/backends/xorrisobackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6461 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/backends/slatebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7237 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/dup_threading.py
--rw-r--r--   0 ken       (1000) ken       (1000)    62036 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/dup_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)    26344 2023-07-09 16:18:42.000000 duplicity-2.0.0rc1/duplicity/backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10934 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/config.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7525 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/globmatch.py
--rw-r--r--   0 ken       (1000) ken       (1000)      995 2023-07-17 16:38:35.000000 duplicity-2.0.0rc1/duplicity/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8427 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/librsync.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2752 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/errors.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10624 2023-07-08 15:56:57.000000 duplicity-2.0.0rc1/duplicity/tempdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1262 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/tarfile.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13789 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/progress.py
--rw-r--r--   0 ken       (1000) ken       (1000)    17370 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/gpg.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2627 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/filechunkio.py
--rw-r--r--   0 ken       (1000) ken       (1000)    21775 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/patchdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    18003 2023-07-09 16:18:42.000000 duplicity-2.0.0rc1/duplicity/manifest.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14877 2023-07-08 19:15:08.000000 duplicity-2.0.0rc1/duplicity/file_naming.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14510 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/duplicity/_librsyncmodule.c
--rw-r--r--   0 ken       (1000) ken       (1000)    46560 2023-07-09 17:10:30.000000 duplicity-2.0.0rc1/duplicity/dup_collections.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2476 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/robust.py
--rw-r--r--   0 ken       (1000) ken       (1000)    26076 2023-07-08 15:56:57.000000 duplicity-2.0.0rc1/duplicity/diffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1668 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/cached_ops.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9893 2023-07-07 20:19:41.000000 duplicity-2.0.0rc1/duplicity/util.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8088 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/dup_temp.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12444 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/cli_util.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10093 2023-07-09 16:18:42.000000 duplicity-2.0.0rc1/duplicity/asyncscheduler.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9158 2023-07-17 16:23:33.000000 duplicity-2.0.0rc1/duplicity/cli_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12913 2023-07-09 16:03:54.000000 duplicity-2.0.0rc1/duplicity/statistics.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15046 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/lazy.py
--rw-r--r--   0 ken       (1000) ken       (1000)    28629 2023-07-07 20:19:42.000000 duplicity-2.0.0rc1/duplicity/path.py
--rw-r--r--   0 ken       (1000) ken       (1000)    28636 2023-07-09 16:25:43.000000 duplicity-2.0.0rc1/duplicity/selection.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15815 2023-07-09 16:18:42.000000 duplicity-2.0.0rc1/duplicity/log.py
--rw-r--r--   0 ken       (1000) ken       (1000)    23296 2023-07-04 20:13:41.000000 duplicity-2.0.0rc1/duplicity/gpginterface.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1284 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/README-LOG.md
--rw-rw-r--   0 ken       (1000) ken       (1000)     2360 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/PKG-INFO
--rw-r--r--   0 ken       (1000) ken       (1000)    18028 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/COPYING
--rw-r--r--   0 ken       (1000) ken       (1000)      164 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/crowdin.yml
--rw-r--r--   0 ken       (1000) ken       (1000)     3250 2023-06-30 18:00:21.000000 duplicity-2.0.0rc1/README-SNAP.md
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/
--rw-r--r--   0 ken       (1000) ken       (1000)    43776 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/fi_FI.po
--rw-r--r--   0 ken       (1000) ken       (1000)    63046 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ru_MD.po
--rw-r--r--   0 ken       (1000) ken       (1000)    58340 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/es_ES.po
--rw-r--r--   0 ken       (1000) ken       (1000)    54802 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/pt_BR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/uk_UA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32646 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/uk_UA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    45098 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/en_GB.po
--rw-r--r--   0 ken       (1000) ken       (1000)    53411 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/zh_CN.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43778 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/no_NO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/nl_NL/
--rw-rw-r--   0 ken       (1000) ken       (1000)    11565 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/nl_NL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    54884 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/it_IT.po
--rw-r--r--   0 ken       (1000) ken       (1000)    58884 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/cs_CZ.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/hu_HU/
--rw-rw-r--   0 ken       (1000) ken       (1000)    25308 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/hu_HU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    60371 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/de_DE.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_ES/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33152 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/es_ES/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_HK/
--rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/zh_HK/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43775 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/da_DK.po
--rw-r--r--   0 ken       (1000) ken       (1000)    55698 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/pl_PL.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43787 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/nl_SR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/vi_VN/
--rw-rw-r--   0 ken       (1000) ken       (1000)      510 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/vi_VN/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43775 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/po/ca_ES.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/nl_BE/
--rw-rw-r--   0 ken       (1000) ken       (1000)      524 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/nl_BE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    44197 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/el_GR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/it_IT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    25347 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/it_IT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43795 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/zh_HK.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ru_UA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32879 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ru_UA/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_EM/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33161 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_EM/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43770 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ja_JP.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/pt_PT/
--rw-rw-r--   0 ken       (1000) ken       (1000)      520 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/pt_PT/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_TW/
--rw-rw-r--   0 ken       (1000) ken       (1000)      522 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/zh_TW/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    60383 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/de_AT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/en_GB/
--rw-rw-r--   0 ken       (1000) ken       (1000)     3375 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/en_GB/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/cs_CZ/
--rw-rw-r--   0 ken       (1000) ken       (1000)    34670 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/cs_CZ/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/pl_PL/
--rw-rw-r--   0 ken       (1000) ken       (1000)    26950 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/pl_PL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43794 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/en_US.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_US/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33167 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_US/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/he_IL/
--rw-rw-r--   0 ken       (1000) ken       (1000)      964 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/he_IL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    48337 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/nl_NL.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ru_BY/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ru_BY/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/en_US/
--rw-rw-r--   0 ken       (1000) ken       (1000)      532 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/en_US/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ar_SA/
--rw-rw-r--   0 ken       (1000) ken       (1000)      598 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ar_SA/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/pt_BR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    24541 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/pt_BR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/tr_TR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     4256 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/tr_TR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/af_ZA/
--rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/af_ZA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)     1184 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/POTFILES.skip
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/nl_SR/
--rw-rw-r--   0 ken       (1000) ken       (1000)      525 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/nl_SR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ru_RU/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32928 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ru_RU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63046 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ru_BY.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ca_ES/
--rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ca_ES/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43861 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/sr_SP.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43784 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/zh_TW.po
--rw-r--r--   0 ken       (1000) ken       (1000)    63048 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ru_UA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ko_KR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     7034 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ko_KR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    44189 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/en_AU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/fi_FI/
--rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/fi_FI/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    62648 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/uk_UA.po
--rw-r--r--   0 ken       (1000) ken       (1000)     2322 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/POTFILES.in
--rwxr-xr-x   0 ken       (1000) ken       (1000)      361 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/update-pot
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/sr_SP/
--rw-rw-r--   0 ken       (1000) ken       (1000)      599 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/sr_SP/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/de_DE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    36226 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/de_DE/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/de_AT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    36238 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/de_AT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    63048 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ru_RU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/sv_SE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    24543 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/sv_SE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    57806 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/fr_FR.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43782 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/pt_PT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ro_RO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      559 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ro_RO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43860 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ar_SA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/el_GR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     1574 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/el_GR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    44011 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/he_IL.po
--rw-r--r--   0 ken       (1000) ken       (1000)    55151 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/hu_HU.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43786 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/nl_BE.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/en_AU/
--rw-rw-r--   0 ken       (1000) ken       (1000)     1412 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/en_AU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43791 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/zh_MO.po
--rw-r--r--   0 ken       (1000) ken       (1000)    45117 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/tr_TR.po
--rw-r--r--   0 ken       (1000) ken       (1000)      276 2023-05-26 15:53:32.000000 duplicity-2.0.0rc1/po/LINGUAS
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/da_DK/
--rw-rw-r--   0 ken       (1000) ken       (1000)      513 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/da_DK/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_MO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      529 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_MO/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_PR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33165 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_PR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_SG/
--rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_SG/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ja_JP/
--rw-rw-r--   0 ken       (1000) ken       (1000)      508 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ja_JP/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    58355 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/es_US.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_MX/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33160 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/es_MX/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/ru_MD/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/ru_MD/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43795 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/zh_SG.po
--rw-r--r--   0 ken       (1000) ken       (1000)    58348 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/es_MX.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/zh_CN/
--rw-rw-r--   0 ken       (1000) ken       (1000)    25656 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/zh_CN/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43792 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/en_PR.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43771 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/po/vi_VN.po
--rw-r--r--   0 ken       (1000) ken       (1000)    54208 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/sv_SE.po
--rw-r--r--   0 ken       (1000) ken       (1000)    58349 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/es_EM.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43778 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/af_ZA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/no_NO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/no_NO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    58353 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/es_PR.po
--rw-r--r--   0 ken       (1000) ken       (1000)     1174 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/po/Makevars
--rw-r--r--   0 ken       (1000) ken       (1000)    46512 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ko_KR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/en_PR/
--rw-rw-r--   0 ken       (1000) ken       (1000)      530 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/en_PR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    44024 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/duplicity.pot
--rw-r--r--   0 ken       (1000) ken       (1000)    43821 2023-06-30 18:02:20.000000 duplicity-2.0.0rc1/po/ro_RO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/po/fr_FR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    29965 2023-07-17 16:38:33.000000 duplicity-2.0.0rc1/po/fr_FR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity.egg-info/
--rw-r--r--   0 ken       (1000) ken       (1000)       18 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity.egg-info/top_level.txt
--rw-r--r--   0 ken       (1000) ken       (1000)       10 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity.egg-info/requires.txt
--rw-r--r--   0 ken       (1000) ken       (1000)     2360 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity.egg-info/PKG-INFO
--rw-r--r--   0 ken       (1000) ken       (1000)        1 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity.egg-info/dependency_links.txt
--rw-r--r--   0 ken       (1000) ken       (1000)     7555 2023-07-17 16:38:34.000000 duplicity-2.0.0rc1/duplicity.egg-info/SOURCES.txt
--rwxr-xr-x   0 ken       (1000) ken       (1000)    12544 2023-07-08 19:08:19.000000 duplicity-2.0.0rc1/setup.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1399 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/README.md
--rw-r--r--   0 ken       (1000) ken       (1000)     1315 2023-07-01 15:25:28.000000 duplicity-2.0.0rc1/README-REPO.md
--rw-r--r--   0 ken       (1000) ken       (1000)     5364 2023-04-24 17:35:53.000000 duplicity-2.0.0rc1/README-TESTING.md
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/
+-rw-r--r--   0 ken       (1000) ken       (1000)   110623 2023-07-24 16:22:34.000000 duplicity-2.0.0rc2/CHANGELOG.md
+-rw-r--r--   0 ken       (1000) ken       (1000)      101 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/setup.cfg
+-rw-r--r--   0 ken       (1000) ken       (1000)     1390 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 ken       (1000) ken       (1000)     2783 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/tox.ini
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/bin/
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     4186 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/bin/duplicity
+-rw-r--r--   0 ken       (1000) ken       (1000)    97668 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/bin/duplicity.1
+-rw-r--r--   0 ken       (1000) ken       (1000)      742 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/requirements.txt
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/snap/
+-rw-r--r--   0 ken       (1000) ken       (1000)     4684 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/snap/snapcraft.yaml
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/snap/local/
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      186 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/snap/local/debug.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      110 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/snap/local/launcher.sh
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/
+-rw-r--r--   0 ken       (1000) ken       (1000)   319661 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/testfiles.tar.gz
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/unit/
+-rw-r--r--   0 ken       (1000) ken       (1000)     8120 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_gpginterface.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    11286 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_patchdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6077 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_dup_time.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    11572 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_lazy.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    11157 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_cli_main.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5578 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_statistics.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13945 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_globmatch.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5703 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_manifest.py
+-rw-r--r--   0 ken       (1000) ken       (1000)      918 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    11690 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_collections.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2447 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_dup_temp.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5402 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_file_naming.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1178 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_tarfile.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12707 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_diffdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2483 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_tempdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10385 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_backend_instance.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2887 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_path.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1432 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_util.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8284 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_gpg.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12151 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    65210 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/unit/test_selection.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/overrides/
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/overrides/bin/
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      155 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/bin/ncftpget
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      512 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/bin/lftp
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      155 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/bin/ncftpput
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      423 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/bin/hsi
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      416 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/bin/tahoe
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      558 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/bin/ncftpls
+-rw-r--r--   0 ken       (1000) ken       (1000)       75 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/overrides/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     4634 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/__init__.py
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      878 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/run-tests
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/functional/
+-rw-r--r--   0 ken       (1000) ken       (1000)     2385 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/test_log.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9537 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/test_final.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1612 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/test_badupload.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3287 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/testing/functional/test_cleanup.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8328 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8640 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/test_verify.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    18677 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/test_restart.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    96829 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/functional/test_selection.py
+-rw-r--r--   0 ken       (1000) ken       (1000)      941 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/conftest.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3196 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/test_code.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/gnupg/
+-rw-r--r--   0 ken       (1000) ken       (1000)      145 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/gnupg/gpg-agent.conf
+-rw-r--r--   0 ken       (1000) ken       (1000)     3567 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/gnupg/pubring.gpg
+-rw-r--r--   0 ken       (1000) ken       (1000)     7549 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/gnupg/secring.gpg
+-rw-r--r--   0 ken       (1000) ken       (1000)      425 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/gnupg/gpg.conf
+-rw-r--r--   0 ken       (1000) ken       (1000)      255 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/gnupg/README
+-rw-r--r--   0 ken       (1000) ken       (1000)     1440 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/testing/gnupg/trustdb.gpg
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/testing/regression/
+-rw-r--r--   0 ken       (1000) ken       (1000)      295 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue103.json
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     1087 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue79.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      278 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue110-test.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      457 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug930151.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      503 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug1526557.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     1621 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue103.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     1312 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue125.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      685 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue25.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      516 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug1919017.sh
+-rw-r--r--   0 ken       (1000) ken       (1000)     8328 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)      144 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue73.env
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      680 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug1860200.sh
+-rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue25.json
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      554 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue110-setup.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      192 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug1846678.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     1001 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue98.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      417 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue100.sh
+-rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue79.json
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      418 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue73.sh
+-rw-r--r--   0 ken       (1000) ken       (1000)      189 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug1919017.json
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      905 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/bug487720.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      464 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue683.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      466 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue26.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      280 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/testing/regression/issue147.sh
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/duplicity/
+-rw-r--r--   0 ken       (1000) ken       (1000)    34560 2023-07-24 16:05:26.000000 duplicity-2.0.0rc2/duplicity/cli_data.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10701 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/dup_time.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/duplicity/backends/
+-rw-r--r--   0 ken       (1000) ken       (1000)     3040 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/localbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    16080 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/onedrivebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    16591 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/adbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8565 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/megav2backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10233 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/swiftbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     4284 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/rclonebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8757 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/b2backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2572 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/tahoebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    16132 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/gdrivebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12971 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/ssh_pexpect_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9159 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/gdocsbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8117 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/giobackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6624 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/megabackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12793 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/pydrivebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5652 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/azurebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1115 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    19244 2023-07-24 16:17:52.000000 duplicity-2.0.0rc2/duplicity/backends/idrivedbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    15477 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/multibackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    19777 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/dpbxbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     7103 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/boxbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1152 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/cfbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    19213 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/webdavbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10028 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/megav3backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2399 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/hubicbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9387 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/lftpbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6455 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/rsyncbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5393 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/ncftpbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     4719 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/mediafirebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2628 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/hsibackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8822 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/par2backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    19474 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/ssh_paramiko_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12468 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/pcabackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10535 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/s3_boto3_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5695 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/jottacloudbackend.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/duplicity/backends/pyrax_identity/
+-rw-r--r--   0 ken       (1000) ken       (1000)     9699 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/pyrax_identity/hubic.py
+-rw-r--r--   0 ken       (1000) ken       (1000)      903 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/duplicity/backends/pyrax_identity/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9732 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/imapbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3905 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/_cf_cloudfiles.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5141 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/_cf_pyrax.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2579 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/duplicity/backends/README
+-rw-r--r--   0 ken       (1000) ken       (1000)     2310 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/sxbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12227 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/xorrisobackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6461 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backends/slatebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     7237 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/dup_threading.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    62036 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/duplicity/dup_main.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    26344 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10934 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/duplicity/config.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     7525 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/globmatch.py
+-rw-r--r--   0 ken       (1000) ken       (1000)      995 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/duplicity/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8427 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/librsync.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2752 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/errors.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10624 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/tempdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1262 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/tarfile.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13789 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/progress.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    17370 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/gpg.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2627 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/filechunkio.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    21775 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/patchdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    18003 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/manifest.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    14877 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/duplicity/file_naming.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    14510 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/duplicity/_librsyncmodule.c
+-rw-r--r--   0 ken       (1000) ken       (1000)    46560 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/duplicity/dup_collections.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2476 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/robust.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    26076 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/diffdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1668 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/cached_ops.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9893 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/util.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8088 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/dup_temp.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12639 2023-07-24 16:02:22.000000 duplicity-2.0.0rc2/duplicity/cli_util.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10093 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/duplicity/asyncscheduler.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9158 2023-07-24 15:19:18.000000 duplicity-2.0.0rc2/duplicity/cli_main.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12882 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/duplicity/statistics.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    15046 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/lazy.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    28629 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/path.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    28636 2023-07-22 20:15:29.000000 duplicity-2.0.0rc2/duplicity/selection.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    15815 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/log.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    23296 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/duplicity/gpginterface.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1284 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/README-LOG.md
+-rw-rw-r--   0 ken       (1000) ken       (1000)     2360 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 ken       (1000) ken       (1000)    18028 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/COPYING
+-rw-r--r--   0 ken       (1000) ken       (1000)      164 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/crowdin.yml
+-rw-r--r--   0 ken       (1000) ken       (1000)     3250 2023-06-30 18:00:21.000000 duplicity-2.0.0rc2/README-SNAP.md
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/
+-rw-r--r--   0 ken       (1000) ken       (1000)    43776 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/fi_FI.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    63046 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ru_MD.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    58340 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/es_ES.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    54802 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/pt_BR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/uk_UA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32646 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/uk_UA/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    45098 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/en_GB.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    53411 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/zh_CN.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43778 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/no_NO.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/nl_NL/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    11565 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/nl_NL/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    54884 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/it_IT.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    58884 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/cs_CZ.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/hu_HU/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    25308 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/hu_HU/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    60371 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/de_DE.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/es_ES/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33152 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/es_ES/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/zh_HK/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/zh_HK/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43775 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/da_DK.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    55698 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/pl_PL.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43787 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/nl_SR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/vi_VN/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      510 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/vi_VN/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43775 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/po/ca_ES.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/nl_BE/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      524 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/nl_BE/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    44197 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/el_GR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/it_IT/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    25347 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/it_IT/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43795 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/zh_HK.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ru_UA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32879 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ru_UA/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/es_EM/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33161 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/es_EM/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43770 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ja_JP.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/pt_PT/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      520 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/pt_PT/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/zh_TW/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      522 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/zh_TW/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    60383 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/de_AT.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/en_GB/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     3375 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/en_GB/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/cs_CZ/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    34670 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/cs_CZ/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/pl_PL/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    26950 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/pl_PL/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43794 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/en_US.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/es_US/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33167 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/es_US/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/he_IL/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      964 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/he_IL/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    48337 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/nl_NL.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ru_BY/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ru_BY/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/en_US/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      532 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/en_US/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ar_SA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      598 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ar_SA/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/pt_BR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    24541 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/pt_BR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/tr_TR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     4256 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/tr_TR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/af_ZA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/af_ZA/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)     1184 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/POTFILES.skip
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/nl_SR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      525 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/nl_SR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ru_RU/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32928 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ru_RU/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    63046 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ru_BY.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ca_ES/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ca_ES/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43861 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/sr_SP.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43784 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/zh_TW.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    63048 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ru_UA.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ko_KR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     7034 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ko_KR/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    44189 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/en_AU.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/fi_FI/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/fi_FI/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    62648 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/uk_UA.po
+-rw-r--r--   0 ken       (1000) ken       (1000)     2322 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/POTFILES.in
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      361 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/update-pot
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/sr_SP/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      599 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/sr_SP/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/de_DE/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    36226 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/de_DE/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/de_AT/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    36238 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/de_AT/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    63048 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ru_RU.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/sv_SE/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    24543 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/sv_SE/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    57806 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/fr_FR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43782 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/pt_PT.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ro_RO/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      559 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ro_RO/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43860 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ar_SA.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/el_GR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1574 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/el_GR/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    44011 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/he_IL.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    55151 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/hu_HU.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43786 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/nl_BE.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/en_AU/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1412 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/en_AU/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43791 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/zh_MO.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    45117 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/tr_TR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)      276 2023-05-26 15:53:32.000000 duplicity-2.0.0rc2/po/LINGUAS
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/da_DK/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      513 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/da_DK/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/zh_MO/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      529 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/zh_MO/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/es_PR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33165 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/es_PR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/zh_SG/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/zh_SG/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ja_JP/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      508 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ja_JP/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    58355 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/es_US.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/es_MX/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33160 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/es_MX/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/ru_MD/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/ru_MD/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43795 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/zh_SG.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    58348 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/es_MX.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/zh_CN/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    25656 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/zh_CN/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43792 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/en_PR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43771 2023-07-22 17:10:39.000000 duplicity-2.0.0rc2/po/vi_VN.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    54208 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/sv_SE.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    58349 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/es_EM.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43778 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/af_ZA.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/no_NO/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/no_NO/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    58353 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/es_PR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)     1174 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/po/Makevars
+-rw-r--r--   0 ken       (1000) ken       (1000)    46512 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ko_KR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/en_PR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      530 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/en_PR/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    44024 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/duplicity.pot
+-rw-r--r--   0 ken       (1000) ken       (1000)    43821 2023-06-30 18:02:20.000000 duplicity-2.0.0rc2/po/ro_RO.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/po/fr_FR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    29965 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/po/fr_FR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/duplicity.egg-info/
+-rw-rw-r--   0 ken       (1000) ken       (1000)       18 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/duplicity.egg-info/top_level.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)       10 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/duplicity.egg-info/requires.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)     2360 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/duplicity.egg-info/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1000)        1 2023-07-24 16:31:12.000000 duplicity-2.0.0rc2/duplicity.egg-info/dependency_links.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)     7555 2023-07-24 16:31:13.000000 duplicity-2.0.0rc2/duplicity.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ken       (1000) ken       (1000)    12545 2023-07-24 16:19:56.000000 duplicity-2.0.0rc2/setup.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1399 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/README.md
+-rw-r--r--   0 ken       (1000) ken       (1000)     1315 2023-07-22 17:10:38.000000 duplicity-2.0.0rc2/README-REPO.md
+-rw-r--r--   0 ken       (1000) ken       (1000)     5364 2023-04-24 17:35:53.000000 duplicity-2.0.0rc2/README-TESTING.md
```

### Comparing `duplicity-2.0.0rc1/CHANGELOG.md` & `duplicity-2.0.0rc2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,35 @@
+## rel.2.0.0rc2 (2023-07-24)
+
+### Changes
+
+* Fix format strings in idrivedbackend.py. [Kenneth Loafman]
+
+* Add additional CLI checks. [Kenneth Loafman]
+
+* Fix format strings in idrivedbackend.py. [Kenneth Loafman]
+
+* Fix format string in statistics.py. [Kenneth Loafman]
+
+* Remove kerberos from snap builds. [Kenneth Loafman]
+
+  kerberos will not build in snapcraft.
+
+* Changes to allow building snaps. [Kenneth Loafman]
+
+  Found another bug in snapcraft, see:
+  https://bugs.launchpad.net/snapcraft/+bug/2028303
+
+
 ## rel.2.0.0rc1 (2023-07-17)
 
 ### Changes
 
+* Update CHANGELOG.md. [Kenneth Loafman]
+
 * Fix implied command handling. [Kenneth Loafman]
 
 * Create regression test dir from old scripts. [Kenneth Loafman]
 
 
 ## rel.2.0.0rc0 (2023-07-10)
```

### Comparing `duplicity-2.0.0rc1/CONTRIBUTING.md` & `duplicity-2.0.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/tox.ini` & `duplicity-2.0.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/bin/duplicity` & `duplicity-2.0.0rc2/bin/duplicity`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/bin/duplicity.1` & `duplicity-2.0.0rc2/bin/duplicity.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH DUPLICITY 1 "July 17, 2023" "Version 2.0.0rc1" "User Manuals" \"  -*- nroff -*-
+.TH DUPLICITY 1 "July 24, 2023" "Version 2.0.0rc2" "User Manuals" \"  -*- nroff -*-
 .\" disable justification (adjust text to left margin only)
 .\" command line examples stay readable through that
 .ad l
 .\" disable hyphenation
 .nh
 
 .SH NAME
```

### Comparing `duplicity-2.0.0rc1/requirements.txt` & `duplicity-2.0.0rc2/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 ##### installed first to avoid conflicts #####
 
 chardet<3.10
-urllib3<1.26
 cryptography==3.4.8
 requests
+urllib3<1.26
 
 ##### basic requirements #####
 
 fasteners
 python-gettext
 
 ##### backend libraries #####
@@ -35,21 +35,20 @@
 paramiko
 pexpect
 psutil
 pydrive2
 pyrax
 python-swiftclient
 python-keystoneclient
-requests
 requests-oauthlib
 
 ##### testing libraries #####
 
 coverage
-mock >= 3.0.5
+mock>=3.0.5
 pycodestyle
 pylint
 pytest
 pytest-cov
 pytest-runner
 setuptools>=44.1.1
 setuptools-scm>=5.0.2
```

### Comparing `duplicity-2.0.0rc1/snap/snapcraft.yaml` & `duplicity-2.0.0rc2/snap/snapcraft.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: duplicity
-version: 2.0.0rc1
+version: 2.0.0rc2
 license: GPL-2.0
 summary: Efficient, encrypted backup to local or remote hosts
 description: |
   Duplicity backs directories by producing encrypted tar-format volumes and uploading
   them to a remote or local file server. Because duplicity uses librsync, the incremental
   archives are space efficient and only record the parts of files that have changed since
   the last backup. Because duplicity uses GnuPG to encrypt and/or sign these archives,
@@ -50,14 +50,18 @@
             # show env vars for debugging
             #env
             # upgrade pip to latest
             apt install curl -y
             curl -s https://bootstrap.pypa.io/get-pip.py -o get-pip.py
             python3 get-pip.py
             snapcraftctl build
+            # Some python modules cause snap build to import argparse from pypi.
+            # argparse in pypi supports <= 3.4 so we need the distribution version.
+            # Let pip remove that version since the new one is in the distribution.
+            python3 -m pip uninstall -y argparse
             # python module tahoe-lafs dies trying to compile really old pycddl 
             # on other archs than amd64, as python plugin does not support 
             # conditions we only include it in amd64 snaps manually here
             if [ "$SNAPCRAFT_BUILD_FOR" != "amd64" ]; then
                 echo "Skipping tahoe-lafs integration on arch '$SNAPCRAFT_BUILD_FOR'!='amd64'"
             else
                 pip install tahoe-lafs
```

### Comparing `duplicity-2.0.0rc1/testing/testfiles.tar.gz` & `duplicity-2.0.0rc2/testing/testfiles.tar.gz`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_gpginterface.py` & `duplicity-2.0.0rc2/testing/unit/test_gpginterface.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_patchdir.py` & `duplicity-2.0.0rc2/testing/unit/test_patchdir.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 fp.close()
 
         tf = patchdir.TarFile_FromFileobjs(get_fileobjs())
         namelist = []
         for tarinfo in tf:
             namelist.append(tarinfo.name)
         for i in range(1, 6):
-            assert (f"tmp/{int(i)}") in namelist, namelist
+            assert f"tmp/{int(i)}" in namelist, namelist
 
     def test_doubledot_hole(self):
         """Test for the .. bug that lets tar overwrite parent dir"""
 
         def make_bad_tar(filename):
             """Write attack tarfile to filename"""
             tf = tarfile.TarFile(name=filename, mode="w")
@@ -291,16 +291,16 @@
             fout = result.open("rb")
             contents = fout.read()
             assert not fout.close()
             assert contents == buf, (contents, buf)
 
         ids = f"{int(os.getuid())}:{int(os.getgid())}"
 
-        testseq([self.snapshot()], (f"{ids} 600"), b"hello, world!")
-        testseq([self.snapshot(), self.delta1()], (f"{ids} 640"),
+        testseq([self.snapshot()], f"{ids} 600", b"hello, world!")
+        testseq([self.snapshot(), self.delta1()], f"{ids} 640",
                 b"aonseuth aosetnuhaonsuhtansoetuhaoe")
-        testseq([self.snapshot(), self.delta1(), self.delta2()], (f"{ids} 644"),
+        testseq([self.snapshot(), self.delta1(), self.delta2()], f"{ids} 644",
                 b"3499 34957839485792357 458348573")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `duplicity-2.0.0rc1/testing/unit/test_dup_time.py` & `duplicity-2.0.0rc2/testing/unit/test_dup_time.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_lazy.py` & `duplicity-2.0.0rc2/testing/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_cli_main.py` & `duplicity-2.0.0rc2/testing/unit/test_cli_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_statistics.py` & `duplicity-2.0.0rc2/testing/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_globmatch.py` & `duplicity-2.0.0rc2/testing/unit/test_globmatch.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_manifest.py` & `duplicity-2.0.0rc2/testing/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/__init__.py` & `duplicity-2.0.0rc2/testing/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_collections.py` & `duplicity-2.0.0rc2/testing/unit/test_collections.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_dup_temp.py` & `duplicity-2.0.0rc2/testing/unit/test_dup_temp.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_file_naming.py` & `duplicity-2.0.0rc2/testing/unit/test_file_naming.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_tarfile.py` & `duplicity-2.0.0rc2/testing/unit/test_tarfile.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_diffdir.py` & `duplicity-2.0.0rc2/testing/unit/test_diffdir.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     tf2 = tarfile.TarFile("none", "r", tarfile2)
     tf2_iter = iter(tf2)
 
     for ti1 in tf1:
         try:
             ti2 = next(tf2_iter)
         except StopIteration:
-            assert 0, (f"Premature end to second tarfile, ti1.name = {ti1.name}")
+            assert 0, f"Premature end to second tarfile, ti1.name = {ti1.name}"
         # print "Comparing ", ti1.name, ti2.name
         assert tarinfo_eq(ti1, ti2), f"{ti1.name} {ti2.name}"
         if ti1.size != 0:
             fp1 = tf1.extractfile(ti1)
             buf1 = fp1.read()
             fp1.close()
             fp2 = tf2.extractfile(ti2)
@@ -271,15 +271,15 @@
             fp2.close()
             assert buf1 == buf2
     try:
         ti2 = next(tf2_iter)
     except StopIteration:
         pass
     else:
-        assert 0, (f"Premature end to first tarfile, ti2.name = {ti2.name}")
+        assert 0, f"Premature end to first tarfile, ti2.name = {ti2.name}"
 
     tarfile1.close()
     tarfile2.close()
 
 
 def tarinfo_eq(ti1, ti2):
     if ti1.name != ti2.name:
```

### Comparing `duplicity-2.0.0rc1/testing/unit/test_tempdir.py` & `duplicity-2.0.0rc2/testing/unit/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_backend_instance.py` & `duplicity-2.0.0rc2/testing/unit/test_backend_instance.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_path.py` & `duplicity-2.0.0rc2/testing/unit/test_path.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_util.py` & `duplicity-2.0.0rc2/testing/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_gpg.py` & `duplicity-2.0.0rc2/testing/unit/test_gpg.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_backend.py` & `duplicity-2.0.0rc2/testing/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/unit/test_selection.py` & `duplicity-2.0.0rc2/testing/unit/test_selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/overrides/bin/lftp` & `duplicity-2.0.0rc2/testing/overrides/bin/lftp`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/overrides/bin/ncftpls` & `duplicity-2.0.0rc2/testing/overrides/bin/ncftpls`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/__init__.py` & `duplicity-2.0.0rc2/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/run-tests` & `duplicity-2.0.0rc2/testing/run-tests`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_log.py` & `duplicity-2.0.0rc2/testing/functional/test_log.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_final.py` & `duplicity-2.0.0rc2/testing/functional/test_final.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_badupload.py` & `duplicity-2.0.0rc2/testing/functional/test_badupload.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_cleanup.py` & `duplicity-2.0.0rc2/testing/functional/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/__init__.py` & `duplicity-2.0.0rc2/testing/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_verify.py` & `duplicity-2.0.0rc2/testing/functional/test_verify.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_restart.py` & `duplicity-2.0.0rc2/testing/functional/test_restart.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/functional/test_selection.py` & `duplicity-2.0.0rc2/testing/functional/test_selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/conftest.py` & `duplicity-2.0.0rc2/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/test_code.py` & `duplicity-2.0.0rc2/testing/test_code.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/gnupg/pubring.gpg` & `duplicity-2.0.0rc2/testing/gnupg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/gnupg/secring.gpg` & `duplicity-2.0.0rc2/testing/gnupg/secring.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/gnupg/trustdb.gpg` & `duplicity-2.0.0rc2/testing/gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/issue79.sh` & `duplicity-2.0.0rc2/testing/regression/issue79.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/issue103.sh` & `duplicity-2.0.0rc2/testing/regression/issue103.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/issue125.sh` & `duplicity-2.0.0rc2/testing/regression/issue125.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/issue25.sh` & `duplicity-2.0.0rc2/testing/regression/issue25.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/bug1919017.sh` & `duplicity-2.0.0rc2/testing/regression/bug1919017.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/__init__.py` & `duplicity-2.0.0rc2/testing/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/bug1860200.sh` & `duplicity-2.0.0rc2/testing/regression/bug1860200.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/issue110-setup.sh` & `duplicity-2.0.0rc2/testing/regression/issue110-setup.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/issue98.sh` & `duplicity-2.0.0rc2/testing/regression/issue98.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/testing/regression/bug487720.sh` & `duplicity-2.0.0rc2/testing/regression/bug487720.sh`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/cli_data.py` & `duplicity-2.0.0rc2/duplicity/cli_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,14 +671,15 @@
         "metavar": _("seconds"),
         "type": check_timeout,
         "help": "Network timeout in seconds",
         "default": dflt(config.timeout)
     }
     time_separator = {
         "metavar": _("char"),
+        "type": check_char,
         "help": "Character used like the ':' in time strings like\n"
                 "2002-08-06T04:22:00-07:00",
         "default": dflt(config.time_separator)
     }
     use_agent = {
         "action": "store_true",
         "help": "Whether to specify --use-agent in GnuPG options",
```

### Comparing `duplicity-2.0.0rc1/duplicity/dup_time.py` & `duplicity-2.0.0rc2/duplicity/dup_time.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/localbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/localbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/onedrivebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/onedrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/adbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/adbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/megav2backend.py` & `duplicity-2.0.0rc2/duplicity/backends/megav2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/swiftbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/swiftbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/rclonebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/rclonebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/b2backend.py` & `duplicity-2.0.0rc2/duplicity/backends/b2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/tahoebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/tahoebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/gdrivebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/gdrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/ssh_pexpect_backend.py` & `duplicity-2.0.0rc2/duplicity/backends/ssh_pexpect_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/gdocsbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/gdocsbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/giobackend.py` & `duplicity-2.0.0rc2/duplicity/backends/giobackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/megabackend.py` & `duplicity-2.0.0rc2/duplicity/backends/megabackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/pydrivebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/pydrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/azurebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/azurebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/__init__.py` & `duplicity-2.0.0rc2/duplicity/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/idrivedbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/idrivedbackend.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,16 +236,17 @@
         self.idrivedevid = None
         for item in el.findall('item'):
             if item.attrib['nick_name'] == self.bucket:
                 # prefix and suffix reverse-engineered from Common.pl!
                 self.idrivedevid = f"5c0b{item.attrib['device_id']}4b5z"
         if self.idrivedevid is None:
             el = self.request(
-                self.cmd + self.auth_switch +
-                f" --create-bucket --bucket-type=D --nick-name={self.bucket} --os=Linux --uid=987654321 "
+                f"{self.cmd}{self.auth_switch} "
+                f"--create-bucket --bucket-type=D --nick-name={self.bucket} "
+                f"--os=Linux --uid=987654321 "
                 f"{self.idriveid}@{self.idriveserver}::home/").find('item')
             # prefix and suffix reverse-engineered from Common.pl!
             self.idrivedevid = f"5c0b{el.attrib['device_id']}4b5z"
 
         # We're fully connected!
         self.connected = True
         log.Debug("User fully connected")
@@ -291,16 +292,18 @@
 
         log.Debug(f"put_file: source_path={source_path.name}, remote_file={filename}")
 
         flist = tempfile.NamedTemporaryFile('w')
         flist.write(intrim_file)
         flist.seek(0)
 
-        putrequest = (f"{self.cmd + self.auth_switch}  --device-id={{0}} --files-from={{1}} / {{2}}@{{3}}::home/{{4}}"
-                      .format(self.idrivedevid, flist.name, self.idriveid, self.idriveserver, remote_dirpath))
+        putrequest = f"{self.cmd}{self.auth_switch} " \
+                     f"--device-id={self.idrivedevid} " \
+                     f"--files-from={flist.name} / " \
+                     f"{self.idriveid}@{self.idriveserver}::home/{remote_dirpath}"
         log.Debug(f"put_file put command: {putrequest}")
         _, putresponse, _ = self.subprocess_popen(putrequest)
         log.Debug(f"put_file put response: {putresponse}")
 
         flist.close()
         os.remove(intrim_file)
 
@@ -324,21 +327,21 @@
         log.Debug(f"_get created temporary download folder: {tmpdir}")
 
         # The filelist file
         flist = tempfile.NamedTemporaryFile('w')
         flist.write(remote_path)
         flist.seek(0)
 
-        commandline = f"{self.cmd + self.auth_switch} " \
-                      f"--device-id={self.idrivedevid} " \
-                      f"--files-from={flist.name} " \
-                      f"{self.idriveid}@{self.idriveserver}::home/ " \
-                      f"{tmpdir}"
-        log.Debug(f"get command: {commandline}")
-        _, getresponse, _ = self.subprocess_popen(commandline)
+        getrequest = f"{self.cmd}{self.auth_switch} " \
+                     f"--device-id={self.idrivedevid} " \
+                     f"--files-from={flist.name} " \
+                     f"{self.idriveid}@{self.idriveserver}::home/ " \
+                     f"{tmpdir}"
+        log.Debug(f"get command: {getrequest}")
+        _, getresponse, _ = self.subprocess_popen(getrequest)
         log.Debug(f"_get response: {getresponse}")
 
         flist.close()
 
         # move to the final location
         downloadedSrcPath = os.path.join(tmpdir, remote_path.lstrip('/').rstrip('/'))
         log.Debug(f"_get moving file {downloadedSrcPath} to final location: {local_path.name}")
@@ -374,17 +377,19 @@
 
         # target path (remote) on IDrive
         remote_path = os.path.join(urllib.parse.unquote(self.parsed_url.path.lstrip('/')),
                                    self.fakeroot.lstrip('/')).rstrip()
         log.Debug(f"delete: {filename} from remote file path {remote_path}")
 
         # delete files from file-list
-        delrequest = ((self.cmd + self.auth_switch +
-                       " --delete-items --device-id={0} --files-from={1} {2}@{3}::home/{4}")
-                      .format(self.idrivedevid, flist.name, self.idriveid, self.idriveserver, remote_path))
+        delrequest = f"{self.cmd}{self.auth_switch} " \
+                     f"--delete-items " \
+                     f"--device-id={self.idrivedevid} " \
+                     f"--files-from={flist.name} " \
+                     f"{self.idriveid}@{self.idriveserver}::home/{remote_path}"
         log.Debug(f"delete: {delrequest}")
         _, delresponse, _ = self.subprocess_popen(delrequest)
         log.Debug(f"delete response: {delresponse}")
 
         # close tempfile
         flist.close()
 
@@ -404,17 +409,19 @@
 
         # target path (remote) on IDrive
         remote_path = os.path.join(urllib.parse.unquote(self.parsed_url.path.lstrip('/')),
                                    self.fakeroot.lstrip('/')).rstrip()
         log.Debug(f"delete multiple files from remote file path {remote_path}")
 
         # delete files from file-list
-        delrequest = ((self.cmd + self.auth_switch +
-                       " --delete-items --device-id={0} --files-from={1} {2}@{3}::home/{4}")
-                      .format(self.idrivedevid, flist.name, self.idriveid, self.idriveserver, remote_path))
+        delrequest = f"{self.cmd}{self.auth_switch} " \
+                     f"--delete-items " \
+                     f"--device-id={self.idrivedevid} " \
+                     f"--files-from={flist.name} " \
+                     f"{self.idriveid}@{self.idriveserver}::home/{remote_path}"
         log.Debug(f"delete: {delrequest}")
         _, delresponse, _ = self.subprocess_popen(delrequest)
         log.Debug(f"delete response: {delresponse}")
 
         # close tempfile
         flist.close()
```

### Comparing `duplicity-2.0.0rc1/duplicity/backends/multibackend.py` & `duplicity-2.0.0rc2/duplicity/backends/multibackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/dpbxbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/dpbxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/boxbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/boxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/cfbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/cfbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/webdavbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/webdavbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/megav3backend.py` & `duplicity-2.0.0rc2/duplicity/backends/megav3backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/hubicbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/hubicbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/lftpbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/lftpbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/rsyncbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/rsyncbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/ncftpbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/ncftpbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/mediafirebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/mediafirebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/hsibackend.py` & `duplicity-2.0.0rc2/duplicity/backends/hsibackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/par2backend.py` & `duplicity-2.0.0rc2/duplicity/backends/par2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/ssh_paramiko_backend.py` & `duplicity-2.0.0rc2/duplicity/backends/ssh_paramiko_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/pcabackend.py` & `duplicity-2.0.0rc2/duplicity/backends/pcabackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/s3_boto3_backend.py` & `duplicity-2.0.0rc2/duplicity/backends/s3_boto3_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/jottacloudbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/jottacloudbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/pyrax_identity/hubic.py` & `duplicity-2.0.0rc2/duplicity/backends/pyrax_identity/hubic.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/pyrax_identity/__init__.py` & `duplicity-2.0.0rc2/duplicity/backends/pyrax_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/imapbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/imapbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/_cf_cloudfiles.py` & `duplicity-2.0.0rc2/duplicity/backends/_cf_cloudfiles.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/_cf_pyrax.py` & `duplicity-2.0.0rc2/duplicity/backends/_cf_pyrax.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/README` & `duplicity-2.0.0rc2/duplicity/backends/README`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/sxbackend.py` & `duplicity-2.0.0rc2/duplicity/backends/sxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/xorrisobackend.py` & `duplicity-2.0.0rc2/duplicity/backends/xorrisobackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backends/slatebackend.py` & `duplicity-2.0.0rc2/duplicity/backends/slatebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/dup_threading.py` & `duplicity-2.0.0rc2/duplicity/dup_threading.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/dup_main.py` & `duplicity-2.0.0rc2/duplicity/dup_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/backend.py` & `duplicity-2.0.0rc2/duplicity/backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/config.py` & `duplicity-2.0.0rc2/duplicity/config.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/globmatch.py` & `duplicity-2.0.0rc2/duplicity/globmatch.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/__init__.py` & `duplicity-2.0.0rc2/duplicity/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with duplicity; if not, write to the Free Software Foundation,
 # Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
 import gettext
 
-__version__ = '2.0.0rc1'
+__version__ = '2.0.0rc2'
 
 gettext.install('duplicity', names=['ngettext'])
```

### Comparing `duplicity-2.0.0rc1/duplicity/librsync.py` & `duplicity-2.0.0rc2/duplicity/librsync.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/errors.py` & `duplicity-2.0.0rc2/duplicity/errors.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/tempdir.py` & `duplicity-2.0.0rc2/duplicity/tempdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/tarfile.py` & `duplicity-2.0.0rc2/duplicity/tarfile.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/progress.py` & `duplicity-2.0.0rc2/duplicity/progress.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/gpg.py` & `duplicity-2.0.0rc2/duplicity/gpg.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/filechunkio.py` & `duplicity-2.0.0rc2/duplicity/filechunkio.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/patchdir.py` & `duplicity-2.0.0rc2/duplicity/patchdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/manifest.py` & `duplicity-2.0.0rc2/duplicity/manifest.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/file_naming.py` & `duplicity-2.0.0rc2/duplicity/file_naming.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/_librsyncmodule.c` & `duplicity-2.0.0rc2/duplicity/_librsyncmodule.c`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/dup_collections.py` & `duplicity-2.0.0rc2/duplicity/dup_collections.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/robust.py` & `duplicity-2.0.0rc2/duplicity/robust.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/diffdir.py` & `duplicity-2.0.0rc2/duplicity/diffdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/cached_ops.py` & `duplicity-2.0.0rc2/duplicity/cached_ops.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/util.py` & `duplicity-2.0.0rc2/duplicity/util.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/dup_temp.py` & `duplicity-2.0.0rc2/duplicity/dup_temp.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/cli_util.py` & `duplicity-2.0.0rc2/duplicity/cli_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,25 +103,27 @@
     def __init__(self, option_strings, dest, **kwargs):
         super().__init__(option_strings, dest, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         command_line_error(dedent(
             f"""\
             Option '{option_string} was removed in 2.0.0.
-            The following options were deprecated in 2.0.0
+            These additional options were deprecated in 2.0.0
                 --exclude-filelist-stdin
                 --exclude-globbing-filelist
                 --gio
                 --include-filelist-stdin
                 --include-globbing-filelist
                 --old-filenames
                 --s3-multipart-max-timeout
                 --s3-use-multiprocessing
                 --s3-use-server-side-encryption
-                --short-filenames"""))
+                --short-filenames
+                --time-separator
+                """))
 
 
 class ChangedOptionAction(DuplicityAction):
     def __init__(self, option_strings, dest, **kwargs):
         super().__init__(option_strings, dest, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
@@ -135,14 +137,21 @@
 def _check_int(val):
     try:
         return int(val)
     except Exception as e:
         command_line_error(_(f"'{val}' is not an int: {str(e)}"))
 
 
+def check_char(val):
+    if len(val) == 1:
+        return val
+    else:
+        command_line_error(_(f"'{val} is not a single character."))
+
+
 def check_count(val):
     return _check_int(val)
 
 
 def check_file(value):
     return os.fsencode(expand_fn(value))
```

### Comparing `duplicity-2.0.0rc1/duplicity/asyncscheduler.py` & `duplicity-2.0.0rc2/duplicity/asyncscheduler.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/cli_main.py` & `duplicity-2.0.0rc2/duplicity/cli_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/statistics.py` & `duplicity-2.0.0rc2/duplicity/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,16 +192,15 @@
                 abbrev_count = float(byte_count) / abbrev_bytes
                 if abbrev_count >= 100:
                     precision = 0
                 elif abbrev_count >= 10:
                     precision = 1
                 else:
                     precision = 2
-                return f"{sign}%.{int(precision)}f {abbrev_string}" \
-                    % (abbrev_count,)
+                return f"{sign}{abbrev_count:.{precision}f} {abbrev_string}"
         byte_count = round(byte_count)
         if byte_count == 1:
             return f"{sign}1 byte"
         else:
             return f"{sign}{int(byte_count)} bytes"
 
     def get_stats_logstring(self, title):
```

### Comparing `duplicity-2.0.0rc1/duplicity/lazy.py` & `duplicity-2.0.0rc2/duplicity/lazy.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/path.py` & `duplicity-2.0.0rc2/duplicity/path.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/selection.py` & `duplicity-2.0.0rc2/duplicity/selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/log.py` & `duplicity-2.0.0rc2/duplicity/log.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity/gpginterface.py` & `duplicity-2.0.0rc2/duplicity/gpginterface.py`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/README-LOG.md` & `duplicity-2.0.0rc2/README-LOG.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/PKG-INFO` & `duplicity-2.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplicity
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Encrypted backup using rsync algorithm
 Home-page: http://duplicity.us
 Author: Ben Escoto <ben@emrose.org>
 Author-email: ben@emrose.org
 Maintainer: Kenneth Loafman <kenneth@loafman.com>
 Maintainer-email: kenneth@loafman.com
 Platform: any
```

### Comparing `duplicity-2.0.0rc1/COPYING` & `duplicity-2.0.0rc2/COPYING`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/README-SNAP.md` & `duplicity-2.0.0rc2/README-SNAP.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/fi_FI.po` & `duplicity-2.0.0rc2/po/fi_FI.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_MD.po` & `duplicity-2.0.0rc2/po/ru_MD.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_ES.po` & `duplicity-2.0.0rc2/po/es_ES.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/pt_BR.po` & `duplicity-2.0.0rc2/po/pt_BR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/uk_UA/duplicity.mo` & `duplicity-2.0.0rc2/po/uk_UA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_GB.po` & `duplicity-2.0.0rc2/po/en_GB.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_CN.po` & `duplicity-2.0.0rc2/po/zh_CN.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/no_NO.po` & `duplicity-2.0.0rc2/po/no_NO.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/nl_NL/duplicity.mo` & `duplicity-2.0.0rc2/po/nl_NL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/it_IT.po` & `duplicity-2.0.0rc2/po/it_IT.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/cs_CZ.po` & `duplicity-2.0.0rc2/po/cs_CZ.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/hu_HU/duplicity.mo` & `duplicity-2.0.0rc2/po/hu_HU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/de_DE.po` & `duplicity-2.0.0rc2/po/de_DE.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_ES/duplicity.mo` & `duplicity-2.0.0rc2/po/es_ES/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_HK/duplicity.mo` & `duplicity-2.0.0rc2/po/zh_HK/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/da_DK.po` & `duplicity-2.0.0rc2/po/da_DK.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/pl_PL.po` & `duplicity-2.0.0rc2/po/pl_PL.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/nl_SR.po` & `duplicity-2.0.0rc2/po/nl_SR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ca_ES.po` & `duplicity-2.0.0rc2/po/ca_ES.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/nl_BE/duplicity.mo` & `duplicity-2.0.0rc2/po/nl_BE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/el_GR.po` & `duplicity-2.0.0rc2/po/el_GR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/it_IT/duplicity.mo` & `duplicity-2.0.0rc2/po/it_IT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_HK.po` & `duplicity-2.0.0rc2/po/zh_HK.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_UA/duplicity.mo` & `duplicity-2.0.0rc2/po/ru_UA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_EM/duplicity.mo` & `duplicity-2.0.0rc2/po/es_EM/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ja_JP.po` & `duplicity-2.0.0rc2/po/ja_JP.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/pt_PT/duplicity.mo` & `duplicity-2.0.0rc2/po/pt_PT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_TW/duplicity.mo` & `duplicity-2.0.0rc2/po/zh_TW/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/de_AT.po` & `duplicity-2.0.0rc2/po/de_AT.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_GB/duplicity.mo` & `duplicity-2.0.0rc2/po/en_GB/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/cs_CZ/duplicity.mo` & `duplicity-2.0.0rc2/po/cs_CZ/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/pl_PL/duplicity.mo` & `duplicity-2.0.0rc2/po/pl_PL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_US.po` & `duplicity-2.0.0rc2/po/en_US.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_US/duplicity.mo` & `duplicity-2.0.0rc2/po/es_US/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/he_IL/duplicity.mo` & `duplicity-2.0.0rc2/po/he_IL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/nl_NL.po` & `duplicity-2.0.0rc2/po/nl_NL.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_BY/duplicity.mo` & `duplicity-2.0.0rc2/po/ru_BY/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_US/duplicity.mo` & `duplicity-2.0.0rc2/po/en_US/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ar_SA/duplicity.mo` & `duplicity-2.0.0rc2/po/ar_SA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/pt_BR/duplicity.mo` & `duplicity-2.0.0rc2/po/pt_BR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/tr_TR/duplicity.mo` & `duplicity-2.0.0rc2/po/tr_TR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/af_ZA/duplicity.mo` & `duplicity-2.0.0rc2/po/af_ZA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/POTFILES.skip` & `duplicity-2.0.0rc2/po/POTFILES.skip`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/nl_SR/duplicity.mo` & `duplicity-2.0.0rc2/po/nl_SR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_RU/duplicity.mo` & `duplicity-2.0.0rc2/po/ru_RU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_BY.po` & `duplicity-2.0.0rc2/po/ru_BY.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ca_ES/duplicity.mo` & `duplicity-2.0.0rc2/po/ca_ES/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/sr_SP.po` & `duplicity-2.0.0rc2/po/sr_SP.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_TW.po` & `duplicity-2.0.0rc2/po/zh_TW.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_UA.po` & `duplicity-2.0.0rc2/po/ru_UA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ko_KR/duplicity.mo` & `duplicity-2.0.0rc2/po/ko_KR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_AU.po` & `duplicity-2.0.0rc2/po/en_AU.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/fi_FI/duplicity.mo` & `duplicity-2.0.0rc2/po/fi_FI/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/uk_UA.po` & `duplicity-2.0.0rc2/po/uk_UA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/POTFILES.in` & `duplicity-2.0.0rc2/po/POTFILES.in`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/sr_SP/duplicity.mo` & `duplicity-2.0.0rc2/po/sr_SP/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/de_DE/duplicity.mo` & `duplicity-2.0.0rc2/po/de_DE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/de_AT/duplicity.mo` & `duplicity-2.0.0rc2/po/de_AT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_RU.po` & `duplicity-2.0.0rc2/po/ru_RU.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/sv_SE/duplicity.mo` & `duplicity-2.0.0rc2/po/sv_SE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/fr_FR.po` & `duplicity-2.0.0rc2/po/fr_FR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/pt_PT.po` & `duplicity-2.0.0rc2/po/pt_PT.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ro_RO/duplicity.mo` & `duplicity-2.0.0rc2/po/ro_RO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ar_SA.po` & `duplicity-2.0.0rc2/po/ar_SA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/el_GR/duplicity.mo` & `duplicity-2.0.0rc2/po/el_GR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/he_IL.po` & `duplicity-2.0.0rc2/po/he_IL.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/hu_HU.po` & `duplicity-2.0.0rc2/po/hu_HU.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/nl_BE.po` & `duplicity-2.0.0rc2/po/nl_BE.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_AU/duplicity.mo` & `duplicity-2.0.0rc2/po/en_AU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_MO.po` & `duplicity-2.0.0rc2/po/zh_MO.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/tr_TR.po` & `duplicity-2.0.0rc2/po/tr_TR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/da_DK/duplicity.mo` & `duplicity-2.0.0rc2/po/da_DK/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_MO/duplicity.mo` & `duplicity-2.0.0rc2/po/zh_MO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_PR/duplicity.mo` & `duplicity-2.0.0rc2/po/es_PR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_SG/duplicity.mo` & `duplicity-2.0.0rc2/po/zh_SG/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_US.po` & `duplicity-2.0.0rc2/po/es_US.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_MX/duplicity.mo` & `duplicity-2.0.0rc2/po/es_MX/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ru_MD/duplicity.mo` & `duplicity-2.0.0rc2/po/ru_MD/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_SG.po` & `duplicity-2.0.0rc2/po/zh_SG.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_MX.po` & `duplicity-2.0.0rc2/po/es_MX.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/zh_CN/duplicity.mo` & `duplicity-2.0.0rc2/po/zh_CN/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_PR.po` & `duplicity-2.0.0rc2/po/en_PR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/vi_VN.po` & `duplicity-2.0.0rc2/po/vi_VN.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/sv_SE.po` & `duplicity-2.0.0rc2/po/sv_SE.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_EM.po` & `duplicity-2.0.0rc2/po/es_EM.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/af_ZA.po` & `duplicity-2.0.0rc2/po/af_ZA.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/no_NO/duplicity.mo` & `duplicity-2.0.0rc2/po/no_NO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/es_PR.po` & `duplicity-2.0.0rc2/po/es_PR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/Makevars` & `duplicity-2.0.0rc2/po/Makevars`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ko_KR.po` & `duplicity-2.0.0rc2/po/ko_KR.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/en_PR/duplicity.mo` & `duplicity-2.0.0rc2/po/en_PR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/duplicity.pot` & `duplicity-2.0.0rc2/po/duplicity.pot`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/ro_RO.po` & `duplicity-2.0.0rc2/po/ro_RO.po`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/po/fr_FR/duplicity.mo` & `duplicity-2.0.0rc2/po/fr_FR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/duplicity.egg-info/PKG-INFO` & `duplicity-2.0.0rc2/duplicity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplicity
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Encrypted backup using rsync algorithm
 Home-page: http://duplicity.us
 Author: Ben Escoto <ben@emrose.org>
 Author-email: ben@emrose.org
 Maintainer: Kenneth Loafman <kenneth@loafman.com>
 Maintainer-email: kenneth@loafman.com
 Platform: any
```

### Comparing `duplicity-2.0.0rc1/duplicity.egg-info/SOURCES.txt` & `duplicity-2.0.0rc2/duplicity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/setup.py` & `duplicity-2.0.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 # check that we can function here
 if not (sys.version_info[0] == 3 and sys.version_info[1] >= 8):
     print("Sorry, duplicity requires version 3.8 or later of Python3.")
     sys.exit(1)
 
 
-Version = "2.0.0b2"
+Version = "2.0.0rc2"
 scm_version_args = {
     'tag_regex': r'^(?P<prefix>rel.)?(?P<version>[^\+]+)(?P<suffix>.*)?$',
     'local_scheme': 'no-local-version',
     'fallback_version': Version,
     }
 try:
     from setuptools_scm import get_version  # pylint: disable=import-error
```

### Comparing `duplicity-2.0.0rc1/README.md` & `duplicity-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/README-REPO.md` & `duplicity-2.0.0rc2/README-REPO.md`

 * *Files identical despite different names*

### Comparing `duplicity-2.0.0rc1/README-TESTING.md` & `duplicity-2.0.0rc2/README-TESTING.md`

 * *Files identical despite different names*

