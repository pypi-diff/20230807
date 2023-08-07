# Comparing `tmp/mkdocs-macros-plugin-1.0.2.tar.gz` & `tmp/mkdocs-macros-plugin-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-macros-plugin-1.0.2.tar", last modified: Wed Jul 12 10:57:08 2023, max compression
+gzip compressed data, was "mkdocs-macros-plugin-1.0.4.tar", last modified: Mon Aug  7 15:01:44 2023, max compression
```

## Comparing `mkdocs-macros-plugin-1.0.2.tar` & `mkdocs-macros-plugin-1.0.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/.github/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/.github/workflows/
--rw-r--r--   0 laurent    (501) staff       (20)      457 2020-03-10 06:37:22.000000 mkdocs-macros-plugin-1.0.2/.github/workflows/greetings.yml
--rw-r--r--   0 laurent    (501) staff       (20)      423 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.2/.gitignore
--rw-r--r--   0 laurent    (501) staff       (20)      601 2021-04-23 13:52:57.000000 mkdocs-macros-plugin-1.0.2/.readthedocs.yml
--rw-r--r--   0 laurent    (501) staff       (20)     4611 2023-07-02 17:49:04.000000 mkdocs-macros-plugin-1.0.2/CHANGELOG.md
--rw-r--r--   0 laurent    (501) staff       (20)     1134 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.2/LICENSE.md
--rw-r--r--   0 laurent    (501) staff       (20)       64 2020-11-22 09:50:49.000000 mkdocs-macros-plugin-1.0.2/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     6692 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.2/README.md
--rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-02-24 19:02:56.000000 mkdocs-macros-plugin-1.0.2/macros_info.png
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/
--rw-rw-r--   0 laurent    (501) staff       (20)      234 2021-01-04 17:04:12.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)    11781 2023-07-03 06:44:13.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/context.py
--rw-r--r--   0 laurent    (501) staff       (20)     1073 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/errors.py
--rw-r--r--   0 laurent    (501) staff       (20)     1604 2023-04-22 15:06:54.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/macros_info.md
--rw-r--r--   0 laurent    (501) staff       (20)    27055 2023-07-02 14:52:08.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/plugin.py
--rwxr-xr-x   0 laurent    (501) staff       (20)     6562 2022-03-16 08:10:30.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/util.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-07-12 10:57:04.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     1759 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       60 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/entry_points.txt
--rw-r--r--   0 laurent    (501) staff       (20)      132 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)       14 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/top_level.txt
--rw-r--r--   0 laurent    (501) staff       (20)       38 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     1923 2023-07-02 17:49:16.000000 mkdocs-macros-plugin-1.0.2/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/debug/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/debug/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      129 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.2/test/debug/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      223 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.2/test/debug/mkdocs.yml
--rw-rw-r--   0 laurent    (501) staff       (20)     1277 2020-02-23 06:57:46.000000 mkdocs-macros-plugin-1.0.2/test/main_sample.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/module/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      361 2023-07-02 09:57:52.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/environment.md
--rw-r--r--   0 laurent    (501) staff       (20)     2372 2023-07-02 09:55:13.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      357 2021-04-21 16:34:52.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/literal.md
--rw-r--r--   0 laurent    (501) staff       (20)      165 2023-07-02 13:51:07.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/other.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/module/include/
--rw-r--r--   0 laurent    (501) staff       (20)       68 2021-06-19 05:35:28.000000 mkdocs-macros-plugin-1.0.2/test/module/include/foo.md
--rw-r--r--   0 laurent    (501) staff       (20)     2023 2023-04-23 08:53:11.000000 mkdocs-macros-plugin-1.0.2/test/module/main.py
--rw-r--r--   0 laurent    (501) staff       (20)      518 2023-07-02 10:41:31.000000 mkdocs-macros-plugin-1.0.2/test/module/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      237 2022-03-25 19:54:47.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/docs/environment.md
--rw-r--r--   0 laurent    (501) staff       (20)      529 2023-07-02 09:54:23.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/include/
--rw-r--r--   0 laurent    (501) staff       (20)       68 2020-03-02 21:15:58.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/include/foo.md
--rw-r--r--   0 laurent    (501) staff       (20)      281 2020-09-25 16:31:43.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/mymodule/
--rw-r--r--   0 laurent    (501) staff       (20)      685 2021-06-19 08:12:07.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/mymodule/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      160 2020-09-28 06:50:54.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      138 2020-03-22 11:26:31.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/main.py
--rw-r--r--   0 laurent    (501) staff       (20)      336 2020-09-28 06:42:49.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/docs/
--rw-r--r--   0 laurent    (501) staff       (20)       62 2023-04-22 10:48:15.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/docs/page_with_macros.md
--rw-r--r--   0 laurent    (501) staff       (20)      257 2023-04-22 13:36:25.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      160 2023-04-22 11:13:20.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/docs/page_with_macros.md
--rw-r--r--   0 laurent    (501) staff       (20)      255 2023-04-22 13:35:37.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/simple/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/simple/docs/
--rw-r--r--   0 laurent    (501) staff       (20)       21 2020-03-04 11:55:35.000000 mkdocs-macros-plugin-1.0.2/test/simple/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      138 2020-09-15 20:07:40.000000 mkdocs-macros-plugin-1.0.2/test/simple/main_old.py
--rw-r--r--   0 laurent    (501) staff       (20)       92 2020-02-24 18:30:04.000000 mkdocs-macros-plugin-1.0.2/test/simple/mkdocs.yml
--rwxr-xr-x   0 laurent    (501) staff       (20)     1119 2020-10-03 09:23:32.000000 mkdocs-macros-plugin-1.0.2/update_pypi.sh
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/webdoc/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     7677 2023-04-24 07:59:08.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/advanced.md
--rw-r--r--   0 laurent    (501) staff       (20)       50 2021-04-23 09:53:10.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/changelog.md
--rw-r--r--   0 laurent    (501) staff       (20)     2338 2021-04-24 11:27:05.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/contribute.md
--rw-r--r--   0 laurent    (501) staff       (20)    23462 2020-05-15 08:53:26.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/dog-eating.jpg
--rw-r--r--   0 laurent    (501) staff       (20)     3998 2022-01-26 01:22:27.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/git_info.md
--rw-r--r--   0 laurent    (501) staff       (20)      960 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/help.md
--rw-r--r--   0 laurent    (501) staff       (20)     9232 2023-04-24 07:30:46.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)     1081 2020-03-10 08:29:58.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/license.md
--rw-r--r--   0 laurent    (501) staff       (20)    13954 2023-04-23 09:30:47.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/macros.md
--rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-03-10 08:57:11.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/macros_info.png
--rw-r--r--   0 laurent    (501) staff       (20)     7420 2023-07-03 05:17:35.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/pages.md
--rw-r--r--   0 laurent    (501) staff       (20)     5693 2021-09-09 06:43:39.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/pluglets.md
--rw-r--r--   0 laurent    (501) staff       (20)    10756 2023-04-23 11:02:22.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/post_production.md
--rw-r--r--   0 laurent    (501) staff       (20)     9834 2023-04-23 14:23:38.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/rendering.md
--rw-r--r--   0 laurent    (501) staff       (20)     8741 2023-07-02 18:14:07.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/tips.md
--rw-r--r--   0 laurent    (501) staff       (20)    10171 2023-04-23 19:17:25.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/troubleshooting.md
--rw-r--r--   0 laurent    (501) staff       (20)     7478 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/why.md
--rw-r--r--   0 laurent    (501) staff       (20)       51 2021-04-23 13:51:49.000000 mkdocs-macros-plugin-1.0.2/webdoc/extra_requirements.txt
--rw-r--r--   0 laurent    (501) staff       (20)     1383 2023-04-23 14:27:56.000000 mkdocs-macros-plugin-1.0.2/webdoc/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/.github/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/.github/workflows/
+-rw-r--r--   0 laurent    (501) staff       (20)      457 2020-03-10 06:37:22.000000 mkdocs-macros-plugin-1.0.4/.github/workflows/greetings.yml
+-rw-r--r--   0 laurent    (501) staff       (20)      423 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.4/.gitignore
+-rw-r--r--   0 laurent    (501) staff       (20)      601 2021-04-23 13:52:57.000000 mkdocs-macros-plugin-1.0.4/.readthedocs.yml
+-rw-r--r--   0 laurent    (501) staff       (20)     4789 2023-08-07 15:00:38.000000 mkdocs-macros-plugin-1.0.4/CHANGELOG.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1134 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.4/LICENSE.md
+-rw-r--r--   0 laurent    (501) staff       (20)       64 2020-11-22 09:50:49.000000 mkdocs-macros-plugin-1.0.4/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     6692 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.4/README.md
+-rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-02-24 19:02:56.000000 mkdocs-macros-plugin-1.0.4/macros_info.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/
+-rw-rw-r--   0 laurent    (501) staff       (20)      234 2021-01-04 17:04:12.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)    11834 2023-07-16 09:12:56.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/context.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1073 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/errors.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1604 2023-04-22 15:06:54.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/macros_info.md
+-rw-r--r--   0 laurent    (501) staff       (20)    27055 2023-07-02 14:52:08.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/plugin.py
+-rwxr-xr-x   0 laurent    (501) staff       (20)     6764 2023-08-03 14:37:40.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros/util.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-08-07 15:01:40.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     1759 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-08-07 15:01:40.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       60 2023-08-07 15:01:40.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      132 2023-08-07 15:01:40.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       14 2023-08-07 15:01:40.000000 mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/top_level.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       38 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     1923 2023-08-03 14:42:55.000000 mkdocs-macros-plugin-1.0.4/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/test/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/test/debug/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/test/debug/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      129 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.4/test/debug/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      223 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.4/test/debug/mkdocs.yml
+-rw-rw-r--   0 laurent    (501) staff       (20)     1277 2020-02-23 06:57:46.000000 mkdocs-macros-plugin-1.0.4/test/main_sample.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/test/module/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/test/module/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      361 2023-07-02 09:57:52.000000 mkdocs-macros-plugin-1.0.4/test/module/docs/environment.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2372 2023-07-02 09:55:13.000000 mkdocs-macros-plugin-1.0.4/test/module/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      357 2021-04-21 16:34:52.000000 mkdocs-macros-plugin-1.0.4/test/module/docs/literal.md
+-rw-r--r--   0 laurent    (501) staff       (20)      165 2023-07-02 13:51:07.000000 mkdocs-macros-plugin-1.0.4/test/module/docs/other.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:43.000000 mkdocs-macros-plugin-1.0.4/test/module/include/
+-rw-r--r--   0 laurent    (501) staff       (20)       68 2021-06-19 05:35:28.000000 mkdocs-macros-plugin-1.0.4/test/module/include/foo.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2023 2023-04-23 08:53:11.000000 mkdocs-macros-plugin-1.0.4/test/module/main.py
+-rw-r--r--   0 laurent    (501) staff       (20)      564 2023-07-16 09:03:29.000000 mkdocs-macros-plugin-1.0.4/test/module/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      237 2022-03-25 19:54:47.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/docs/environment.md
+-rw-r--r--   0 laurent    (501) staff       (20)      529 2023-07-02 09:54:23.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/include/
+-rw-r--r--   0 laurent    (501) staff       (20)       68 2020-03-02 21:15:58.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/include/foo.md
+-rw-r--r--   0 laurent    (501) staff       (20)      281 2020-09-25 16:31:43.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/mymodule/
+-rw-r--r--   0 laurent    (501) staff       (20)      685 2021-06-19 08:12:07.000000 mkdocs-macros-plugin-1.0.4/test/module_dir/mymodule/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/new_syntax/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/new_syntax/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      160 2020-09-28 06:50:54.000000 mkdocs-macros-plugin-1.0.4/test/new_syntax/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      138 2020-03-22 11:26:31.000000 mkdocs-macros-plugin-1.0.4/test/new_syntax/main.py
+-rw-r--r--   0 laurent    (501) staff       (20)      336 2020-09-28 06:42:49.000000 mkdocs-macros-plugin-1.0.4/test/new_syntax/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/opt-in/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/opt-in/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)       62 2023-04-22 10:48:15.000000 mkdocs-macros-plugin-1.0.4/test/opt-in/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.4/test/opt-in/docs/page_with_macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)      257 2023-04-22 13:36:25.000000 mkdocs-macros-plugin-1.0.4/test/opt-in/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/opt-out/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/opt-out/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      160 2023-04-22 11:13:20.000000 mkdocs-macros-plugin-1.0.4/test/opt-out/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.4/test/opt-out/docs/page_with_macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)      255 2023-04-22 13:35:37.000000 mkdocs-macros-plugin-1.0.4/test/opt-out/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/simple/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/test/simple/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)       21 2020-03-04 11:55:35.000000 mkdocs-macros-plugin-1.0.4/test/simple/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      138 2020-09-15 20:07:40.000000 mkdocs-macros-plugin-1.0.4/test/simple/main_old.py
+-rw-r--r--   0 laurent    (501) staff       (20)       92 2020-02-24 18:30:04.000000 mkdocs-macros-plugin-1.0.4/test/simple/mkdocs.yml
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1119 2020-10-03 09:23:32.000000 mkdocs-macros-plugin-1.0.4/update_pypi.sh
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/webdoc/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-08-07 15:01:44.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7677 2023-04-24 07:59:08.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/advanced.md
+-rw-r--r--   0 laurent    (501) staff       (20)       50 2021-04-23 09:53:10.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/changelog.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2338 2021-04-24 11:27:05.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/contribute.md
+-rw-r--r--   0 laurent    (501) staff       (20)    23462 2020-05-15 08:53:26.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/dog-eating.jpg
+-rw-r--r--   0 laurent    (501) staff       (20)     3998 2022-01-26 01:22:27.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/git_info.md
+-rw-r--r--   0 laurent    (501) staff       (20)      960 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/help.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9232 2023-04-24 07:30:46.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1081 2020-03-10 08:29:58.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/license.md
+-rw-r--r--   0 laurent    (501) staff       (20)    13954 2023-04-23 09:30:47.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-03-10 08:57:11.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/macros_info.png
+-rw-r--r--   0 laurent    (501) staff       (20)     7420 2023-07-03 05:17:35.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/pages.md
+-rw-r--r--   0 laurent    (501) staff       (20)     5693 2021-09-09 06:43:39.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/pluglets.md
+-rw-r--r--   0 laurent    (501) staff       (20)    10756 2023-04-23 11:02:22.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/post_production.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9834 2023-04-23 14:23:38.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/rendering.md
+-rw-r--r--   0 laurent    (501) staff       (20)     8741 2023-07-02 18:14:07.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/tips.md
+-rw-r--r--   0 laurent    (501) staff       (20)    10171 2023-04-23 19:17:25.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/troubleshooting.md
+-rw-r--r--   0 laurent    (501) staff       (20)     7478 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-1.0.4/webdoc/docs/why.md
+-rw-r--r--   0 laurent    (501) staff       (20)       51 2021-04-23 13:51:49.000000 mkdocs-macros-plugin-1.0.4/webdoc/extra_requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)     1383 2023-04-23 14:27:56.000000 mkdocs-macros-plugin-1.0.4/webdoc/mkdocs.yml
```

### Comparing `mkdocs-macros-plugin-1.0.2/.readthedocs.yml` & `mkdocs-macros-plugin-1.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/CHANGELOG.md` & `mkdocs-macros-plugin-1.0.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog: mkdocs-macros
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.0.4, 2023-08-07
+
+* Fixed: Warning due to filter issue with mkdocs >= 1.5
+* Fixed: Debug html tables (including for `macro_info()`) are 
+    now readable also in dark mode.
+
 ## 1.0.2, 2023-07-02
 * Added: it is now possible to use macros in page titles, in the
     nav section of the yaml file, or in the level 1 titles; 
     the macros are correctly interpreted in the navigation part
     of the page.
 
 ## 1.0.1, 2023-05-25
