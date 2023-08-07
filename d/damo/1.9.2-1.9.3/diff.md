# Comparing `tmp/damo-1.9.2.tar.gz` & `tmp/damo-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.9.2.tar", last modified: Tue Aug  1 00:43:31 2023, max compression
+gzip compressed data, was "damo-1.9.3.tar", last modified: Mon Aug  7 19:16:45 2023, max compression
```

## Comparing `damo-1.9.2.tar` & `damo-1.9.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.461842 damo-1.9.2/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-08-01 00:43:31.461842 damo-1.9.2/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-08-01 00:43:27.000000 damo-1.9.2/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.2/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-08-01 00:43:31.461842 damo-1.9.2/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.2/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.445843 damo-1.9.2/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.461842 damo-1.9.2/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:27.000000 damo-1.9.2/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/_damo_deprecated.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.2/src/damo/_damo_deprecation_notice.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.2/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    36884 2023-07-30 19:06:29.000000 damo-1.9.2/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    15397 2023-07-30 18:25:59.000000 damo-1.9.2/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.2/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-07-30 17:37:07.000000 damo-1.9.2/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20236 2023-07-29 21:28:06.000000 damo-1.9.2/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3853 2023-07-23 17:09:22.000000 damo-1.9.2/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.2/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.2/src/damo/damo_convert_record_format.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13384 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.2/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.2/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_record_info.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.2/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.2/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    18632 2023-07-30 19:06:29.000000 damo-1.9.2/src/damo/damo_show.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.2/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3447 2023-07-30 17:59:22.000000 damo-1.9.2/src/damo/damo_status.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.2/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.2/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.2/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.2/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-08-01 00:42:15.000000 damo-1.9.2/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.2/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-01 00:43:31.461842 damo-1.9.2/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1136 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-08-01 00:43:31.000000 damo-1.9.2/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-07 19:16:45.561197 damo-1.9.3/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-08-07 19:16:45.561197 damo-1.9.3/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7845 2023-08-07 19:16:41.000000 damo-1.9.3/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2022-04-22 09:53:30.000000 damo-1.9.3/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-08-07 19:16:45.561197 damo-1.9.3/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-13 14:44:13.000000 damo-1.9.3/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-07 19:16:45.549198 damo-1.9.3/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-07 19:16:45.561197 damo-1.9.3/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-08-07 19:16:41.000000 damo-1.9.3/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1442 2023-08-05 20:24:20.000000 damo-1.9.3/src/damo/_damo_ascii_color.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7357 2023-07-04 00:27:48.000000 damo-1.9.3/src/damo/_damo_deprecated.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-21 19:11:52.000000 damo-1.9.3/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9825 2023-07-15 19:33:44.000000 damo-1.9.3/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    36945 2023-08-01 16:47:08.000000 damo-1.9.3/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    15397 2023-07-30 18:25:59.000000 damo-1.9.3/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    16293 2023-06-24 19:25:59.000000 damo-1.9.3/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    28979 2023-08-02 23:20:58.000000 damo-1.9.3/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20236 2023-07-29 21:28:06.000000 damo-1.9.3/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3853 2023-07-23 17:09:22.000000 damo-1.9.3/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2023 2023-06-18 17:20:10.000000 damo-1.9.3/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      892 2023-06-18 18:06:08.000000 damo-1.9.3/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13603 2023-08-05 20:23:18.000000 damo-1.9.3/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3030 2023-07-04 00:27:48.000000 damo-1.9.3/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2743 2023-06-18 17:30:14.000000 damo-1.9.3/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5776 2023-07-08 17:18:37.000000 damo-1.9.3/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4094 2023-07-04 00:27:48.000000 damo-1.9.3/src/damo/damo_record_info.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1172 2023-07-04 00:27:48.000000 damo-1.9.3/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3723 2023-07-15 19:33:44.000000 damo-1.9.3/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1511 2023-06-17 18:37:36.000000 damo-1.9.3/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    25947 2023-08-06 18:26:51.000000 damo-1.9.3/src/damo/damo_show.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      599 2023-07-08 17:03:00.000000 damo-1.9.3/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3447 2023-07-30 17:59:22.000000 damo-1.9.3/src/damo/damo_status.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      701 2023-07-08 17:18:37.000000 damo-1.9.3/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      865 2023-05-29 19:12:16.000000 damo-1.9.3/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-20 19:08:28.000000 damo-1.9.3/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3929 2023-07-04 00:27:48.000000 damo-1.9.3/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-08-07 19:15:34.000000 damo-1.9.3/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5537 2023-07-15 19:33:44.000000 damo-1.9.3/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-08-07 19:16:45.561197 damo-1.9.3/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8366 2023-08-07 19:16:45.000000 damo-1.9.3/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1166 2023-08-07 19:16:45.000000 damo-1.9.3/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-08-07 19:16:45.000000 damo-1.9.3/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-08-07 19:16:45.000000 damo-1.9.3/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-08-07 19:16:45.000000 damo-1.9.3/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.9.2/PKG-INFO` & `damo-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.9.2
+Version: 1.9.3
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -45,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.2/README.md` & `damo-1.9.3/src/damo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: damo
+Version: 1.9.3
+Summary: DAMON user-space tool
+Home-page: https://github.com/awslabs/damo
+Author: SeongJae Park
+Author-email: sj@kernel.org
+Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
+Project-URL: DAMON, https://damonitor.github.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -30,16 +45,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -47,15 +62,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -75,19 +90,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.2/setup.py` & `damo-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_deprecated.py` & `damo-1.9.3/src/damo/_damo_deprecated.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_deprecation_notice.py` & `damo-1.9.3/src/damo/_damo_deprecation_notice.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_dist.py` & `damo-1.9.3/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_fmt_str.py` & `damo-1.9.3/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_fs.py` & `damo-1.9.3/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_paddr_layout.py` & `damo-1.9.3/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damo_subcmds.py` & `damo-1.9.3/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damon.py` & `damo-1.9.3/src/damo/_damon.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Contains core functions for DAMON control.
 """
 
 import collections
 import copy
 import os
+import random
 import time
 
 import _damo_fmt_str
 
 # Core data structures
 
 class DamonIntervals:
@@ -960,15 +961,15 @@
     idxs = running_kdamond_idxs()
     if len(idxs) == 0:
         return None
     if stats:
         err = update_schemes_stats(idxs)
         if err != None:
             return err
-    if tried_regions:
+    if tried_regions and feature_supported('schemes_tried_regions'):
         return update_schemes_tried_regions(idxs)
     return None
 
 def turn_damon_on(kdamonds_idxs):
     err = _damon_fs.turn_damon_on(kdamonds_idxs)
     if err:
         return err
```

### Comparing `damo-1.9.2/src/damo/_damon_args.py` & `damo-1.9.3/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damon_dbgfs.py` & `damo-1.9.3/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/_damon_result.py` & `damo-1.9.3/src/damo/_damon_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             nr_acc_to_add[r] = max(nr_acc_to_add[r],
                     region.nr_accesses.samples)
 
             new_regions = []
             if region.start < r.start:
                 new_regions.append(_damon.DamonRegion(
                     region.start, r.start,
-                    region.nr_accesses.samples, _damon.unit_samepls,
+                    region.nr_accesses.samples, _damon.unit_samples,
                     region.age.aggr_intervals, _damon.unit_aggr_intervals))
             if r.end < region.end:
                 new_regions.append(_damon.DamonRegion(
                         r.end, region.end,
                         region.nr_accesses.samples, _damon.unit_samples,
                         region.age.aggr_intervals,
                         _damon.unit_aggr_intervals))
```

### Comparing `damo-1.9.2/src/damo/_damon_sysfs.py` & `damo-1.9.3/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo.py` & `damo-1.9.3/src/damo/damo.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_adjust.py` & `damo-1.9.3/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_convert_record_format.py` & `damo-1.9.3/src/damo/damo_convert_record_format.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_features.py` & `damo-1.9.3/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_fmt_json.py` & `damo-1.9.3/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_heats.py` & `damo-1.9.3/src/damo/damo_heats.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import argparse
 import os
 import subprocess
 import sys
 import tempfile
 
+import _damo_ascii_color
 import _damo_fmt_str
 import _damon_result
 
 class HeatPixel:
     time = None
     addr = None
     heat = None
@@ -92,39 +93,24 @@
                 highest_heat = pixel.heat
             if lowest_heat == None or lowest_heat > pixel.heat:
                 lowest_heat = pixel.heat
     if highest_heat == None and lowest_heat == None:
         return
     heat_unit = float(highest_heat + 1 - lowest_heat) / 9
 
-    colorsets = {
-        'gray':[
-            [232] * 10,
-            [237, 239, 241, 243, 245, 247, 249, 251, 253, 255]],
-        'flame':[
-            [232, 1, 1, 2, 3, 3, 20, 21,26, 27, 27],
-            [239, 235, 237, 239, 243, 245, 247, 249, 251, 255]],
-        'emotion':[
-            [232, 234, 20, 21, 26, 2, 3, 1, 1, 1],
-            [239, 235, 237, 239, 243, 245, 247, 249, 251, 255]],
-        }
-    colors = colorsets[colorset]
     for snapshot in pixels:
         chars = []
         for pixel in snapshot:
             heat = int(float(pixel.heat - lowest_heat) / heat_unit)
-            heat = min(heat, len(colors[0]) - 1)
-            bg = colors[0][heat]
-            fg = colors[1][heat]
-            chars.append(u'\u001b[48;5;%dm\u001b[38;5;%dm%d' %
-                    (bg, fg, heat))
-        print(''.join(chars) + u'\u001b[0m')
-    color_samples = [u'\u001b[48;5;%dm\u001b[38;5;%dm %d ' %
-            (colors[0][i], colors[1][i], i) for i in range(10)]
-    print('# access_frequency: %s' % ''.join(color_samples) + u'\u001b[0m')
+            heat = min(heat, _damo_ascii_color.max_color_level())
+            chars.append('%s%d' %
+                    (_damo_ascii_color.color_mode_start_txt(colorset, heat),
+                        heat))
+        print(''.join(chars) + _damo_ascii_color.color_mode_end_txt())
+    print('# access_frequency: %s' % _damo_ascii_color.color_samples(colorset))
     print('# x-axis: space (%d-%d: %s)' % (addr_range[0], addr_range[1],
         _damo_fmt_str.format_sz(addr_range[1] - addr_range[0], False)))
     print('# y-axis: time (%d-%d: %s)' % (time_range[0], time_range[1],
         _damo_fmt_str.format_time_ns(time_range[1] - time_range[0], False)))
     print('# resolution: %dx%d (%s and %s for each character)' % (
         len(pixels[1]), len(pixels),
         _damo_fmt_str.format_sz(
@@ -352,23 +338,39 @@
             help='display absolute address in output')
 
     parser.add_argument('--guide', action='store_true',
             help='print a guidance for the ranges and resolution settings')
     parser.add_argument('--heatmap', metavar='<file>', type=str,
             help='heatmap image file to create.  stdout for terminal output')
     parser.add_argument('--stdout_heatmap_color',
-            choices=['gray', 'flame', 'emotion'], default='gray',
+            choices=['gray', 'flame', 'emotion'],
             help='color theme for access frequencies')
+    parser.add_argument('--ascii_color',
+            choices=['gray', 'flame', 'emotion'],
+            help='another name of stdout_heatmap_color')
+    parser.add_argument('--plot_ascii', action='store_true',
+            help='shortcut of \'--heatmap stdout\'')
 
 def main(args=None):
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
+    # --plot_ascii and --ascii_color is used in the demo screenshop[1].
+    # Support those.
+    #
+    # [1] https://sjp38.github.io/img/masim_stairs_heatmap_ascii.png
+    if args.heatmap == None and args.plot_ascii:
+        args.heatmap = 'stdout'
+    if args.ascii_color != None and args.stdout_heatmap_color == None:
+        args.stdout_heatmap_color = args.ascii_color
+    if args.ascii_color == None and args.stdout_heatmap_color == None:
+        args.stdout_heatmap_color = 'gray'
+
     records, err = _damon_result.parse_records_file(args.input)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (args.input, err))
         exit(1)
 
     # Use 80x40 resolution as default for ascii plot
```

### Comparing `damo-1.9.2/src/damo/damo_lru_sort.py` & `damo-1.9.3/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_monitor.py` & `damo-1.9.3/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_nr_regions.py` & `damo-1.9.3/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_reclaim.py` & `damo-1.9.3/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_record.py` & `damo-1.9.3/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_record_info.py` & `damo-1.9.3/src/damo/damo_record_info.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_report.py` & `damo-1.9.3/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_report_raw.py` & `damo-1.9.3/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_schemes.py` & `damo-1.9.3/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_show.py` & `damo-1.9.3/src/damo/damo_show.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,240 @@
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
+import collections
 import copy
 import json
+import math
 import os
 import random
 import time
 
+import _damo_ascii_color
 import _damo_fmt_str
 import _damon
 import _damon_args
 import _damon_result
 
-record_formatters = {
-        '<kdamond index>': lambda record, raw:
-            '%s' % record.kdamond_idx,
-        '<context index>': lambda record, raw:
-            '%s' % record.context_idx,
-        '<scheme index>': lambda record, raw:
-            '%s' % record.scheme_idx,
-        '<target id>': lambda record, raw:
-            '%s' % record.target_id,
-        '<record start abs time>': lambda record, raw:
+class Formatter:
+    keyword = None
+    format_fn = None
+    help_msg = None
+
+    def __init__(self, keyword, format_fn, help_msg):
+            self.keyword = keyword
+            self.format_fn = format_fn
+            self.help_msg = help_msg
+
+    def __str__(self):
+        return '%s\n%s' % (self.keyword, self.help_msg)
+
+record_formatters = [
+        Formatter('<kdamond index>',
+            lambda record, raw: '%s' % record.kdamond_idx,
+            'index of the record\'s kdamond'),
+        Formatter('<context index>',
+            lambda record, raw: '%s' % record.context_idx,
+            'index of the record\'s DAMON context'),
+        Formatter('<scheme index>',
+            lambda record, raw: '%s' % record.scheme_idx,
+            'index of the record\'s DAMOS scheme'),
+        Formatter('<target id>',
+            lambda record, raw: '%s' % record.target_id,
+            'index of the record\'s DAMON target'),
+        Formatter('<record start abs time>',
+            lambda record, raw:
             _dmo_fmt_str.format_ns(record.snapshots[0].start_time, raw),
-        '<record duration>': lambda record, raw:
+            'absolute time of the start of the record'),
+        Formatter('<record duration>',
+            lambda record, raw:
             _damo_fmt_str.format_time_ns(
                 record.snapshots[-1].end_time - record.snapshots[0].start_time,
-                raw)
-            }
-
-snapshot_formatters = {
-        '<total bytes>': lambda snapshot, record, raw:
+                raw),
+            'duration of the record'),
+        ]
+
+snapshot_formatters = [
+        Formatter('<total bytes>',
+            lambda snapshot, record, raw:
             _damo_fmt_str.format_sz(snapshot.total_bytes, raw),
-        '<monitor duration>': lambda snapshot, record, raw:
-            _damo_fmt_str.format_time_ns(
+            'total bytes of regions in the snapshot'),
+        Formatter('<monitor duration>',
+            lambda snapshot, record, raw: _damo_fmt_str.format_time_ns(
                 snapshot.end_time - snapshot.start_time, raw),
-        '<monitor start time>': lambda snapshot, record, raw:
-            _damo_fmt_str.format_time_ns(
+            'access monitoring duration for the snapshot'),
+        Formatter('<monitor start time>',
+            lambda snapshot, record, raw: _damo_fmt_str.format_time_ns(
                 snapshot.start_time - record.snapshots[0].start_time, raw),
-        '<monitor end time>': lambda snapshot, record, raw:
-            _damo_fmt_str.format_time_ns(
+            'access monitoring start time for the snapshot, relative to the record start time'),
+        Formatter('<monitor end time>',
+            lambda snapshot, record, raw: _damo_fmt_str.format_time_ns(
                 snapshot.end_time - record.snapshots[0].start_time, raw),
-        '<monitor start abs time>': lambda snapshot, record, raw:
+            'access monitoring end time for the snapshot, relative to the record end time'),
+        Formatter('<monitor start abs time>',
+            lambda snapshot, record, raw:
             _damo_fmt_str.format_time_ns(snapshot.start_time, raw),
-        '<monitor end abs time>': lambda snapshot, record, raw:
+            'absolute access monitoring start time for the snapshot'),
+        Formatter('<monitor end abs time>',
+            lambda snapshot, record, raw:
             _damo_fmt_str.format_time_ns(snapshot.end_time, raw),
-        '<number of regions>': lambda snapshot, record, raw:
+            'absolute access monitoring end time for the snapshot'),
+        Formatter('<number of regions>',
+            lambda snapshot, record, raw:
             _damo_fmt_str.format_nr(len(snapshot.regions), raw),
-            }
+            'the number of regions in the snapshot'),
+        ]
 
-region_formatters = {
-        '<index>': lambda index, region, raw, mms:
+region_formatters = [
+        Formatter('<index>',
+            lambda index, region, raw, rbargs:
             _damo_fmt_str.format_nr(index, raw),
-        '<start address>': lambda index, region, raw, mms:
+            'index of the region in the regions of the snapshot'),
+        Formatter('<start address>',
+            lambda index, region, raw, rbargs:
             _damo_fmt_str.format_sz(region.start, raw),
-        '<end address>': lambda index, region, raw, mms:
+            'start address of the region'),
+        Formatter('<end address>',
+            lambda index, region, raw, rbargs:
             _damo_fmt_str.format_sz(region.end, raw),
-        '<region size>': lambda index, region, raw, mms:
+            'end address of the region'),
+        Formatter('<region size>',
+            lambda index, region, raw, rbargs:
             _damo_fmt_str.format_sz(region.size(), raw),
-        '<access rate>': lambda index, region, raw, mms:
+            'size of the region'),
+        Formatter('<access rate>',
+            lambda index, region, raw, rbargs:
             _damo_fmt_str.format_percent(region.nr_accesses.percent, raw),
-        '<age>': lambda index, region, raw, mms:
+            'monitored access rate of the region'),
+        Formatter('<age>',
+            lambda index, region, raw, rbargs:
             _damo_fmt_str.format_time_us(region.age.usec, raw),
-        '<size bar>': lambda index, region, raw, mms:
-           size_bar(region, mms, 0, 20),
-        '<size heat bar>': lambda index, region, raw, mms:
-           size_heat_bar(region, mms, 1, 20),
-        '<size heat age bar>': lambda index, region, raw, mms:
-           size_heat_age_bar(region, mms, 1, 20),
-
-        }
+            'how long the access pattern of the region has maintained'),
+        Formatter('<size bar>',
+            lambda index, region, raw, rbargs:
+            rbargs.to_str(region, 'size', None, None),
+            'character box representing relative size of the region'),
+        Formatter('<size heat bar>',
+            lambda index, region, raw, rbargs:
+            rbargs.to_str(region, 'size', 'heat', None),
+           'character box representing relative size and access frequency of the region'),
+        Formatter('<age heat bar>',
+            lambda index, region, raw, rbargs:
+            rbargs.to_str(region, 'age', 'heat', None),
+            'character box represeting relative age and access frequency of the region'),
+        Formatter('<size heat age box>',
+            lambda index, region, raw, rbargs:
+            rbargs.to_str(region, 'size', 'heat', 'age'),
+            'character box representing relative size, access frequency, and the age of the region'),
+        Formatter('<box>',
+            lambda index, region, raw, rbargs:
+            rbargs.to_str(region, None, None, None),
+            'user-customizable (via --region_box_*) box (size-heat-age by default)'),
+        ]
 
 formatters = {
         'record': record_formatters,
         'snapshot': snapshot_formatters,
         'region': region_formatters
         }
 
-def __age_size_heat_box(region, record,
-        usec_per_column, bytes_per_row, nr_per_access_rate_percent):
+def rescale_val(val, orig_scale_minmax, new_scale_minmax):
+    '''Return a value in new scale
+
+    Parameters
+    ----------
+    val : int, float
+        The value to rescale
+    orig_scale_minmax : list
+        min/max values of original scale
+    new_scale_minmax : list
+        min/max values of new scale
+
+    Returns
+    -------
+    float
+        The rescaled value
     '''
-    Generate a string that represents a box.  The box represents age, size, and
-    heat of the region with length (number of columns), height (number of
-    rows), and number, respectively.
+    orig_length = orig_scale_minmax[1] - orig_scale_minmax[0]
+    new_length = new_scale_minmax[1] - new_scale_minmax[0]
+    ratio = new_length / orig_length if orig_length > 0 else 1
+    return (val - orig_scale_minmax[0]) * ratio + new_scale_minmax[0]
+
+def rescale_val_logscale(val, orig_scale_minmax, new_scale_minmax):
+    '''Return a value in new scale, in logscale
+
+    Parameters
+    ----------
+    val : int, float
+        The value to rescale
+    orig_scale_minmax : list
+        min/max values of original scale
+    new_scale_minmax : list
+        min/max values of new scale
+
+    Returns
+    -------
+    float
+        The rescaled value
     '''
-    nr_columns = int(region.age.usec / usec_per_column)
-    nr_rows = int(region.size() / bytes_per_row)
-    heat_nr = int(region.nr_accesses.percent / nr_per_access_rate_percent)
-    return '\n'.join([('%d' % heat_nr) * nr_columns] * nr_rows)
+    log_val = math.log(val, 2) if val > 0 else 0
+    log_minmax = [math.log(v, 2) if v > 0 else 0 for v in orig_scale_minmax]
+    return rescale_val(log_val, log_minmax, new_scale_minmax)
+
+class ColoredBox:
+    column_val = None
+    column_val_minmaxs = None
+
+    color_val = None
+    color_val_minmaxs = None
+    colorset = None
+
+    row_val = None
+    row_val_minmaxs = None
+
+    nr_columns_minmaxs = None
+    nr_rows_minmaxs = None
+
+    def __init__(self, column_val, column_val_minmaxs, nr_columns_minmaxs,
+            color_val, color_val_minmaxs, colorset,
+            row_val, row_val_minmaxs, nr_rows_minmaxs):
+        self.column_val = column_val
+        self.column_val_minmaxs = column_val_minmaxs
+        self.nr_columns_minmaxs = nr_columns_minmaxs
+
+        self.color_val = color_val
+        self.color_val_minmaxs = color_val_minmaxs
+        self.colorset = colorset
+
+        self.row_val = row_val
+        self.row_val_minmaxs = row_val_minmaxs
+        self.nr_rows_minmaxs = nr_rows_minmaxs
+
+    def __str__(self):
+        nr_cols = int(rescale_val_logscale(self.column_val,
+            self.column_val_minmaxs, self.nr_columns_minmaxs))
+
+        if self.row_val != None:
+            nr_rows = int(rescale_val_logscale(self.row_val,
+                self.row_val_minmaxs, self.nr_rows_minmaxs))
+        else:
+            nr_rows = 1
+
+        if type(self.color_val) == str:
+            row = '<%s>' % (self.color_val * nr_cols)
+        else:
+            color_level = int(rescale_val(self.color_val,
+                self.color_val_minmaxs, [0, 9]))
+            row = '<%s>' % _damo_ascii_color.colored(
+                    ('%d' % color_level) * nr_cols, self.colorset, color_level)
+
+        rows = '\n'.join([row] * nr_rows)
+        if nr_rows > 1:
+            rows += '\n'
+        return rows
 
 class MinMaxOfRecords:
     min_sz_region = None
     max_sz_region = None
     min_access_rate_percent = None
     max_access_rate_percent = None
     min_age_us = None
@@ -118,66 +261,67 @@
 
     def __init__(self, records):
         for record in records:
             for snapshot in record.snapshots:
                 for region in snapshot.regions:
                     self.set_fields(region, record.intervals)
 
-def rescale_val(val, orig_scale_minmax, new_scale_minmax):
-    '''Return a value in new scale
-
-    Parameters
-    ----------
-    val : int, float
-        The value to rescale
-    orig_scale_minmax : list
-        min/max values of original scale
-    new_scale_minmax : list
-        min/max values of new scale
-
-    Returns
-    -------
-    float
-        The rescaled value
-    '''
-    orig_length = orig_scale_minmax[1] - orig_scale_minmax[0]
-    new_length = new_scale_minmax[1] - new_scale_minmax[0]
-    ratio = new_length / orig_length if orig_length > 0 else 1
-    return (val - orig_scale_minmax[0]) * ratio + new_scale_minmax[0]
-
-def size_bar(region, minmaxs, min_cols, max_cols):
-    print(region.size())
-    nr_cols = int(rescale_val(region.size(),
-            [minmaxs.min_sz_region, minmaxs.max_sz_region],
-            [min_cols, max_cols]))
-    return '<%s>' % ('-' * nr_cols)
-
-def size_heat_bar(region, minmaxs, min_cols, max_cols):
-    nr_cols = int(rescale_val(region.size(),
-            [minmaxs.min_sz_region, minmaxs.max_sz_region],
-            [min_cols, max_cols]))
-    heat_symbol = int(rescale_val(region.nr_accesses.percent,
-        [minmaxs.min_access_rate_percent, minmaxs.max_access_rate_percent],
-        [0, 9]))
-
-    return '<%s>' % ('%d' % heat_symbol * nr_cols)
-
-def size_heat_age_bar(region, minmaxs, min_cols, max_cols):
-    nr_cols = int(rescale_val(region.size(),
-            [minmaxs.min_sz_region, minmaxs.max_sz_region],
-            [min_cols, max_cols]))
-    heat_symbol = int(rescale_val(region.nr_accesses.percent,
-        [minmaxs.min_access_rate_percent, minmaxs.max_access_rate_percent],
-        [0, 9]))
-    nr_rows = int(rescale_val(region.age.usec,
-        [minmaxs.min_age_us, minmaxs.max_age_us],
-        [1, 5]))
-
-    row = '<%s>' % ('%d' % heat_symbol * nr_cols)
-    return '\n'.join([row] * nr_rows) + '\n'
+class RegionBoxArgs:
+    record_minmaxs = None
+    min_max_cols = None
+    min_max_rows = None
+    colorset = None
+
+    col_val_name = None
+    color_val_name = None
+    row_val_name = None
+
+    def __init__(self, record_minmaxs, min_max_cols, min_max_rows, colorset,
+            col_val_name=None, color_val_name=None, row_val_name=None):
+        self.record_minmaxs = record_minmaxs
+        self.min_max_cols = min_max_cols
+        self.min_max_rows = min_max_rows
+        self.colorset = colorset
+        self.col_val_name = col_val_name
+        self.color_val_name = color_val_name
+        self.row_val_name = row_val_name
+
+    def val_minmax(self, region, value_name):
+        mms = self.record_minmaxs
+        if value_name == 'size':
+            return region.size(), [mms.min_sz_region, mms.max_sz_region]
+        elif value_name in ['heat', 'access_rate']:
+            return region.nr_accesses.percent, [
+                    mms.min_access_rate_percent, mms.max_access_rate_percent]
+        elif value_name == 'age':
+            return region.age.usec, [mms.min_age_us, mms.max_age_us]
+        return None, None
+
+    def to_str(self, region, col_val_name, color_val_name, row_val_name):
+        if col_val_name == None:
+            col_val_name = self.col_val_name
+        if color_val_name == None:
+            color_val_name = self.color_val_name
+        if row_val_name == None:
+            row_val_name = self.row_val_name
+
+        if (col_val_name == None and color_val_name == None and
+                row_val_name == None):
+            col_val_name = 'size'
+            color_val_name = 'heat'
+            row_val_name = 'age'
+
+        cval, cval_minmax = self.val_minmax(region, col_val_name)
+        clval, clval_minmax = self.val_minmax(region, color_val_name)
+        if clval == None:
+            clval = '-'
+        rval, rval_minmax = self.val_minmax(region, row_val_name)
+        return '%s' % ColoredBox(cval, cval_minmax, self.min_max_cols,
+                clval, clval_minmax, self.colorset,
+                rval, rval_minmax, self.min_max_rows)
 
 def apply_min_chars(min_chars, field_name, txt):
     # min_chars: [[<field name>, <number of min chars>]...]
     for name, nr in min_chars:
         try:
             nr = int(nr)
         except:
@@ -186,27 +330,29 @@
         if name == field_name:
             if len(txt) >= nr:
                 return txt
             txt += ' ' * (nr - len(txt))
             return txt
     return txt
 
-def format_pr(template, min_chars, index, region, snapshot, record, raw, mms):
+def format_pr(template, min_chars, index, region, snapshot, record, raw, mms,
+        region_box_args):
     if template == '':
         return
     for category, category_formatters in formatters.items():
-        for field_name, formatter in category_formatters.items():
+        for formatter in category_formatters:
+            field_name = formatter.keyword
             if template.find(field_name) == -1:
                 continue
             if category == 'record':
-                txt = formatter(record, raw)
+                txt = formatter.format_fn(record, raw)
             elif category == 'snapshot':
-                txt = formatter(snapshot, record, raw)
+                txt = formatter.format_fn(snapshot, record, raw)
             elif category == 'region':
-                txt = formatter(index, region, raw, mms)
+                txt = formatter.format_fn(index, region, raw, region_box_args)
             txt = apply_min_chars(min_chars, field_name, txt)
             template = template.replace(field_name, txt)
     template = template.replace('\\n', '\n')
     print(template)
 
 def set_formats(args, records):
     if args.format_record_head == None:
@@ -246,37 +392,44 @@
     if args.json:
         print(json.dumps([r.to_kvpairs(args.raw_number)
             for r in records], indent=4))
         exit(0)
 
     set_formats(args, records)
     mms = MinMaxOfRecords(records)
+    region_box_args = RegionBoxArgs(mms, args.region_box_min_max_cols,
+            args.region_box_min_max_rows, args.region_box_colorset,
+            args.region_box_values[0], args.region_box_values[1],
+            args.region_box_values[2])
 
     for record in records:
         format_pr(args.format_record_head, args.min_chars_field, None, None,
-                None, record, args.raw_number, mms)
+                None, record, args.raw_number, mms, region_box_args)
         snapshots = record.snapshots
 
         for sidx, snapshot in enumerate(snapshots):
             format_pr(args.format_snapshot_head, args.min_chars_field, None,
-                    None, snapshot, record, args.raw_number, mms)
+                    None, snapshot, record, args.raw_number, mms,
+                    region_box_args)
             for r in snapshot.regions:
                 r.nr_accesses.add_unset_unit(record.intervals)
                 r.age.add_unset_unit(record.intervals)
             for idx, r in enumerate(
                     sorted_regions(snapshot.regions, args.sort_regions_by)):
                 format_pr(args.format_region, args.min_chars_field, idx, r,
-                        snapshot, record, args.raw_number, mms)
+                        snapshot, record, args.raw_number, mms,
+                        region_box_args)
             format_pr(args.format_snapshot_tail, args.min_chars_field, None,
-                    None, snapshot, record, args.raw_number, mms)
+                    None, snapshot, record, args.raw_number, mms,
+                    region_box_args)
 
             if sidx < len(snapshots) - 1 and not args.total_sz_only:
                 print('')
         format_pr(args.format_record_tail, args.min_chars_field, None, None,
-                None, record, args.raw_number, mms)
+                None, record, args.raw_number, mms, region_box_args)
 
 def filter_by_pattern(record, access_pattern):
     sz_bytes = access_pattern.sz_bytes
     nr_acc = access_pattern.nr_acc_min_max
     age = access_pattern.age_min_max
 
     for snapshot in record.snapshots:
@@ -372,22 +525,41 @@
     # don't set default for record head and snapshot head because it depends on
     # given number of record and snapshots.  Decide those in set_formats().
     parser.add_argument('--format_record_head', metavar='<template>',
             help='record output head format')
     parser.add_argument('--format_record_tail', metavar='<template>',
             default='',
             help='record output tail format')
+    parser.add_argument('--ls_record_format_keywords', action='store_true',
+            help='list available record format keywords')
     parser.add_argument('--format_snapshot_head', metavar='<template>',
             help='snapshot output tail format')
     parser.add_argument('--format_snapshot_tail', metavar='<template>',
             default='total size: <total bytes>',
             help='snapshot output tail format')
+    parser.add_argument('--ls_snapshot_format_keywords', action='store_true',
+            help='list available snapshot format keywords')
     parser.add_argument('--format_region', metavar='<template>',
             default='<index> addr [<start address>, <end address>) (<region size>) access <access rate> age <age>',
             help='region output format')
+    parser.add_argument('--ls_region_format_keywords', action='store_true',
+            help='list available region format keywords')
+    parser.add_argument('--region_box_values',
+            choices=['size', 'access_rate', 'age', 'none'], nargs=3,
+            default=['none', 'none', 'none'],
+            help='values to show via the box\'s length, color, and height')
+    parser.add_argument('--region_box_min_max_cols', nargs=2, type=int,
+            metavar=('<min>', '<max>'), default=[1, 30],
+            help='minimum and maximum number of columns for region box')
+    parser.add_argument('--region_box_min_max_rows', nargs=2, type=int,
+            metavar=('<min>', '<max>'), default=[1, 5],
+            help='minimum and maximum number of rows for region box')
+    parser.add_argument('--region_box_colorset', default='gray',
+            choices=['gray', 'flame', 'emotion'],
+            help='colorset to use for region box')
     parser.add_argument('--min_chars_field', nargs=2,
             metavar=('<field name>', '<number>'), action='append',
             default=[['<index>', 3],
                 ['<start address>', 12],['<end address>', 11],
                 ['<region size>', 11], ['<access rate>', 5]],
             help='minimum character for each field')
     parser.add_argument('--total_sz_only', action='store_true',
@@ -408,18 +580,31 @@
 
 def main(args=None):
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
+    args.region_box_values = [v if v != 'none' else None
+            for v in args.region_box_values]
+
     access_pattern = _damon.DamosAccessPattern(args.sz_region,
             args.access_rate, _damon.unit_percent, args.age * 1000000,
             _damon.unit_usec)
 
+    if args.ls_record_format_keywords:
+        print('\n\n'.join(['%s' % f for f in record_formatters]))
+        return
+    if args.ls_snapshot_format_keywords:
+        print('\n\n'.join(['%s' % f for f in snapshot_formatters]))
+        return
+    if args.ls_region_format_keywords:
+        print('\n\n'.join(['%s' % f for f in region_formatters]))
+        return
+
     if args.input_file == None:
         _damon.ensure_root_and_initialized(args)
         err = 'assumed error'
         nr_tries = 0
         while err != None and nr_tries < 5:
             nr_tries += 1
             if args.tried_regions_of == None:
```

### Comparing `damo-1.9.2/src/damo/damo_start.py` & `damo-1.9.3/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_status.py` & `damo-1.9.3/src/damo/damo_status.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_stop.py` & `damo-1.9.3/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_translate_damos.py` & `damo-1.9.3/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_tune.py` & `damo-1.9.3/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_validate.py` & `damo-1.9.3/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo/damo_wss.py` & `damo-1.9.3/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.9.2/src/damo.egg-info/PKG-INFO` & `damo-1.9.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: damo
-Version: 1.9.2
-Summary: DAMON user-space tool
-Home-page: https://github.com/awslabs/damo
-Author: SeongJae Park
-Author-email: sj@kernel.org
-Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
-Project-URL: DAMON, https://damonitor.github.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -45,16 +30,16 @@
     $ # install from PyPI, or use your distribution's package manager
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.2/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.3/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.9.3/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -62,15 +47,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -90,19 +75,19 @@
 How can I participate in the development of `damo`?
 ---------------------------------------------------
 
 Please refer to
 [CONTRIBUTING](https://github.com/awslabs/damo/blob/next/CONTRIBUTING) file.
 
 
-Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) file?
+Why some subcommands are not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) file?
 ---------------------------------------------------------------------
 
 Only sufficiently stabilized features are documented there.  In other words,
-any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.2/USAGE.md) are in experimental
+any feature that not documented on [USAGE.md](https://github.com/awslabs/damo/blob/v1.9.3/USAGE.md) are in experimental
 stage.  Such experimental features could be deprecated and removed without any
 notice and grace priods.  The documented features could also be deprecated, but
 those will provide some notification and grace periods.
 
 
 Recording Data Access Patterns
 ==============================
```

### Comparing `damo-1.9.2/src/damo.egg-info/SOURCES.txt` & `damo-1.9.3/src/damo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 setup.py
 src/damo/__init__.py
+src/damo/_damo_ascii_color.py
 src/damo/_damo_deprecated.py
 src/damo/_damo_deprecation_notice.py
 src/damo/_damo_dist.py
 src/damo/_damo_fmt_str.py
 src/damo/_damo_fs.py
 src/damo/_damo_paddr_layout.py
 src/damo/_damo_subcmds.py
```

