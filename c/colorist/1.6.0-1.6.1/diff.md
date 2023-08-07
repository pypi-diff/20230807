# Comparing `tmp/colorist-1.6.0.tar.gz` & `tmp/colorist-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorist-1.6.0.tar", last modified: Mon Jun 19 14:50:19 2023, max compression
+gzip compressed data, was "colorist-1.6.1.tar", last modified: Mon Aug  7 00:08:52 2023, max compression
```

## Comparing `colorist-1.6.0.tar` & `colorist-1.6.1.tar`

### file list

```diff
@@ -1,76 +1,73 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.275304 colorist-1.6.0/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1827 2023-06-19 14:42:06.000000 colorist-1.6.0/INSTALLATION.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.6.0/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 10:14:25.000000 colorist-1.6.0/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24217 2023-06-19 14:50:19.275415 colorist-1.6.0/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    20077 2023-06-19 14:42:06.000000 colorist-1.6.0/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:58:40.000000 colorist-1.6.0/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1429 2023-06-19 14:50:19.275739 colorist-1.6.0/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.262969 colorist-1.6.0/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.264702 colorist-1.6.0/src/colorist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2724 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.266555 colorist-1.6.0/src/colorist/constants/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.6.0/src/colorist/constants/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2181 2023-04-11 11:49:16.000000 colorist-1.6.0/src/colorist/constants/ansi.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.6.0/src/colorist/constants/ascii.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.268506 colorist-1.6.0/src/colorist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.6.0/src/colorist/helper/.coverage
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.269227 colorist-1.6.0/src/colorist/helper/.pytest_cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/.gitignore
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/README.md
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.263243 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.269622 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.6.0/src/colorist/helper/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-23 10:26:22.000000 colorist-1.6.0/src/colorist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1973 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/helper/convert.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      733 2023-04-22 10:25:27.000000 colorist-1.6.0/src/colorist/helper/error.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.6.0/src/colorist/helper/generate.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1181 2023-04-25 04:39:14.000000 colorist-1.6.0/src/colorist/helper/print.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      493 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/helper/validate.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.270026 colorist-1.6.0/src/colorist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1789 2023-04-22 08:37:25.000000 colorist-1.6.0/src/colorist/model/README.MD
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.271053 colorist-1.6.0/src/colorist/model/abc/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/effect.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1329 2023-04-22 10:25:27.000000 colorist-1.6.0/src/colorist/model/abc/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/abc/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.272151 colorist-1.6.0/src/colorist/model/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      504 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/background/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      541 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      466 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.272993 colorist-1.6.0/src/colorist/model/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/model/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      507 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/foreground/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      544 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      469 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/model/foreground/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.273322 colorist-1.6.0/src/colorist/print/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.274194 colorist-1.6.0/src/colorist/print/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2509 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1320 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      461 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/background/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      561 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      465 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1395 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.275134 colorist-1.6.0/src/colorist/print/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2331 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1142 2023-04-11 07:01:26.000000 colorist-1.6.0/src/colorist/print/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      415 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/foreground/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      531 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      435 2023-04-23 22:57:28.000000 colorist-1.6.0/src/colorist/print/foreground/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1318 2023-04-23 11:04:46.000000 colorist-1.6.0/src/colorist/print/general.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.6.0/src/colorist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2023-06-19 14:42:06.000000 colorist-1.6.0/src/colorist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-06-19 14:50:19.265798 colorist-1.6.0/src/colorist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24217 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1964 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.6.0/src/colorist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       96 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2023-06-19 14:50:19.000000 colorist-1.6.0/src/colorist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.242177 colorist-1.6.1/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1503 2023-04-22 06:53:41.000000 colorist-1.6.1/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      193 2023-08-07 00:00:30.000000 colorist-1.6.1/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    15032 2023-08-07 00:08:52.242428 colorist-1.6.1/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    12330 2023-08-07 00:07:08.000000 colorist-1.6.1/README.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      109 2022-12-28 14:58:11.000000 colorist-1.6.1/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1759 2023-08-07 00:08:52.243854 colorist-1.6.1/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.181303 colorist-1.6.1/src/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.191565 colorist-1.6.1/src/colorist/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2724 2023-05-23 08:52:08.000000 colorist-1.6.1/src/colorist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.200847 colorist-1.6.1/src/colorist/constants/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      149 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/constants/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2181 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/constants/ansi.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      502 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/constants/ascii.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.209388 colorist-1.6.1/src/colorist/helper/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      215 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1973 2023-05-23 08:52:08.000000 colorist-1.6.1/src/colorist/helper/convert.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      733 2023-05-23 08:52:08.000000 colorist-1.6.1/src/colorist/helper/error.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1222 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/helper/generate.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1181 2023-08-06 16:14:43.000000 colorist-1.6.1/src/colorist/helper/print.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      493 2023-05-23 08:52:08.000000 colorist-1.6.1/src/colorist/helper/validate.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.211550 colorist-1.6.1/src/colorist/model/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1789 2023-04-22 08:35:56.000000 colorist-1.6.1/src/colorist/model/README.MD
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.215583 colorist-1.6.1/src/colorist/model/abc/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      572 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/abc/color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      426 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/abc/effect.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1329 2023-05-23 08:52:08.000000 colorist-1.6.1/src/colorist/model/abc/hex.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1915 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/abc/hsl.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      424 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/abc/mkdocstrings.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1326 2023-08-06 10:17:55.000000 colorist-1.6.1/src/colorist/model/abc/rgb.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.221881 colorist-1.6.1/src/colorist/model/background/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/background/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1410 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1306 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/background/color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1275 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/background/hex.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1428 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1354 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1516 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/effect.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.229134 colorist-1.6.1/src/colorist/model/foreground/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/foreground/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1402 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1298 2023-04-22 06:53:41.000000 colorist-1.6.1/src/colorist/model/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1278 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1431 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1357 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/model/foreground/rgb.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.230847 colorist-1.6.1/src/colorist/print/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.236037 colorist-1.6.1/src/colorist/print/background/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/background/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3270 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2985 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/background/color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1397 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/background/hex.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1638 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1481 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     3899 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/effect.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.241651 colorist-1.6.1/src/colorist/print/foreground/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/foreground/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2868 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     2583 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1307 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1591 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1423 2023-08-07 00:00:30.000000 colorist-1.6.1/src/colorist/print/foreground/rgb.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1318 2023-05-23 08:52:08.000000 colorist-1.6.1/src/colorist/print/general.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2022-04-27 16:25:22.000000 colorist-1.6.1/src/colorist/py.typed
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      174 2023-08-07 00:07:18.000000 colorist-1.6.1/src/colorist/version.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-07 00:08:52.198020 colorist-1.6.1/src/colorist.egg-info/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)    15032 2023-08-07 00:08:51.000000 colorist-1.6.1/src/colorist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1950 2023-08-07 00:08:52.000000 colorist-1.6.1/src/colorist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2023-08-07 00:08:51.000000 colorist-1.6.1/src/colorist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2023-08-07 00:08:48.000000 colorist-1.6.1/src/colorist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       96 2023-08-07 00:08:51.000000 colorist-1.6.1/src/colorist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        9 2023-08-07 00:08:52.000000 colorist-1.6.1/src/colorist.egg-info/top_level.txt
```

### Comparing `colorist-1.6.0/LICENSE.md` & `colorist-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/README.md` & `colorist-1.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,47 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.0&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+Metadata-Version: 2.1
+Name: colorist
+Version: 1.6.1
+Summary: Colorist for Python
+Home-page: https://jakob-bagterp.github.io/colorist-for-python/
+Download-URL: https://pypi.org/project/colorist/
+Author: Jakob Bagterp
+Author-email: jakob_bagterp@hotmail.com
+Maintainer: Jakob Bagterp
+Maintainer-email: jakob_bagterp@hotmail.com
+License: 3-Clause BSD License
+Project-URL: Bug Tracker, https://github.com/jakob-bagterp/colorist-for-python/issues
+Project-URL: Documentation, https://jakob-bagterp.github.io/colorist-for-python/
+Project-URL: API Reference, https://jakob-bagterp.github.io/colorist-for-python/reference/
+Project-URL: Source Code, https://github.com/jakob-bagterp/colorist-for-python
+Project-URL: Release Notes, https://github.com/jakob-bagterp/colorist-for-python/releases
+Keywords: python,colors,terminal
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE.md
+
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.6.1&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
+[![CodeQL](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
 
 # 🌈 Colorist for Python 🌈
 Lightweight Python package that makes it easy and fast to print colored text in the terminal.
 
-Ready to try? [Learn how to install](https://github.com/jakob-bagterp/colorist-for-python/blob/master/INSTALLATION.md).
+Ready to try? See [how to install](https://jakob-bagterp.github.io/colorist-for-python/getting-started/installation/).
 
 ## Getting Started
 ### Print Line of Colored Text
 How to print a full line of colored text in the terminal:
 
 ```python
 from colorist import green, yellow, red
@@ -20,314 +49,152 @@
 green("This is GREEN!")
 yellow("This is YELLOW!")
 red("This is RED!")
 ```
 
 How it appears in the terminal:
 
-![Example of full line of green, yellow, red colored text printed in a terminal window](/assets/images/examples/color_full_text_green_yellow_red.png)
+![Example of full line of green, yellow, red colored text printed in a terminal window](/docs/assets/images/examples/color_full_text_green_yellow_red.png)
 
 ### Print Mixed Text Colors
 How to customize colors inside a paragraph and print it in the terminal:
 
 ```python
 from colorist import Color
 
 print(f"I want {Color.RED}red{Color.OFF} color inside this paragraph")
 
 print(f"Both {Color.GREEN}green{Color.OFF} and {Color.YELLOW}yellow{Color.OFF} are nice colors")
 ```
 
 How it appears in the terminal:
 
-![Example of white text mixed with green, yellow, red colors printed in a terminal window](/assets/images/examples/color_custom_text_green_yellow_red.png)
+![Example of white text mixed with green, yellow, red colors printed in a terminal window](/docs/assets/images/examples/color_custom_text_green_yellow_red.png)
 
 ## Other Styling Options
 ### Print Bright Colors
 Most terminals support bright colors that stand more out:
 
 ```python
 from colorist import BrightColor
 
 print(f"I want {BrightColor.CYAN}cyan{BrightColor.OFF} color inside this paragraph")
 ```
 
 How it appears in the terminal:
 
-![Example of white text mixed with cyan printed in a terminal window](/assets/images/examples/bright_color_custom_text_cyan.png)
+![Example of white text mixed with cyan printed in a terminal window](/docs/assets/images/examples/bright_color_custom_text_cyan.png)
 
-Remember to use `Color.OFF` or `BrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
+Remember to use `Color.OFF` or `BrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise, the color may spill over and into other terminal messages.
 
 ### Print Background Colors
 ```python
 from colorist import bg_green, bg_yellow, bg_red
 
 bg_green("This is GREEN background!")
 bg_yellow("This is YELLOW background!")
 bg_red("This is RED background!")
 ```
 
 How it appears in the terminal:
 
-![Example of white text and colored backgrounds if green, yellow, red printed in a terminal window](/assets/images/examples/bg_color_full_text_green_yellow_red.png)
+![Example of white text and colored backgrounds if green, yellow, red printed in a terminal window](/docs/assets/images/examples/bg_color_full_text_green_yellow_red.png)
 
 Background colors can also be mixed inside a paragraph:
 
 ```python
 from colorist import BgColor
 
 print(f"I want {BgColor.RED}red{BgColor.OFF} background color inside this paragraph")
 
 print(f"Both {BgColor.GREEN}green{BgColor.OFF} and {BgColor.YELLOW}yellow{BgColor.OFF} are nice background colors")
 ```
 
 How it appears in the terminal:
 
-![Example of black, green, yellow, red background colors mixed inside paragraph printed in a terminal window](/assets/images/examples/bg_color_custom_text_green_yellow_red.png)
-
+![Example of black, green, yellow, red background colors mixed inside paragraph printed in a terminal window](/docs/assets/images/examples/bg_color_custom_text_green_yellow_red.png)
 
 ```python
 from colorist import BgBrightColor
 
 print(f"I want {BgBrightColor.CYAN}cyan{BgBrightColor.OFF} background color inside this paragraph")
 ```
 
 How it appears in the terminal:
 
-![Example of white text on a cyan background color printed in a terminal window](/assets/images/examples/bg_bright_color_custom_text_cyan.png)
-
-As with text colors, remember to use `BgColor.OFF` or `BgBrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise the color may spill over and into other terminal messages.
-
-### Other String Formats
-It's often easier and more readable to use [f-strings](https://peps.python.org/pep-0498/) as in the examples above, but f-strings aren't supported in some earlier versions of Python. Instead, you can also use string formatting or concatenation:
-
-```python
-from colorist import Color
-
-print("I want {0}red{1} color inside this paragraph".format(Color.RED, Color.OFF))
-print("I want " + Color.RED + "red" + Color.OFF + " color inside this paragraph")
-```
-
-Both options appear the same in the terminal:
-
-![Example of terminal message with red text color](/assets/images/examples/color_custom_text_red.png)
-
-### Print RGB, HSL and Hex Colors
-Note that not all terminals support RGB, HSL or Hex colors. If your terminal does support such advanced colors, read on.
-
-#### RGB Colors
-Try the `rgb` and `bg_rgb` methods for a full line of colored text. The values for red, green, blue can be an integer between `0-255`.
-
-```python
-from colorist import rgb, bg_rgb
-
-rgb("I want this text in blue RGB colors", 0, 128, 255)
-bg_rgb("I want this background in blue RGB colors", 0, 128, 255)
-```
-
-How it appears in the terminal:
-
-![Example of text in RGB colors printed in a terminal window](/assets/images/examples/rgb_full_text.png)
-
-Or customize the styling of text and background with the `ColorRGB` and `BgColorRGB` classes:
-
-```python
-from colorist import ColorRGB, BgColorRGB
-
-dusty_pink = ColorRGB(194, 145, 164)
-bg_steel_blue = BgColorRGB(70, 130, 180)
-
-print(f"I want to use {dusty_pink}dusty pink{dusty_pink.OFF} and {bg_steel_blue}steel blue{bg_steel_blue.OFF} colors inside this paragraph")
-```
-
-How it appears in the terminal:
-
-![Another example of text in RGB colors printed in a terminal window](/assets/images/examples/rgb_custom_text.png)
-
-#### HSL Colors
-Similarly, you can also output colors in HSL with the `hsl` and `bg_hsl` methods. The value for hue can be between `0-360` degrees, while saturation and lightness can be a percentage between `0-100` %:
-
-```python
-from colorist import hsl, bg_hsl
-
-hsl("I want this text in green HSL colors", 120, 50, 50)
-bg_hsl("I want this background in green HSL colors", 120, 50, 50)
-```
-
-How it appears in the terminal:
-
-![Example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_full_text.png)
-
-Or customize the styling of text and background with the `ColorHSL` and `BgColorHSL` classes:
-
-```python
-from colorist import ColorHSL, BgColorHSL
-
-mustard_green = ColorHSL(60, 56, 43)
-bg_steel_gray = BgColorHSL(190, 2, 49)
-
-print(f"I want to use {mustard_green}mustard green{mustard_green.OFF} and {bg_steel_gray}steel blue{bg_steel_gray.OFF} colors inside this paragraph")
-```
-
-How it appears in the terminal:
-
-![Another example of text in HSL colors printed in a terminal window](/assets/images/examples/hsl_custom_text.png)
-
-#### Hex Colors
-Try the `hex` and `bg_hex` methods for a full line of colored text. Allowed Hex values are, for instance, `#00aaff` or `#0af`, alternatively without the hash sign as `00aaff` or `0af`.
-
-```python
-from colorist import hex, bg_hex
-
-hex("I want this text in coral Hex colors", "#ff7f50")
-bg_hex("I want this background in coral Hex colors", "#ff7f50")
-```
-
-How it appears in the terminal:
-
-![Example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_full_text.png)
+![Example of white text on a cyan background color printed in a terminal window](/docs/assets/images/examples/bg_bright_color_custom_text_cyan.png)
 
-Or customize the styling of text and background with the `ColorHex` and `BgColorHex` classes:
-
-```python
-from colorist import ColorHex, BgColorHex
-
-watermelon_red = ColorHex("#ff5733")
-bg_mint_green = BgColorHex("#99ff99")
-
-print(f"I want to use {watermelon_red}watermelon pink{watermelon_red.OFF} and {bg_mint_green}mint green{bg_mint_green.OFF} colors inside this paragraph")
-```
-
-How it appears in the terminal:
-
-![Another example of text in Hex colors printed in a terminal window](/assets/images/examples/hex_custom_text.png)
-
-### Print Effects and Other Styles
-In addition to colors, Colorist can also add effects when you print text in the terminal. How to print a full line of text with effects:
-
-```python
-from colorist import effect_blink
-
-effect_blink("This is BLINKING!")
-```
-
-How it appears in the terminal:
-
-![Example of terminal message with blinking text](/assets/images/examples/effect_full_text_blink_default.gif)
-
-And this can also be combined with an optional color:
-
-```python
-from colorist import Color, effect_blink
-
-effect_blink("This is BLINKING!", Color.CYAN)
-```
-
-How it appears in the terminal:
-
-![Example of terminal message with blinking, cyan-colored text](/assets/images/examples/effect_full_text_blink_cyan.gif)
-
-How to customize terminal messages and change effect inside a paragraph:
-
-```python
-from colorist import Effect
-
-print(f"I want {Effect.UNDERLINE}underlined text{Effect.UNDERLINE_OFF} inside this paragraph")
-
-print(f"I want {Effect.BOLD}emphasized text{Effect.BOLD_OFF} inside this paragraph")
-```
-
-How it appears in the terminal:
-
-![Example of terminal message with underline and bold text](/assets/images/examples/effect_custom_text_underline_bold.png)
-
-Effects can also be mixed with colors:
-
-```python
-from colorist import Color, Effect
-
-print(f"I want both {Color.RED}colored and {Effect.BLINK}blinking{Effect.BLINK_OFF} text{Color.OFF} inside this paragraph")
-```
-
-How it appears in the terminal:
-
-![Example of terminal message with red and blinking text](/assets/images/examples/effect_custom_text_blink_red.gif)
-
-Similar to `Color.OFF`, remember to turn off an effect with the relevant reset option (e.g `Effect.BOLD_OFF`, `Effect.DIM_OFF`, etc. or even just `Effect.OFF`) every time you want to revert back to the default terminal text style. Otherwise the effect may spill over and into other terminal messages.
-
-# Supported Colors and Styles
-Colorist is based on [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code), a standard that defines colors, styling and effects for text in terminal windows. Note that most terminals support all color options, but not all:
-
-| Category                                               | Color Options                                                                |
-| ------------------------------------------------------ | ---------------------------------------------------------------------------- |
-| Standard ANSI colors supported by almost all terminals | `Color`, `BgColor`, `Effect`                                                 |
-| Non-standard ANSI colors supported by most terminals   | `BrightColor`, `BgBrightColor`                                               |
-| Advanced ANSI colors only supported by some terminals  | `ColorRGB`, `BgColorRGB`, `ColorHSL`, `BgColorHSL`, `ColorHex`, `BgColorHex` |
+As with text colors, remember to use `BgColor.OFF` or `BgBrightColor.OFF` every time you want to revert back to the default terminal text style. Otherwise, the color may spill over and into other terminal messages.
 
 ## Foreground Text
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
-| ![Green](/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/assets/images/examples/color_map/green_full_text_167x16.png) |
-| ![Yellow](/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/assets/images/examples/color_map/yellow_full_text_167x16.png) |
-| ![Red](/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/assets/images/examples/color_map/red_full_text_167x16.png) |
-| ![Magenta](/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/assets/images/examples/color_map/magenta_full_text_167x16.png) |
-| ![Blue](/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/assets/images/examples/color_map/blue_full_text_167x16.png) |
-| ![Cyan](/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/assets/images/examples/color_map/cyan_full_text_167x16.png) |
-| ![White](/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/assets/images/examples/color_map/white_full_text_167x16.png) |
-| ![Black](/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/assets/images/examples/color_map/black_full_text_167x16.png) |
+| ![Green](/docs/assets/images/colors/green_16x16.png) | `green("text")` | `Color.GREEN` | ![Green text color in terminal](/docs/assets/images/examples/color_map/green_full_text_167x16.png) |
+| ![Yellow](/docs/assets/images/colors/yellow_16x16.png) | `yellow("text")` | `Color.YELLOW` | ![Yellow text color in terminal](/docs/assets/images/examples/color_map/yellow_full_text_167x16.png) |
+| ![Red](/docs/assets/images/colors/red_16x16.png) | `red("text")` | `Color.RED` | ![Red text color in terminal](/docs/assets/images/examples/color_map/red_full_text_167x16.png) |
+| ![Magenta](/docs/assets/images/colors/magenta_16x16.png) | `magenta("text")` | `Color.MAGENTA` | ![Magenta text color in terminal](/docs/assets/images/examples/color_map/magenta_full_text_167x16.png) |
+| ![Blue](/docs/assets/images/colors/blue_16x16.png) | `blue("text")` | `Color.BLUE` | ![Blue text color in terminal](/docs/assets/images/examples/color_map/blue_full_text_167x16.png) |
+| ![Cyan](/docs/assets/images/colors/cyan_16x16.png) | `cyan("text")` | `Color.CYAN` | ![Cyan text color in terminal](/docs/assets/images/examples/color_map/cyan_full_text_167x16.png) |
+| ![White](/docs/assets/images/colors/white_16x16.png) | `white("text")` | `Color.WHITE` | ![White text color in terminal](/docs/assets/images/examples/color_map/white_full_text_167x16.png) |
+| ![Black](/docs/assets/images/colors/black_16x16.png) | `black("text")` | `Color.BLACK` | ![Black text color in terminal](/docs/assets/images/examples/color_map/black_full_text_167x16.png) |
 | - | - | `Color.DEFAULT` | - |
 | - | - | `Color.OFF` | - |
-| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
-| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
-| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
-| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
-| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
-| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
-| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
-| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
+| ![Bright green](/docs/assets/images/colors/bright_green_16x16.png) | `bright_green("text")` | `BrightColor.GREEN` | ![Bright green text color in terminal](/docs/assets/images/examples/color_map/bright_green_full_text_167x16.png) |
+| ![Bright yellow](/docs/assets/images/colors/bright_yellow_16x16.png) | `bright_yellow("text")` | `BrightColor.YELLOW` | ![Bright yellow text color in terminal](/docs/assets/images/examples/color_map/bright_yellow_full_text_167x16.png) |
+| ![Bright red](/docs/assets/images/colors/bright_red_16x16.png) | `bright_red("text")` | `BrightColor.RED` | ![Bright red text color in terminal](/docs/assets/images/examples/color_map/bright_red_full_text_167x16.png) |
+| ![Bright magenta](/docs/assets/images/colors/bright_magenta_16x16.png) | `bright_magenta("text")` | `BrightColor.MAGENTA` | ![Bright magenta text color in terminal](/docs/assets/images/examples/color_map/bright_magenta_full_text_167x16.png) |
+| ![Bright blue](/docs/assets/images/colors/bright_blue_16x16.png) | `bright_blue("text")` | `BrightColor.BLUE` | ![Bright blue text color in terminal](/docs/assets/images/examples/color_map/bright_blue_full_text_167x16.png) |
+| ![Bright cyan](/docs/assets/images/colors/bright_cyan_16x16.png) | `bright_cyan("text")` | `BrightColor.CYAN` | ![Bright cyan text color in terminal](/docs/assets/images/examples/color_map/bright_cyan_full_text_167x16.png) |
+| ![Bright white](/docs/assets/images/colors/bright_white_16x16.png) | `bright_white("text")` | `BrightColor.WHITE` | ![Bright white text color in terminal](/docs/assets/images/examples/color_map/bright_white_full_text_167x16.png) |
+| ![Bright black](/docs/assets/images/colors/bright_black_16x16.png) | `bright_black("text")` | `BrightColor.BLACK` | ![Bright black text color in terminal](/docs/assets/images/examples/color_map/bright_black_full_text_167x16.png) |
 | - | - | `BrightColor.DEFAULT` | - |
 | - | - | `BrightColor.OFF` | - |
 
 ## Background
 | Color | Full Text Function | Custom | Example |
 | ----- | ------------------ | ------ | ------- |
-| ![Green](/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
-| ![Yellow](/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
-| ![Red](/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
-| ![Magenta](/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
-| ![Blue](/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
-| ![Cyan](/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
-| ![White](/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
-| ![Black](/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
+| ![Green](/docs/assets/images/colors/green_16x16.png) | `bg_green("text")` | `BgColor.GREEN` | ![Green background color in terminal](/docs/assets/images/examples/bg_color_map/green_full_text_194x16.png) |
+| ![Yellow](/docs/assets/images/colors/yellow_16x16.png) | `bg_yellow("text")` | `BgColor.YELLOW` | ![Yellow background color in terminal](/docs/assets/images/examples/bg_color_map/yellow_full_text_194x16.png) |
+| ![Red](/docs/assets/images/colors/red_16x16.png) | `bg_red("text")` | `BgColor.RED` | ![Red background color in terminal](/docs/assets/images/examples/bg_color_map/red_full_text_194x16.png) |
+| ![Magenta](/docs/assets/images/colors/magenta_16x16.png) | `bg_magenta("text")` | `BgColor.MAGENTA` | ![Magenta background color in terminal](/docs/assets/images/examples/bg_color_map/magenta_full_text_194x16.png) |
+| ![Blue](/docs/assets/images/colors/blue_16x16.png) | `bg_blue("text")` | `BgColor.BLUE` | ![Blue background color in terminal](/docs/assets/images/examples/bg_color_map/blue_full_text_194x16.png) |
+| ![Cyan](/docs/assets/images/colors/cyan_16x16.png) | `bg_cyan("text")` | `BgColor.CYAN` | ![Cyan background color in terminal](/docs/assets/images/examples/bg_color_map/cyan_full_text_194x16.png) |
+| ![White](/docs/assets/images/colors/white_16x16.png) | `bg_white("text")` | `BgColor.WHITE` | ![White background color in terminal](/docs/assets/images/examples/bg_color_map/white_full_text_194x16.png) |
+| ![Black](/docs/assets/images/colors/black_16x16.png) | `bg_black("text")` | `BgColor.BLACK` | ![Black background color in terminal](/docs/assets/images/examples/bg_color_map/black_full_text_194x16.png) |
 | - | - | `BgColor.DEFAULT` | - |
 | - | - | `BgColor.OFF` | - |
-| ![Bright green](/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
-| ![Bright yellow](/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
-| ![Bright red](/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
-| ![Bright magenta](/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
-| ![Bright blue](/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
-| ![Bright cyan](/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
-| ![Bright white](/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
-| ![Bright black](/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
-| - | - |`BgBrightColor.DEFAULT` | - |
+| ![Bright green](/docs/assets/images/colors/bright_green_16x16.png) | `bg_bright_green("text")` | `BgBrightColor.GREEN` | ![Bright green background color in terminal](/docs/assets/images/examples/bg_color_map/bright_green_full_text_194x16.png) |
+| ![Bright yellow](/docs/assets/images/colors/bright_yellow_16x16.png) | `bg_bright_yellow("text")` | `BgBrightColor.YELLOW` | ![Bright yellow background color in terminal](/docs/assets/images/examples/bg_color_map/bright_yellow_full_text_194x16.png) |
+| ![Bright red](/docs/assets/images/colors/bright_red_16x16.png) | `bg_bright_red("text")` | `BgBrightColor.RED` | ![Bright red background color in terminal](/docs/assets/images/examples/bg_color_map/bright_red_full_text_194x16.png) |
+| ![Bright magenta](/docs/assets/images/colors/bright_magenta_16x16.png) | `bg_bright_magenta("text")` | `BgBrightColor.MAGENTA` | ![Bright magenta background color in terminal](/docs/assets/images/examples/bg_color_map/bright_magenta_full_text_194x16.png) |
+| ![Bright blue](/docs/assets/images/colors/bright_blue_16x16.png) | `bg_bright_blue("text")` | `BgBrightColor.BLUE` | ![Bright blue background color in terminal](/docs/assets/images/examples/bg_color_map/bright_blue_full_text_194x16.png) |
+| ![Bright cyan](/docs/assets/images/colors/bright_cyan_16x16.png) | `bg_bright_cyan("text")` | `BgBrightColor.CYAN` | ![Bright cyan background color in terminal](/docs/assets/images/examples/bg_color_map/bright_cyan_full_text_194x16.png) |
+| ![Bright white](/docs/assets/images/colors/bright_white_16x16.png) | `bg_bright_white("text")` | `BgBrightColor.WHITE` | ![Bright white background color in terminal](/docs/assets/images/examples/bg_color_map/bright_white_full_text_194x16.png) |
+| ![Bright black](/docs/assets/images/colors/bright_black_16x16.png) | `bg_bright_black("text")` | `BgBrightColor.BLACK` | ![Bright black background color in terminal](/docs/assets/images/examples/bg_color_map/bright_black_full_text_194x16.png) |
+| - | - | `BgBrightColor.DEFAULT` | - |
 | - | - | `BgBrightColor.OFF` | - |
 
-## Effects
-| Effect           | Full Text Function         | Custom             | Reset                  | Example    |
-| ---------------- | -------------------------- | ------------------ | ---------------------- | ---------- |
-| **Bold**         | `effect_bold("text")`      | `Effect.BOLD`      | `Effect.BOLD_OFF`      | ![Example of terminal message with bold text](/assets/images/examples/effect_map/bold_full_text_140x16.png) |
-| Dim              | `effect_dim("text")`       | `Effect.DIM`       | `Effect.DIM_OFF`       | ![Example of terminal message with dimmed text](/assets/images/examples/effect_map/dim_full_text_140x16.png) |
-| <u>Underline</u> | `effect_underline("text")` | `Effect.UNDERLINE` | `Effect.UNDERLINE_OFF` | ![Example of terminal message with underlined text](/assets/images/examples/effect_map/underline_full_text_140x16.png) |
-| Blink            | `effect_blink("text")`     | `Effect.BLINK`     | `Effect.BLINK_OFF`     | ![Example of terminal message with blinking text](/assets/images/examples/effect_map/blink_full_text_140x16.gif) |
-| Reverse          | `effect_reverse("text")`   | `Effect.REVERSE`   | `Effect.REVERSE_OFF`   | ![Example of terminal message with reversed text color and background](/assets/images/examples/effect_map/reverse_full_text_140x16.png) |
-| Hide             | `effect_hide("text")`      | `Effect.HIDE`      | `Effect.HIDE_OFF`      | ![Example of terminal message with hidden text](/assets/images/examples/effect_map/hide_full_text_140x16.png) |
-| -                | -                          | -                  | `Effect.OFF`           | -          |
-
 # Thank You for Supporting
 ## Donate
 This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/colorist-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/colorist-for-python/issues).
+
+# 3-Clause BSD License
+
+Copyright (c) 2022 – present, Jakob Bagterp
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
```

### Comparing `colorist-1.6.0/setup.cfg` & `colorist-1.6.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 name = colorist
 version = attr: colorist.__version__
 author = Jakob Bagterp
 author_email = jakob_bagterp@hotmail.com
 maintainer = Jakob Bagterp
 maintainer_email = jakob_bagterp@hotmail.com
 description = Colorist for Python
-long_description = file: README.md, INSTALLATION.md, LICENSE.md
+long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 keywords = 
 	python
 	colors
 	terminal
-url = https://github.com/jakob-bagterp/colorist-for-python
+url = https://jakob-bagterp.github.io/colorist-for-python/
+download_url = https://pypi.org/project/colorist/
 project_urls = 
 	Bug Tracker = https://github.com/jakob-bagterp/colorist-for-python/issues
+	Documentation = https://jakob-bagterp.github.io/colorist-for-python/
+	API Reference = https://jakob-bagterp.github.io/colorist-for-python/reference/
+	Source Code = https://github.com/jakob-bagterp/colorist-for-python
+	Release Notes = https://github.com/jakob-bagterp/colorist-for-python/releases
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 license = 3-Clause BSD License
@@ -31,19 +36,19 @@
 python_requires = >=3.10
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
 	coverage==7.2.7
-	flake8==6.0.0
-	mypy==1.3.0
-	pytest==7.3.2
+	flake8==6.1.0
+	mypy==1.4.1
+	pytest==7.4.0
 	pytest-cov==4.1.0
-	tox==4.6.0
+	tox==4.6.4
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `colorist-1.6.0/src/colorist/__init__.py` & `colorist-1.6.1/src/colorist/__init__.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/constants/ansi.py` & `colorist-1.6.1/src/colorist/constants/ansi.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/helper/convert.py` & `colorist-1.6.1/src/colorist/helper/convert.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/helper/error.py` & `colorist-1.6.1/src/colorist/helper/error.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/helper/generate.py` & `colorist-1.6.1/src/colorist/helper/generate.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/helper/print.py` & `colorist-1.6.1/src/colorist/helper/print.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/README.MD` & `colorist-1.6.1/src/colorist/model/README.MD`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/abc/color.py` & `colorist-1.6.1/src/colorist/model/abc/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/abc/hex.py` & `colorist-1.6.1/src/colorist/model/abc/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/abc/hsl.py` & `colorist-1.6.1/src/colorist/model/abc/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/abc/rgb.py` & `colorist-1.6.1/src/colorist/model/abc/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/background/bright_color.py` & `colorist-1.6.1/src/colorist/model/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/background/color.py` & `colorist-1.6.1/src/colorist/model/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/effect.py` & `colorist-1.6.1/src/colorist/model/effect.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/foreground/bright_color.py` & `colorist-1.6.1/src/colorist/model/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/model/foreground/color.py` & `colorist-1.6.1/src/colorist/model/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist/print/general.py` & `colorist-1.6.1/src/colorist/print/general.py`

 * *Files identical despite different names*

### Comparing `colorist-1.6.0/src/colorist.egg-info/SOURCES.txt` & `colorist-1.6.1/src/colorist.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-INSTALLATION.md
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/colorist/__init__.py
 src/colorist/py.typed
@@ -12,48 +11,49 @@
 src/colorist.egg-info/dependency_links.txt
 src/colorist.egg-info/not-zip-safe
 src/colorist.egg-info/requires.txt
 src/colorist.egg-info/top_level.txt
 src/colorist/constants/__init__.py
 src/colorist/constants/ansi.py
 src/colorist/constants/ascii.py
-src/colorist/helper/.coverage
 src/colorist/helper/__init__.py
 src/colorist/helper/convert.py
 src/colorist/helper/error.py
 src/colorist/helper/generate.py
 src/colorist/helper/print.py
 src/colorist/helper/validate.py
-src/colorist/helper/.pytest_cache/.gitignore
-src/colorist/helper/.pytest_cache/CACHEDIR.TAG
-src/colorist/helper/.pytest_cache/README.md
-src/colorist/helper/.pytest_cache/v/cache/nodeids
-src/colorist/helper/.pytest_cache/v/cache/stepwise
 src/colorist/model/README.MD
+src/colorist/model/__init__.py
 src/colorist/model/effect.py
 src/colorist/model/abc/color.py
 src/colorist/model/abc/effect.py
 src/colorist/model/abc/hex.py
 src/colorist/model/abc/hsl.py
+src/colorist/model/abc/mkdocstrings.py
 src/colorist/model/abc/rgb.py
+src/colorist/model/background/__init__.py
 src/colorist/model/background/bright_color.py
 src/colorist/model/background/color.py
 src/colorist/model/background/hex.py
 src/colorist/model/background/hsl.py
 src/colorist/model/background/rgb.py
+src/colorist/model/foreground/__init__.py
 src/colorist/model/foreground/bright_color.py
 src/colorist/model/foreground/color.py
 src/colorist/model/foreground/hex.py
 src/colorist/model/foreground/hsl.py
 src/colorist/model/foreground/rgb.py
+src/colorist/print/__init__.py
 src/colorist/print/effect.py
 src/colorist/print/general.py
+src/colorist/print/background/__init__.py
 src/colorist/print/background/bright_color.py
 src/colorist/print/background/color.py
 src/colorist/print/background/hex.py
 src/colorist/print/background/hsl.py
 src/colorist/print/background/rgb.py
+src/colorist/print/foreground/__init__.py
 src/colorist/print/foreground/bright_color.py
 src/colorist/print/foreground/color.py
 src/colorist/print/foreground/hex.py
 src/colorist/print/foreground/hsl.py
 src/colorist/print/foreground/rgb.py
```

