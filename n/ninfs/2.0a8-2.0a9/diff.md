# Comparing `tmp/ninfs-2.0a8.tar.gz` & `tmp/ninfs-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninfs-2.0a8.tar", last modified: Sun Jan 30 01:15:44 2022, max compression
+gzip compressed data, was "ninfs-2.0a9.tar", last modified: Fri Mar 25 01:15:03 2022, max compression
```

## Comparing `ninfs-2.0a8.tar` & `ninfs-2.0a9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.921769 ninfs-2.0a8/
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1083 2021-01-22 13:56:03.000000 ninfs-2.0a8/LICENSE.md
--rw-r--r--   0 ianburgwin   (501) staff       (20)    11362 2022-01-30 01:15:44.921628 ninfs-2.0a8/PKG-INFO
--rw-r--r--   0 ianburgwin   (501) staff       (20)    10693 2022-01-27 03:55:20.000000 ninfs-2.0a8/README.md
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.909303 ninfs-2.0a8/ninfs/
--rw-r--r--   0 ianburgwin   (501) staff       (20)      334 2022-01-30 01:13:06.000000 ninfs-2.0a8/ninfs/__init__.py
--rwxr-xr-x   0 ianburgwin   (501) staff       (20)      647 2021-01-22 13:55:14.000000 ninfs-2.0a8/ninfs/__main__.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)      666 2021-05-10 18:44:10.000000 ninfs-2.0a8/ninfs/_frozen_main.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1904 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/fmt_detect.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    42051 2021-01-22 13:55:14.000000 ninfs-2.0a8/ninfs/fuse.py
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.912104 ninfs-2.0a8/ninfs/gui/
--rw-r--r--   0 ianburgwin   (501) staff       (20)    13838 2022-01-27 08:01:13.000000 ninfs-2.0a8/ninfs/gui/__init__.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     4544 2022-01-27 06:19:47.000000 ninfs-2.0a8/ninfs/gui/about.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2153 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/confighandler.py
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.914730 ninfs-2.0a8/ninfs/gui/data/
--rw-r--r--   0 ianburgwin   (501) staff       (20)   969467 2020-09-07 05:15:15.000000 ninfs-2.0a8/ninfs/gui/data/1024x1024.png
--rw-r--r--   0 ianburgwin   (501) staff       (20)    21665 2020-09-07 05:15:15.000000 ninfs-2.0a8/ninfs/gui/data/128x128.png
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1321 2020-09-07 05:15:15.000000 ninfs-2.0a8/ninfs/gui/data/16x16.png
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2878 2020-09-07 05:15:15.000000 ninfs-2.0a8/ninfs/gui/data/32x32.png
--rw-r--r--   0 ianburgwin   (501) staff       (20)     7493 2020-09-07 05:15:15.000000 ninfs-2.0a8/ninfs/gui/data/64x64.png
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.916056 ninfs-2.0a8/ninfs/gui/data/licenses/
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1105 2020-09-19 17:22:25.000000 ninfs-2.0a8/ninfs/gui/data/licenses/haccrypto.md
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1083 2021-03-09 03:02:51.000000 ninfs-2.0a8/ninfs/gui/data/licenses/ninfs.md
--rw-r--r--   0 ianburgwin   (501) staff       (20)     3262 2021-03-09 03:01:43.000000 ninfs-2.0a8/ninfs/gui/data/licenses/pycryptodome.rst
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1083 2021-03-09 03:01:58.000000 ninfs-2.0a8/ninfs/gui/data/licenses/pyctr
--rw-r--r--   0 ianburgwin   (501) staff       (20)    36642 2020-09-19 17:22:25.000000 ninfs-2.0a8/ninfs/gui/data/licenses/winfsp.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)   138190 2022-01-27 07:58:28.000000 ninfs-2.0a8/ninfs/gui/data/windows.ico
--rw-r--r--   0 ianburgwin   (501) staff       (20)      876 2021-01-22 13:55:14.000000 ninfs-2.0a8/ninfs/gui/opendir.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1512 2021-01-22 13:55:14.000000 ninfs-2.0a8/ninfs/gui/optionsframes.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1165 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/osver.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1067 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/outputviewer.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2065 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/settings.py
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.918316 ninfs-2.0a8/ninfs/gui/setupwizard/
--rw-r--r--   0 ianburgwin   (501) staff       (20)      686 2021-06-29 03:25:47.000000 ninfs-2.0a8/ninfs/gui/setupwizard/__init__.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     4336 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/base.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1887 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/cci.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2896 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/cdn.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2888 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/cia.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1282 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/exefs.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1309 2021-04-15 06:34:54.000000 ninfs-2.0a8/ninfs/gui/setupwizard/nandbb.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2627 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/nandctr.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     3026 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/nandhac.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2128 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/nandtwl.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2894 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/ncch.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1282 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/romfs.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2907 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/sd.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2924 2021-06-29 03:23:52.000000 ninfs-2.0a8/ninfs/gui/setupwizard/sdtitle.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1286 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/srl.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1284 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/setupwizard/threedsx.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)      873 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/supportfiles.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2684 2021-01-22 13:55:13.000000 ninfs-2.0a8/ninfs/gui/updatecheck.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    14799 2022-01-30 01:01:04.000000 ninfs-2.0a8/ninfs/gui/wizardcontainer.py
--rwxr-xr-x   0 ianburgwin   (501) staff       (20)     5160 2021-07-09 09:50:40.000000 ninfs-2.0a8/ninfs/main.py
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.921375 ninfs-2.0a8/ninfs/mount/
--rw-r--r--   0 ianburgwin   (501) staff       (20)        0 2021-03-23 17:21:36.000000 ninfs-2.0a8/ninfs/mount/__init__.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    11767 2021-07-09 10:22:21.000000 ninfs-2.0a8/ninfs/mount/_common.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     6011 2021-04-14 20:32:09.000000 ninfs-2.0a8/ninfs/mount/cci.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     7276 2021-04-14 20:32:09.000000 ninfs-2.0a8/ninfs/mount/cdn.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     7051 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/cia.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     6482 2022-01-27 03:49:56.000000 ninfs-2.0a8/ninfs/mount/exefs.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     6478 2021-04-14 20:32:09.000000 ninfs-2.0a8/ninfs/mount/nandbb.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    19193 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/nandctr.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    12337 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/nandhac.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    10626 2021-06-22 14:40:30.000000 ninfs-2.0a8/ninfs/mount/nandtwl.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     6685 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/ncch.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     4057 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/romfs.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    10437 2021-06-27 04:32:07.000000 ninfs-2.0a8/ninfs/mount/sd.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     7440 2021-06-29 03:20:45.000000 ninfs-2.0a8/ninfs/mount/sdtitle.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)    11068 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/srl.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     5634 2021-04-14 20:35:28.000000 ninfs-2.0a8/ninfs/mount/threedsx.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     2342 2022-01-30 00:50:41.000000 ninfs-2.0a8/ninfs/mountinfo.py
--rwxr-xr-x   0 ianburgwin   (501) staff       (20)     1896 2021-01-22 13:55:14.000000 ninfs-2.0a8/ninfs/reg_shell.py
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1732 2021-01-22 13:55:14.000000 ninfs-2.0a8/ninfs/winpathmodify.py
-drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-01-30 01:15:44.910028 ninfs-2.0a8/ninfs.egg-info/
--rw-r--r--   0 ianburgwin   (501) staff       (20)    11362 2022-01-30 01:15:44.000000 ninfs-2.0a8/ninfs.egg-info/PKG-INFO
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1808 2022-01-30 01:15:44.000000 ninfs-2.0a8/ninfs.egg-info/SOURCES.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)        1 2022-01-30 01:15:44.000000 ninfs-2.0a8/ninfs.egg-info/dependency_links.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)      858 2022-01-30 01:15:44.000000 ninfs-2.0a8/ninfs.egg-info/entry_points.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)       69 2022-01-30 01:15:44.000000 ninfs-2.0a8/ninfs.egg-info/requires.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)        6 2022-01-30 01:15:44.000000 ninfs-2.0a8/ninfs.egg-info/top_level.txt
--rw-r--r--   0 ianburgwin   (501) staff       (20)       38 2022-01-30 01:15:44.921806 ninfs-2.0a8/setup.cfg
--rw-r--r--   0 ianburgwin   (501) staff       (20)     1898 2022-01-27 03:39:02.000000 ninfs-2.0a8/setup.py
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.015789 ninfs-2.0a9/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1083 2021-01-22 13:56:03.000000 ninfs-2.0a9/LICENSE.md
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    11344 2022-03-25 01:15:03.015566 ninfs-2.0a9/PKG-INFO
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    10675 2022-03-23 22:23:15.000000 ninfs-2.0a9/README.md
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.007345 ninfs-2.0a9/ninfs/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)      334 2022-03-25 01:04:19.000000 ninfs-2.0a9/ninfs/__init__.py
+-rwxr-xr-x   0 ianburgwin   (501) staff       (20)      647 2021-01-22 13:55:14.000000 ninfs-2.0a9/ninfs/__main__.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)      666 2021-05-10 18:44:10.000000 ninfs-2.0a9/ninfs/_frozen_main.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1904 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/fmt_detect.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    42051 2021-01-22 13:55:14.000000 ninfs-2.0a9/ninfs/fuse.py
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.009669 ninfs-2.0a9/ninfs/gui/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    13820 2022-03-23 22:22:49.000000 ninfs-2.0a9/ninfs/gui/__init__.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     4544 2022-01-27 06:19:47.000000 ninfs-2.0a9/ninfs/gui/about.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2153 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/confighandler.py
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.010984 ninfs-2.0a9/ninfs/gui/data/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)   969467 2020-09-07 05:15:15.000000 ninfs-2.0a9/ninfs/gui/data/1024x1024.png
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    21665 2020-09-07 05:15:15.000000 ninfs-2.0a9/ninfs/gui/data/128x128.png
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1321 2020-09-07 05:15:15.000000 ninfs-2.0a9/ninfs/gui/data/16x16.png
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2878 2020-09-07 05:15:15.000000 ninfs-2.0a9/ninfs/gui/data/32x32.png
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     7493 2020-09-07 05:15:15.000000 ninfs-2.0a9/ninfs/gui/data/64x64.png
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.011643 ninfs-2.0a9/ninfs/gui/data/licenses/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1105 2020-09-19 17:22:25.000000 ninfs-2.0a9/ninfs/gui/data/licenses/haccrypto.md
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1083 2021-03-09 03:02:51.000000 ninfs-2.0a9/ninfs/gui/data/licenses/ninfs.md
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     3262 2021-03-09 03:01:43.000000 ninfs-2.0a9/ninfs/gui/data/licenses/pycryptodome.rst
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1083 2021-03-09 03:01:58.000000 ninfs-2.0a9/ninfs/gui/data/licenses/pyctr
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    36642 2020-09-19 17:22:25.000000 ninfs-2.0a9/ninfs/gui/data/licenses/winfsp.txt
+-rw-r--r--   0 ianburgwin   (501) staff       (20)   138190 2022-03-25 01:09:46.000000 ninfs-2.0a9/ninfs/gui/data/windows.ico
+-rw-r--r--   0 ianburgwin   (501) staff       (20)      876 2021-01-22 13:55:14.000000 ninfs-2.0a9/ninfs/gui/opendir.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1512 2021-01-22 13:55:14.000000 ninfs-2.0a9/ninfs/gui/optionsframes.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1165 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/osver.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1067 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/outputviewer.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2065 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/settings.py
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.013455 ninfs-2.0a9/ninfs/gui/setupwizard/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)      686 2021-06-29 03:25:47.000000 ninfs-2.0a9/ninfs/gui/setupwizard/__init__.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     4336 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/base.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1887 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/cci.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2896 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/cdn.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2888 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/cia.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1282 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/exefs.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1309 2021-04-15 06:34:54.000000 ninfs-2.0a9/ninfs/gui/setupwizard/nandbb.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2627 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/nandctr.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     3026 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/nandhac.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2128 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/nandtwl.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2894 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/ncch.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1282 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/romfs.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2907 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/sd.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2924 2021-06-29 03:23:52.000000 ninfs-2.0a9/ninfs/gui/setupwizard/sdtitle.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1286 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/srl.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1284 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/setupwizard/threedsx.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)      873 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/supportfiles.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2684 2021-01-22 13:55:13.000000 ninfs-2.0a9/ninfs/gui/updatecheck.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    14825 2022-03-25 00:32:00.000000 ninfs-2.0a9/ninfs/gui/wizardcontainer.py
+-rwxr-xr-x   0 ianburgwin   (501) staff       (20)     5160 2021-07-09 09:50:40.000000 ninfs-2.0a9/ninfs/main.py
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.015377 ninfs-2.0a9/ninfs/mount/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)        0 2021-03-23 17:21:36.000000 ninfs-2.0a9/ninfs/mount/__init__.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    11767 2021-07-09 10:22:21.000000 ninfs-2.0a9/ninfs/mount/_common.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     6011 2022-02-08 19:18:23.000000 ninfs-2.0a9/ninfs/mount/cci.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     7276 2022-02-08 19:18:23.000000 ninfs-2.0a9/ninfs/mount/cdn.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     7051 2022-02-08 19:18:23.000000 ninfs-2.0a9/ninfs/mount/cia.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     6482 2022-02-08 19:18:23.000000 ninfs-2.0a9/ninfs/mount/exefs.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     6474 2022-02-08 19:18:49.000000 ninfs-2.0a9/ninfs/mount/nandbb.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    19133 2022-02-08 19:19:22.000000 ninfs-2.0a9/ninfs/mount/nandctr.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    12277 2022-02-08 19:19:22.000000 ninfs-2.0a9/ninfs/mount/nandhac.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    10566 2022-02-08 19:19:57.000000 ninfs-2.0a9/ninfs/mount/nandtwl.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     6685 2022-02-08 19:19:57.000000 ninfs-2.0a9/ninfs/mount/ncch.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     4057 2022-02-08 19:19:57.000000 ninfs-2.0a9/ninfs/mount/romfs.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    10437 2021-06-27 04:32:07.000000 ninfs-2.0a9/ninfs/mount/sd.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     7440 2022-02-08 19:20:20.000000 ninfs-2.0a9/ninfs/mount/sdtitle.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    11068 2022-02-08 19:20:20.000000 ninfs-2.0a9/ninfs/mount/srl.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     5634 2022-02-08 19:20:31.000000 ninfs-2.0a9/ninfs/mount/threedsx.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     2342 2022-01-30 00:50:41.000000 ninfs-2.0a9/ninfs/mountinfo.py
+-rwxr-xr-x   0 ianburgwin   (501) staff       (20)     1896 2021-01-22 13:55:14.000000 ninfs-2.0a9/ninfs/reg_shell.py
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1732 2021-01-22 13:55:14.000000 ninfs-2.0a9/ninfs/winpathmodify.py
+drwxr-xr-x   0 ianburgwin   (501) staff       (20)        0 2022-03-25 01:15:03.008103 ninfs-2.0a9/ninfs.egg-info/
+-rw-r--r--   0 ianburgwin   (501) staff       (20)    11344 2022-03-25 01:15:03.000000 ninfs-2.0a9/ninfs.egg-info/PKG-INFO
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1808 2022-03-25 01:15:03.000000 ninfs-2.0a9/ninfs.egg-info/SOURCES.txt
+-rw-r--r--   0 ianburgwin   (501) staff       (20)        1 2022-03-25 01:15:03.000000 ninfs-2.0a9/ninfs.egg-info/dependency_links.txt
+-rw-r--r--   0 ianburgwin   (501) staff       (20)      858 2022-03-25 01:15:03.000000 ninfs-2.0a9/ninfs.egg-info/entry_points.txt
+-rw-r--r--   0 ianburgwin   (501) staff       (20)       69 2022-03-25 01:15:03.000000 ninfs-2.0a9/ninfs.egg-info/requires.txt
+-rw-r--r--   0 ianburgwin   (501) staff       (20)        6 2022-03-25 01:15:03.000000 ninfs-2.0a9/ninfs.egg-info/top_level.txt
+-rw-r--r--   0 ianburgwin   (501) staff       (20)       38 2022-03-25 01:15:03.015834 ninfs-2.0a9/setup.cfg
+-rw-r--r--   0 ianburgwin   (501) staff       (20)     1898 2022-01-27 03:39:02.000000 ninfs-2.0a9/setup.py
```

### Comparing `ninfs-2.0a8/LICENSE.md` & `ninfs-2.0a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/PKG-INFO` & `ninfs-2.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninfs
-Version: 2.0a8
+Version: 2.0a9
 Summary: FUSE filesystem Python scripts for Nintendo console files
 Home-page: https://github.com/ihaveamac/ninfs
 Author: Ian Burgwin
 Author-email: ian@ianburgwin.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
