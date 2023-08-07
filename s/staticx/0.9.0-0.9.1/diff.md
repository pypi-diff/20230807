# Comparing `tmp/staticx-0.9.0.tar.gz` & `tmp/staticx-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/staticx-0.9.0.tar", last modified: Sat Jan 11 05:55:49 2020, max compression
+gzip compressed data, was "dist/staticx-0.9.1.tar", last modified: Thu Jan 30 02:54:15 2020, max compression
```

## Comparing `staticx-0.9.0.tar` & `staticx-0.9.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-01-11 05:52:33.000000 staticx-0.9.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/bootloader/
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/common.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      385 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/debug.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/mmap.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    11181 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/main.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      802 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/util.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/error.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/elfutil.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      566 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/SConscript
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/extract.h
--rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/util.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/mmap.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      510 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/error.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      543 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/elfutil.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5919 2020-01-11 05:52:33.000000 staticx-0.9.0/bootloader/extract.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2020-01-11 05:55:49.000000 staticx-0.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2544 2020-01-11 05:52:33.000000 staticx-0.9.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1286 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-11 05:53:02.000000 staticx-0.9.0/staticx.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-01-11 05:55:49.000000 staticx-0.9.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/libxz/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_stream.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_private.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      396 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    13905 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_dec_bcj.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    29111 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_dec_lzma2.c
--rw-rw-r--   0 travis    (2000) travis    (2000)    12341 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6112 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_lzma2.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      460 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/SConscript
--rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_crc32.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     2996 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_config.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20688 2020-01-11 05:52:33.000000 staticx-0.9.0/libxz/xz_dec_stream.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2020-01-11 05:52:33.000000 staticx-0.9.0/SConstruct
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/libtar/
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)     2027 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/util.c
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/libtar/compat/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3574 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/compat/strmode.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/compat/compat.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/compat/strlcpy.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      897 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/handle.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     4469 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/block.c
--rw-rw-r--   0 travis    (2000) travis    (2000)      485 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/SConscript
--rw-rw-r--   0 travis    (2000) travis    (2000)     1786 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/COPYRIGHT
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/output.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     1983 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/decode.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     6088 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/libtar.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9449 2020-01-11 05:52:33.000000 staticx-0.9.0/libtar/extract.c
--rw-rw-r--   0 travis    (2000) travis    (2000)     3191 2020-01-11 05:52:33.000000 staticx-0.9.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-11 05:55:49.000000 staticx-0.9.0/staticx/hooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3813 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/hooks/pyinstaller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/hooks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3972 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/archive.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7299 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/elf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      149 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2029 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      874 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2263 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/bcjfilter.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5095 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1442 2020-01-11 05:52:33.000000 staticx-0.9.0/staticx/errors.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-01-30 02:51:02.000000 staticx-0.9.1/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/bootloader/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/common.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      385 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/debug.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/mmap.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11219 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/main.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      802 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/util.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/error.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/elfutil.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      566 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/SConscript
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/extract.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)       91 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/util.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/mmap.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      510 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/error.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      543 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/elfutil.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5919 2020-01-30 02:51:02.000000 staticx-0.9.1/bootloader/extract.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2020-01-30 02:54:15.000000 staticx-0.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2544 2020-01-30 02:51:02.000000 staticx-0.9.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4487 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-30 02:51:30.000000 staticx-0.9.1/staticx.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1208 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       53 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       51 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2020-01-30 02:54:15.000000 staticx-0.9.1/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/libxz/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_stream.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_private.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      396 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13905 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_dec_bcj.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29111 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_dec_lzma2.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12341 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6112 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_lzma2.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      460 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/SConscript
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1261 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_crc32.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2996 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_config.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20688 2020-01-30 02:51:02.000000 staticx-0.9.1/libxz/xz_dec_stream.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2020-01-30 02:51:02.000000 staticx-0.9.1/SConstruct
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/libtar/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      122 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/VERSION
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2027 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/util.c
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/libtar/compat/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3574 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/compat/strmode.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/compat/compat.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/compat/strlcpy.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      897 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/handle.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4469 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/block.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)      485 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/SConscript
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1786 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/COPYRIGHT
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/output.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1983 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/decode.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6088 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/libtar.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9449 2020-01-30 02:51:02.000000 staticx-0.9.1/libtar/extract.c
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3465 2020-01-30 02:51:02.000000 staticx-0.9.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-30 02:54:15.000000 staticx-0.9.1/staticx/hooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3813 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/hooks/pyinstaller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/hooks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3972 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/archive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7420 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/elf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      149 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2029 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      881 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2263 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1099 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/bcjfilter.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5095 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1442 2020-01-30 02:51:02.000000 staticx-0.9.1/staticx/errors.py
```

### Comparing `staticx-0.9.0/bootloader/main.c` & `staticx-0.9.1/bootloader/main.c`

 * *Files 1% similar despite different names*

```diff
@@ -201,18 +201,19 @@
 
     free(interp_path);
 }
 
 static char *
 create_tmpdir(void)
 {
-    char *template = path_join(getenv(TMPDIR) ?: "/tmp", "staticx-XXXXXX");
+    const char *tmproot = getenv(TMPDIR) ?: "/tmp";
+    char *template = path_join(tmproot, "staticx-XXXXXX");
     char *tmpdir = mkdtemp(template);
     if (!tmpdir)
-        error(2, errno, "Failed to create temporary directory: %s", tmpdir);
+        error(2, errno, "Failed to create temporary directory in %s", tmproot);
     assert(tmpdir == template);
     return tmpdir;
 }
 
 static char **
 make_argv(int orig_argc, char **orig_argv, char *argv0)
 {
```

### Comparing `staticx-0.9.0/bootloader/util.c` & `staticx-0.9.1/bootloader/util.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/bootloader/elfutil.c` & `staticx-0.9.1/bootloader/elfutil.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/bootloader/SConscript` & `staticx-0.9.1/bootloader/SConscript`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/bootloader/mmap.c` & `staticx-0.9.1/bootloader/mmap.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/bootloader/elfutil.h` & `staticx-0.9.1/bootloader/elfutil.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/bootloader/extract.c` & `staticx-0.9.1/bootloader/extract.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/README.md` & `staticx-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/staticx.egg-info/SOURCES.txt` & `staticx-0.9.1/staticx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_stream.h` & `staticx-0.9.1/libxz/xz_stream.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_private.h` & `staticx-0.9.1/libxz/xz_private.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_dec_bcj.c` & `staticx-0.9.1/libxz/xz_dec_bcj.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_dec_lzma2.c` & `staticx-0.9.1/libxz/xz_dec_lzma2.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz.h` & `staticx-0.9.1/libxz/xz.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_lzma2.h` & `staticx-0.9.1/libxz/xz_lzma2.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_crc32.c` & `staticx-0.9.1/libxz/xz_crc32.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_config.h` & `staticx-0.9.1/libxz/xz_config.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libxz/xz_dec_stream.c` & `staticx-0.9.1/libxz/xz_dec_stream.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/SConstruct` & `staticx-0.9.1/SConstruct`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/util.c` & `staticx-0.9.1/libtar/util.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/compat/strmode.c` & `staticx-0.9.1/libtar/compat/strmode.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/compat/strlcpy.c` & `staticx-0.9.1/libtar/compat/strlcpy.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/handle.c` & `staticx-0.9.1/libtar/handle.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/block.c` & `staticx-0.9.1/libtar/block.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/COPYRIGHT` & `staticx-0.9.1/libtar/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/output.c` & `staticx-0.9.1/libtar/output.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/decode.c` & `staticx-0.9.1/libtar/decode.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/libtar.h` & `staticx-0.9.1/libtar/libtar.h`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/libtar/extract.c` & `staticx-0.9.1/libtar/extract.c`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/setup.py` & `staticx-0.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,19 +33,27 @@
     def run(self):
         self.run_command('build_bootloader')
         build.run(self)
 
 
 ################################################################################
 
+def read_project_file(path):
+    proj_dir = os.path.dirname(__file__)
+    path = os.path.join(proj_dir, path)
+    with open(path, 'r') as f:
+        return f.read()
+
 setup(
     name = 'staticx',
     version = get_dynamic_version(),
     description = 'Build static self-extracting app from dynamic executable',
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*',
+    long_description = read_project_file('README.md'),
+    long_description_content_type = 'text/markdown',
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
         'Natural Language :: English',
         'Operating System :: POSIX :: Linux',
```

### Comparing `staticx-0.9.0/staticx/hooks/pyinstaller.py` & `staticx-0.9.1/staticx/hooks/pyinstaller.py`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/staticx/archive.py` & `staticx-0.9.1/staticx/archive.py`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/staticx/elf.py` & `staticx-0.9.1/staticx/elf.py`

 * *Files 16% similar despite different names*

```diff
@@ -78,14 +78,57 @@
 tool_strip      = ExternTool('strip', 'binutils')
 
 class LddError(ToolError):
     def __init__(self, message):
         super(LddError, self).__init__('ldd', message)
 
 
+def _parse_ldd_output(output):
+    # Example:
+    #	linux-vdso.so.1 (0x00007ffe53551000)
+    #     or
+    #	linux-vdso.so.1 =>  (0x00007ffe53551000)
+    #	libc.so.6 => /usr/lib64/libc.so.6 (0x00007f42ac010000)
+    #	/lib64/ld-linux-x86-64.so.2 (0x0000557376e75000)
+    #     or
+    #   /lib64/ld-linux-x86-64.so.2 => /usr/lib64/ld-linux-x86-64.so.2 (0x00007f1de63ac000)
+    pat = re.compile(r'\t([\w./+-]*) (?:=> ([\w./+-]*) )?\((0x[0-9a-fA-F]*)\)')
+
+    for line in output.splitlines():
+        m = pat.match(line)
+        if not m:
+            # Some shared objs might have no DT_NEEDED tags (see issue #67)
+            if line == '\tstatically linked':
+                break
+            raise LddError("Unexpected line in ldd output: " + line)
+        libname  = m.group(1)
+        resolved = m.group(2)
+        baseaddr = int(m.group(3), 16)
+
+        if resolved:
+            # ldd outupt a resolved symlink, use that
+            libpath = resolved
+        elif libname.startswith('/'):
+            # The library directly referenced an absolute path, use that
+            libpath = libname
+        else:
+            # Assume an unresolved non-absolute library name is synthetic
+            # like linux-vdso*.so or linux-gate.so which should be ignored
+            # TODO: This check could be removed/relaxed
+            if not libname.startswith('linux-'):
+                raise LddError("Unexpected unresolved libname: " + libname)
+            logging.debug("Ignoring synthetic library: " + libname)
+            continue
+
+        # The library path must be absolute
+        if not libpath.startswith('/'):
+            raise LddError("Unexpected non-absolute libpath: " + libpath)
+        yield libpath
+
+
 def get_shobj_deps(path, libpath=[]):
     """Discover the dependencies of a shared object (*.so file)
     """
 
     # First verify we're dealing with a dynamic ELF file
     ensure_dynamic(path)
 
@@ -116,54 +159,15 @@
         #
         # GNU libc doesn't like something about the ELF headers of object files
         # produced by musl-libc
         #
         # We simply raise a specific exception and let the caller deal with it.
         raise LddError("Unexpected ldd error ({}): {}".format(rc, output))
 
-
-    # Example:
-    #	linux-vdso.so.1 (0x00007ffe53551000)
-    #     or
-    #	linux-vdso.so.1 =>  (0x00007ffe53551000)
-    #	libc.so.6 => /usr/lib64/libc.so.6 (0x00007f42ac010000)
-    #	/lib64/ld-linux-x86-64.so.2 (0x0000557376e75000)
-    pat = re.compile(r'\t([\w./+-]*) (?:=> ([\w./+-]*) )?\((0x[0-9a-fA-F]*)\)')
-
-    def parse():
-        for line in output.splitlines():
-            m = pat.match(line)
-            if not m:
-                # Some shared objs might have no DT_NEEDED tags (see issue #67)
-                if line == '\tstatically linked':
-                    break
-                raise LddError("Unexpected line in ldd output: " + line)
-            libname  = m.group(1)
-            libpath  = m.group(2)
-            baseaddr = int(m.group(3), 16)
-
-            if libname.startswith('/'):
-                # An absolute path here is probably INTERP
-                # and ldd shouldn't output the => /abs/path part.
-                if libpath:
-                    raise LddError("Unexpected line in ldd output: " + line)
-                yield libname
-            else:
-                # A short libname should come from a NEEDED tag
-                # and ldd should include the => /abs/path part.
-                # If it doesn't, then it's probably linux-vdso*.so
-                # or linux-gate.so
-                if not libpath:
-                    # TODO: This check could be removed/relaxed
-                    if libname.startswith('linux-'):
-                        continue
-                    raise LddError("Unexpected line in ldd output: " + line)
-                yield libpath
-
-    return list(parse())
+    return list(_parse_ldd_output(output))
 
 
 
 def elf_add_section(elfpath, secname, secfilename):
     tool_objcopy.run_check(
         '--add-section', '{}={}'.format(secname, secfilename),
         elfpath)
```

### Comparing `staticx-0.9.0/staticx/__main__.py` & `staticx-0.9.1/staticx/__main__.py`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/staticx/utils.py` & `staticx-0.9.1/staticx/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def make_mode_executable(mode):
     mode |= (mode & 0o444) >> 2    # copy R bits to X
     return mode
 
 
 def make_executable(path):
     mode = os.stat(path).st_mode
-    make_mode_executable(mode)
+    mode = make_mode_executable(mode)
     os.chmod(path, mode)
 
 def get_symlink_target(path):
     dirpath = os.path.dirname(os.path.abspath(path))
     return os.path.join(dirpath, os.readlink(path))
 
 def move_file(src, dst):
```

### Comparing `staticx-0.9.0/staticx/version.py` & `staticx-0.9.1/staticx/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # This logic has been adapted from that of PyInstaller
 # https://github.com/pyinstaller/pyinstaller/
 
 PACKAGEPATH = abspath(dirname(__file__))
 PROJPATH = dirname(PACKAGEPATH)
 
 # Base version, which will be augmented with Git information
-BASE_VERSION = '0.9.0'
+BASE_VERSION = '0.9.1'
 
 # This string will be replaced by `git-archive`
 # with the abbreviated commit hash
 git_archive_rev = "$Format:%h$"
 
 def git_describe():
     # Get the version from the local Git repository
```

### Comparing `staticx-0.9.0/staticx/bcjfilter.py` & `staticx-0.9.1/staticx/bcjfilter.py`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/staticx/api.py` & `staticx-0.9.1/staticx/api.py`

 * *Files identical despite different names*

### Comparing `staticx-0.9.0/staticx/errors.py` & `staticx-0.9.1/staticx/errors.py`

 * *Files identical despite different names*