```

### Comparing `mkdocs-macros-plugin-1.0.2/LICENSE.md` & `mkdocs-macros-plugin-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/PKG-INFO` & `mkdocs-macros-plugin-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-plugin
-Version: 1.0.2
+Version: 1.0.4
 Summary: Unleash the power of MkDocs with macros and variables
 Home-page: https://github.com/fralau/mkdocs_macros_plugin
 Author: Laurent Franceschbetti
 Author-email: info@settlenext.com
 License: MIT
 Keywords: mkdocs python markdown macros
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-macros-plugin-1.0.2/README.md` & `mkdocs-macros-plugin-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/macros_info.png` & `mkdocs-macros-plugin-1.0.4/macros_info.png`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros/context.py` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,20 +103,21 @@
                 r_list.append("<b>%s</b> [<i>%s</i>]" %
                               (key, type(value).__name__))
         return ', '.join(r_list)
     else:
         return repr(value)
 
 
-def make_html(rows, header=[], tb_class='pretty'):
+def make_html(rows, header=[], tb_class='macros-tb'):
     "Produce an HTML table"
+    font_color = "#000000"  # black
     back_color = "#F0FFFF"  # light blue
     grid_color = "#DCDCDC"
     padding = "5px"
-    style = "border:1px solid %s; padding: %s" % (grid_color, padding)
+    style = f"color:{font_color}; border:1px solid {grid_color}; padding: {padding}"
     templ = Template("""
 <table class="{{ tb_class }}" style="background-color: {{ back_color}}; {{ style }}">
     {% for item in header %}
     <th style="{{ style }}">{{ item }}</th>
     {% endfor %}
     {% for row in rows %}
         <tr>
```

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros/errors.py` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros/errors.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros/macros_info.md` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros/macros_info.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros/plugin.py` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros/util.py` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 """
 Utilities for mkdocs-macros
 """
 
 import subprocess
 from copy import deepcopy
 import os, sys, importlib.util
+from packaging.version import Version
 
 from termcolor import colored
+import mkdocs
 
 # ------------------------------------------
 # Trace and debug
 # ------------------------------------------
 TRACE_COLOR = 'green'
 TRACE_PREFIX = 'macros' 
 
 import logging
-from mkdocs.utils import warning_filter
 LOG = logging.getLogger("mkdocs.plugins." + __name__)
-LOG.addFilter(warning_filter)
+
+MKDOCS_LOG_VERSION = '1.2'
+if Version(mkdocs.__version__) < Version(MKDOCS_LOG_VERSION):
+    # filter doesn't do anything since that version
+    from mkdocs.utils import warning_filter
+    LOG.addFilter(warning_filter)
 
 
 def format_trace(*args):
     """
     General purpose print function, as trace,
     for the mkdocs-macros framework;
     it will appear if --verbose option is activated
```

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/PKG-INFO` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-plugin
-Version: 1.0.2
+Version: 1.0.4
 Summary: Unleash the power of MkDocs with macros and variables
 Home-page: https://github.com/fralau/mkdocs_macros_plugin
 Author: Laurent Franceschbetti
 Author-email: info@settlenext.com
 License: MIT
 Keywords: mkdocs python markdown macros
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/SOURCES.txt` & `mkdocs-macros-plugin-1.0.4/mkdocs_macros_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/setup.py` & `mkdocs-macros-plugin-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 
 # --------------------
 # Initialization
 # --------------------
 
-VERSION_NUMBER = '1.0.2'
+VERSION_NUMBER = '1.0.4'
 
 # required if you want to run document/test
 # pip install 'mkdocs-macros-plugin[test]'
 TEST_REQUIRE = ['mkdocs-macros-test', 'mkdocs-material>=6.2',
                 'mkdocs-include-markdown-plugin']
 
 # --------------------
```

### Comparing `mkdocs-macros-plugin-1.0.2/test/main_sample.py` & `mkdocs-macros-plugin-1.0.4/test/main_sample.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/test/module/docs/index.md` & `mkdocs-macros-plugin-1.0.4/test/module/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/test/module/main.py` & `mkdocs-macros-plugin-1.0.4/test/module/main.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/test/module/mkdocs.yml` & `mkdocs-macros-plugin-1.0.4/test/module/mkdocs.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 site_name: Main test site
-theme: material
+theme: 
+    name: material
+    palette:
+        scheme: slate
 copyright: (C) Laurent Franceschetti 2020
 
 nav:
     - Home: index.md
     - Environment for {{ unit_price}}: environment.md
     - Second:
         - other.md
```

### Comparing `mkdocs-macros-plugin-1.0.2/test/module_dir/docs/index.md` & `mkdocs-macros-plugin-1.0.4/test/module_dir/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/test/module_dir/mymodule/__init__.py` & `mkdocs-macros-plugin-1.0.4/test/module_dir/mymodule/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/update_pypi.sh` & `mkdocs-macros-plugin-1.0.4/update_pypi.sh`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/advanced.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/contribute.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/dog-eating.jpg` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/dog-eating.jpg`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/git_info.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/git_info.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/help.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/help.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/index.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/license.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/license.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/macros.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/macros.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/macros_info.png` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/macros_info.png`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/pages.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/pages.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/pluglets.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/pluglets.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/post_production.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/post_production.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/rendering.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/rendering.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/tips.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/tips.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/troubleshooting.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/docs/why.md` & `mkdocs-macros-plugin-1.0.4/webdoc/docs/why.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.2/webdoc/mkdocs.yml` & `mkdocs-macros-plugin-1.0.4/webdoc/mkdocs.yml`

 * *Files identical despite different names*