@@ -77,20 +77,20 @@
 ### Windows
 Windows 8.1 or later is required.
 
 #### Installer
 An installer is provided in [releases](https://github.com/ihaveamac/ninfs/releases). It includes both ninfs and WinFsp, which is installed if required.
 
 #### Standalone release
-A standalone zip is also provided in [releases](https://github.com/ihaveamac/ninfs/releases). [WinFsp](http://www.secfs.net/winfsp/rel/) must be installed separately.
+A standalone zip is also provided in [releases](https://github.com/ihaveamac/ninfs/releases). [WinFsp](https://winfsp.dev/rel/) must be installed separately.
 
 #### Install with existing Python
 * Install the latest version of [Python 3](https://www.python.org/downloads/). The x86-64 version is preferred on 64-bit Windows.
   * Python from the Microsoft Store can also be used. If this is used, `python3` must be used instead of `py -3`. This version has some limitations however, such as not being able to mount to directories.
-* Install the latest version of [WinFsp](http://www.secfs.net/winfsp/rel/).
+* Install the latest version of [WinFsp](https://winfsp.dev/rel/).
 * Install ninfs with `py -3 -m pip install --upgrade https://github.com/ihaveamac/ninfs/archive/2.0.zip`
 
 ### macOS
 Versions of macOS supported by Apple are highly recommended. macOS Sierra is the oldest version that should work. [macFUSE](https://osxfuse.github.io/) is required.
 
 No standalone build is available at the moment.
```

### Comparing `ninfs-2.0a8/README.md` & `ninfs-2.0a9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,20 +57,20 @@
 ### Windows
 Windows 8.1 or later is required.
 
 #### Installer
 An installer is provided in [releases](https://github.com/ihaveamac/ninfs/releases). It includes both ninfs and WinFsp, which is installed if required.
 
 #### Standalone release
-A standalone zip is also provided in [releases](https://github.com/ihaveamac/ninfs/releases). [WinFsp](http://www.secfs.net/winfsp/rel/) must be installed separately.
+A standalone zip is also provided in [releases](https://github.com/ihaveamac/ninfs/releases). [WinFsp](https://winfsp.dev/rel/) must be installed separately.
 
 #### Install with existing Python
 * Install the latest version of [Python 3](https://www.python.org/downloads/). The x86-64 version is preferred on 64-bit Windows.
   * Python from the Microsoft Store can also be used. If this is used, `python3` must be used instead of `py -3`. This version has some limitations however, such as not being able to mount to directories.
-* Install the latest version of [WinFsp](http://www.secfs.net/winfsp/rel/).
+* Install the latest version of [WinFsp](https://winfsp.dev/rel/).
 * Install ninfs with `py -3 -m pip install --upgrade https://github.com/ihaveamac/ninfs/archive/2.0.zip`
 
 ### macOS
 Versions of macOS supported by Apple are highly recommended. macOS Sierra is the oldest version that should work. [macFUSE](https://osxfuse.github.io/) is required.
 
 No standalone build is available at the moment.
```

### Comparing `ninfs-2.0a8/ninfs/__main__.py` & `ninfs-2.0a9/ninfs/__main__.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/_frozen_main.py` & `ninfs-2.0a9/ninfs/_frozen_main.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/fmt_detect.py` & `ninfs-2.0a9/ninfs/fmt_detect.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/fuse.py` & `ninfs-2.0a9/ninfs/fuse.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/__init__.py` & `ninfs-2.0a9/ninfs/gui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,17 @@
             import fuse
         except EnvironmentError as e:
             if e.args[0] == 'Unable to find libfuse':
                 if is_windows:
                     res = mb.askyesno('Failed to load libfuse',
                                       'Failed to load libfuse. WinFsp needs to be installed.\n\n'
                                       'Would you like to open the WinFsp download page?\n'
-                                      'http://www.secfs.net/winfsp/rel/')
+                                      'https://winfsp.dev/rel/')
                     if res:
-                        webbrowser.open('http://www.secfs.net/winfsp/rel/')
+                        webbrowser.open('https://winfsp.dev/rel/')
                 elif is_mac:
                     res = mb.askyesno('Failed to load libfuse',
                                       'Failed to load libfuse. macFUSE needs to be installed.\n\n'
                                       'Would you like to open the macFUSE download page?\n'
                                       'https://osxfuse.github.io')
                     if res:
                         webbrowser.open('https://osxfuse.github.io')
```

### Comparing `ninfs-2.0a8/ninfs/gui/about.py` & `ninfs-2.0a9/ninfs/gui/about.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/confighandler.py` & `ninfs-2.0a9/ninfs/gui/confighandler.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/1024x1024.png` & `ninfs-2.0a9/ninfs/gui/data/1024x1024.png`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/128x128.png` & `ninfs-2.0a9/ninfs/gui/data/128x128.png`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/16x16.png` & `ninfs-2.0a9/ninfs/gui/data/16x16.png`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/32x32.png` & `ninfs-2.0a9/ninfs/gui/data/32x32.png`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/64x64.png` & `ninfs-2.0a9/ninfs/gui/data/64x64.png`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/licenses/haccrypto.md` & `ninfs-2.0a9/ninfs/gui/data/licenses/haccrypto.md`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/licenses/ninfs.md` & `ninfs-2.0a9/ninfs/gui/data/licenses/ninfs.md`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/licenses/pycryptodome.rst` & `ninfs-2.0a9/ninfs/gui/data/licenses/pycryptodome.rst`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/licenses/pyctr` & `ninfs-2.0a9/ninfs/gui/data/licenses/pyctr`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/licenses/winfsp.txt` & `ninfs-2.0a9/ninfs/gui/data/licenses/winfsp.txt`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/data/windows.ico` & `ninfs-2.0a9/ninfs/gui/data/windows.ico`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/opendir.py` & `ninfs-2.0a9/ninfs/gui/opendir.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/optionsframes.py` & `ninfs-2.0a9/ninfs/gui/optionsframes.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/osver.py` & `ninfs-2.0a9/ninfs/gui/osver.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/outputviewer.py` & `ninfs-2.0a9/ninfs/gui/outputviewer.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/settings.py` & `ninfs-2.0a9/ninfs/gui/settings.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/__init__.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/__init__.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/base.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/base.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/cci.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/cci.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/cdn.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/cdn.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/cia.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/cia.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/exefs.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/exefs.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/nandbb.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/nandbb.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/nandctr.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/nandctr.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/nandhac.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/nandhac.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/nandtwl.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/nandtwl.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/ncch.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/ncch.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/romfs.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/romfs.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/sd.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/sd.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/sdtitle.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/sdtitle.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/srl.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/srl.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/setupwizard/threedsx.py` & `ninfs-2.0a9/ninfs/gui/setupwizard/threedsx.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/supportfiles.py` & `ninfs-2.0a9/ninfs/gui/supportfiles.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/updatecheck.py` & `ninfs-2.0a9/ninfs/gui/updatecheck.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/gui/wizardcontainer.py` & `ninfs-2.0a9/ninfs/gui/wizardcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
         self.adv_options = {'user_access': 'none', 'use_dev': False}
 
         # special case for nand types here, which should not be mounted to a drive letter
         if is_windows and not cmdargs[0].startswith('nand'):
             self.is_drive_letter = True
 
-            drive_letters = ['A:', 'B:']
+            drive_letters = [x + ':' for x in get_unused_drives()]
 
             container, drive_selector, drive_selector_var = self.make_option_menu('Select the drive letter to use:',
                                                                                   *drive_letters)
             container.pack(fill=tk.X, expand=True)
 
             self.mount_point_var = drive_selector_var
```

### Comparing `ninfs-2.0a8/ninfs/main.py` & `ninfs-2.0a9/ninfs/main.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/mount/_common.py` & `ninfs-2.0a9/ninfs/mount/_common.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/mount/cci.py` & `ninfs-2.0a9/ninfs/mount/cci.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         first_dir = _c.get_first_dir(path)
         if first_dir in self.dirs:
             return self.dirs[first_dir].getattr(_c.remove_first_dir(path), fh)
         uid, gid, pid = fuse_get_context()
         if path == '/':
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': self.reader.sections[self.files[path]].size, 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': self.reader.sections[self.files[path]].size, 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
```

### Comparing `ninfs-2.0a8/ninfs/mount/cdn.py` & `ninfs-2.0a9/ninfs/mount/cdn.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         first_dir = _c.get_first_dir(path)
         if first_dir in self.dirs:
             return self.dirs[first_dir].getattr(_c.remove_first_dir(path), fh)
         uid, gid, pid = fuse_get_context()
         if path == '/' or path in self.dirs:
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': self.files[path][2], 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': self.files[path][2], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
```

### Comparing `ninfs-2.0a8/ninfs/mount/cia.py` & `ninfs-2.0a9/ninfs/mount/cia.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,17 @@
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         first_dir = _c.get_first_dir(path)
         if first_dir in self.dirs:
             return self.dirs[first_dir].getattr(_c.remove_first_dir(path), fh)
         uid, gid, pid = fuse_get_context()
         if path == '/' or path in self.dirs:
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': self.files[path][2], 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': self.files[path][2], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
```

### Comparing `ninfs-2.0a8/ninfs/mount/exefs.py` & `ninfs-2.0a9/ninfs/mount/exefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,25 @@
             self.special_files['/icon_small.png'] = {'size': icon_small_size, 'io': icon_small}
             self.special_files['/icon_large.png'] = {'size': icon_large_size, 'io': icon_large}
 
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         uid, gid, pid = fuse_get_context()
         if path == '/':
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         else:
             if path in self.files:
                 item = self.reader.entries[self.files[path]]
                 size = item.size
             elif path in self.special_files:
                 item = self.special_files[path]
                 size = item['size']
             else:
                 raise FuseOSError(ENOENT)
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': size, 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': size, 'st_nlink': 1}
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
 
     @_c.ensure_lower_path
```

### Comparing `ninfs-2.0a8/ninfs/mount/nandbb.py` & `ninfs-2.0a9/ninfs/mount/nandbb.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,17 +102,17 @@
     def flush(self, path, fh):
         return self.f.flush()
     
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         uid, gid, pid = fuse_get_context()
         if path == '/':
-            st = {'st_mode': (S_IFDIR | (0o555)), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | (0o444)),
+            st = {'st_mode': (S_IFREG | 0o666),
                   'st_size': self.files[path]['size'], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
     
     def open(self, path, flags):
         self.fd += 1
```

### Comparing `ninfs-2.0a8/ninfs/mount/nandctr.py` & `ninfs-2.0a9/ninfs/mount/nandctr.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,17 +261,17 @@
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         if path.startswith('/essential/'):
             return self.exefs_fuse.getattr(_c.remove_first_dir(path), fh)
         else:
             uid, gid, pid = fuse_get_context()
             if path in {'/', '/essential'}:
-                st = {'st_mode': (S_IFDIR | (0o555 if self.readonly else 0o777)), 'st_nlink': 2}
+                st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
             elif path in self.files:
-                st = {'st_mode': (S_IFREG | (0o444 if self.readonly else 0o666)),
+                st = {'st_mode': (S_IFREG | 0o666),
                       'st_size': self.files[path]['size'], 'st_nlink': 1}
             else:
                 raise FuseOSError(ENOENT)
             return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
```

### Comparing `ninfs-2.0a8/ninfs/mount/nandhac.py` & `ninfs-2.0a9/ninfs/mount/nandhac.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,18 @@
     def flush(self, path, fh):
         return self.f.flush()
 
     @_c.ensure_lower_path
     def getattr(self, path: str, fh=None):
         uid, gid, pid = fuse_get_context()
         if path == '/':
-            st = {'st_mode': (S_IFDIR | (0o555 if self.readonly else 0o777)), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
             p = self.files[path]
-            st = {'st_mode': (S_IFREG | (0o444 if self.readonly else 0o666)),
+            st = {'st_mode': (S_IFREG | 0o666),
                   'st_size': p['end'] - p['start'], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path: str, flags):
         self.fd += 1
```

### Comparing `ninfs-2.0a8/ninfs/mount/nandtwl.py` & `ninfs-2.0a9/ninfs/mount/nandtwl.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,17 @@
     def flush(self, path, fh):
         return self.f.flush()
 
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         uid, gid, pid = fuse_get_context()
         if path == '/':
-            st = {'st_mode': (S_IFDIR | (0o555 if self.readonly else 0o777)), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | (0o444 if self.readonly else 0o666)),
+            st = {'st_mode': (S_IFREG | 0o666),
                   'st_size': self.files[path]['size'], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
```

### Comparing `ninfs-2.0a8/ninfs/mount/ncch.py` & `ninfs-2.0a9/ninfs/mount/ncch.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
     def getattr(self, path, fh=None):
         if path.startswith('/exefs/'):
             return self.exefs_fuse.getattr(_c.remove_first_dir(path), fh)
         elif path.startswith('/romfs/'):
             return self.romfs_fuse.getattr(_c.remove_first_dir(path), fh)
         uid, gid, pid = fuse_get_context()
         if path in {'/', '/romfs', '/exefs'}:
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': self.reader.sections[self.files[path]].size, 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': self.reader.sections[self.files[path]].size, 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
```

### Comparing `ninfs-2.0a8/ninfs/mount/romfs.py` & `ninfs-2.0a9/ninfs/mount/romfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     def getattr(self, path, fh=None):
         uid, gid, pid = fuse_get_context()
         try:
             item = self.reader.get_info_from_path(path)
         except RomFSFileNotFoundError:
             raise FuseOSError(ENOENT)
         if item.type == 'dir':
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif item.type == 'file':
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': item.size, 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': item.size, 'st_nlink': 1}
         else:
             # this won't happen unless I fucked up
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
```

### Comparing `ninfs-2.0a8/ninfs/mount/sd.py` & `ninfs-2.0a9/ninfs/mount/sd.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/mount/sdtitle.py` & `ninfs-2.0a9/ninfs/mount/sdtitle.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,17 @@
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         first_dir = _c.get_first_dir(path)
         if first_dir in self.dirs:
             return self.dirs[first_dir].getattr(_c.remove_first_dir(path), fh)
         uid, gid, pid = fuse_get_context()
         if path == '/' or path in self.dirs:
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': self.files[path][2], 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': self.files[path][2], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
```

### Comparing `ninfs-2.0a8/ninfs/mount/srl.py` & `ninfs-2.0a9/ninfs/mount/srl.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,17 +230,17 @@
     destroy = __del__
 
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         uid, gid, pid = fuse_get_context()
         item = self.parse_path(path)
         if item['type'] == 'dir':
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif item['type'] == 'file':
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': item['size'], 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': item['size'], 'st_nlink': 1}
         else:
             # this won't happen unless I fucked up
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     @_c.ensure_lower_path
     def open(self, path, flags):
```

### Comparing `ninfs-2.0a8/ninfs/mount/threedsx.py` & `ninfs-2.0a9/ninfs/mount/threedsx.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 
     @_c.ensure_lower_path
     def getattr(self, path, fh=None):
         if path.startswith('/romfs/'):
             return self.romfs_fuse.getattr(_c.remove_first_dir(path), fh)
         uid, gid, pid = fuse_get_context()
         if path == '/' or path == '/romfs':
-            st = {'st_mode': (S_IFDIR | 0o555), 'st_nlink': 2}
+            st = {'st_mode': (S_IFDIR | 0o777), 'st_nlink': 2}
         elif path in self.files:
-            st = {'st_mode': (S_IFREG | 0o444), 'st_size': self.files[path]['size'], 'st_nlink': 1}
+            st = {'st_mode': (S_IFREG | 0o666), 'st_size': self.files[path]['size'], 'st_nlink': 1}
         else:
             raise FuseOSError(ENOENT)
         return {**st, **self.g_stat, 'st_uid': uid, 'st_gid': gid}
 
     def open(self, path, flags):
         self.fd += 1
         return self.fd
```

### Comparing `ninfs-2.0a8/ninfs/mountinfo.py` & `ninfs-2.0a9/ninfs/mountinfo.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/reg_shell.py` & `ninfs-2.0a9/ninfs/reg_shell.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs/winpathmodify.py` & `ninfs-2.0a9/ninfs/winpathmodify.py`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs.egg-info/PKG-INFO` & `ninfs-2.0a9/ninfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninfs
-Version: 2.0a8
+Version: 2.0a9
 Summary: FUSE filesystem Python scripts for Nintendo console files
 Home-page: https://github.com/ihaveamac/ninfs
 Author: Ian Burgwin
 Author-email: ian@ianburgwin.net
 License: MIT
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
@@ -77,20 +77,20 @@
 ### Windows
 Windows 8.1 or later is required.
 
 #### Installer
 An installer is provided in [releases](https://github.com/ihaveamac/ninfs/releases). It includes both ninfs and WinFsp, which is installed if required.
 
 #### Standalone release
-A standalone zip is also provided in [releases](https://github.com/ihaveamac/ninfs/releases). [WinFsp](http://www.secfs.net/winfsp/rel/) must be installed separately.
+A standalone zip is also provided in [releases](https://github.com/ihaveamac/ninfs/releases). [WinFsp](https://winfsp.dev/rel/) must be installed separately.
 
 #### Install with existing Python
 * Install the latest version of [Python 3](https://www.python.org/downloads/). The x86-64 version is preferred on 64-bit Windows.
   * Python from the Microsoft Store can also be used. If this is used, `python3` must be used instead of `py -3`. This version has some limitations however, such as not being able to mount to directories.
-* Install the latest version of [WinFsp](http://www.secfs.net/winfsp/rel/).
+* Install the latest version of [WinFsp](https://winfsp.dev/rel/).
 * Install ninfs with `py -3 -m pip install --upgrade https://github.com/ihaveamac/ninfs/archive/2.0.zip`
 
 ### macOS
 Versions of macOS supported by Apple are highly recommended. macOS Sierra is the oldest version that should work. [macFUSE](https://osxfuse.github.io/) is required.
 
 No standalone build is available at the moment.
```

### Comparing `ninfs-2.0a8/ninfs.egg-info/SOURCES.txt` & `ninfs-2.0a9/ninfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/ninfs.egg-info/entry_points.txt` & `ninfs-2.0a9/ninfs.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ninfs-2.0a8/setup.py` & `ninfs-2.0a9/setup.py`

 * *Files identical despite different names*

