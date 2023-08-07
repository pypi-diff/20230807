# Comparing `tmp/scidmcli-0.0.0.tar.gz` & `tmp/scidmcli-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scidmcli-0.0.0.tar", last modified: Mon Aug  7 06:24:15 2023, max compression
+gzip compressed data, was "scidmcli-0.0.1.tar", last modified: Mon Aug  7 07:46:50 2023, max compression
```

## Comparing `scidmcli-0.0.0.tar` & `scidmcli-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 06:24:15.947102 scidmcli-0.0.0/
--rw-r--r--   0 waue       (501) staff       (20)      300 2023-08-07 06:24:15.946886 scidmcli-0.0.0/PKG-INFO
--rw-r--r--   0 waue       (501) staff       (20)        1 2023-08-07 02:39:26.000000 scidmcli-0.0.0/README.md
--rw-r--r--   0 waue       (501) staff       (20)      584 2023-08-07 06:08:19.000000 scidmcli-0.0.0/pyproject.toml
--rw-r--r--   0 waue       (501) staff       (20)       38 2023-08-07 06:24:15.947142 scidmcli-0.0.0/setup.cfg
-drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 06:24:15.945424 scidmcli-0.0.0/src/
-drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 06:24:15.946040 scidmcli-0.0.0/src/scidmcli/
--rw-r--r--   0 waue       (501) staff       (20)        0 2023-08-07 02:40:08.000000 scidmcli-0.0.0/src/scidmcli/__init__.py
--rw-r--r--   0 waue       (501) staff       (20)        0 2023-08-07 02:40:19.000000 scidmcli-0.0.0/src/scidmcli/example.py
-drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 06:24:15.946690 scidmcli-0.0.0/src/scidmcli.egg-info/
--rw-r--r--   0 waue       (501) staff       (20)      300 2023-08-07 06:24:15.000000 scidmcli-0.0.0/src/scidmcli.egg-info/PKG-INFO
--rw-r--r--   0 waue       (501) staff       (20)      291 2023-08-07 06:24:15.000000 scidmcli-0.0.0/src/scidmcli.egg-info/SOURCES.txt
--rw-r--r--   0 waue       (501) staff       (20)        1 2023-08-07 06:24:15.000000 scidmcli-0.0.0/src/scidmcli.egg-info/dependency_links.txt
--rw-r--r--   0 waue       (501) staff       (20)       44 2023-08-07 06:24:15.000000 scidmcli-0.0.0/src/scidmcli.egg-info/entry_points.txt
--rw-r--r--   0 waue       (501) staff       (20)       41 2023-08-07 06:24:15.000000 scidmcli-0.0.0/src/scidmcli.egg-info/requires.txt
--rw-r--r--   0 waue       (501) staff       (20)        9 2023-08-07 06:24:15.000000 scidmcli-0.0.0/src/scidmcli.egg-info/top_level.txt
+drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 07:46:50.591733 scidmcli-0.0.1/
+-rw-r--r--   0 waue       (501) staff       (20)      300 2023-08-07 07:46:50.591572 scidmcli-0.0.1/PKG-INFO
+-rw-r--r--   0 waue       (501) staff       (20)        1 2023-08-07 02:39:26.000000 scidmcli-0.0.1/README.md
+-rw-r--r--   0 waue       (501) staff       (20)      549 2023-08-07 07:43:27.000000 scidmcli-0.0.1/pyproject.toml
+-rw-r--r--   0 waue       (501) staff       (20)       38 2023-08-07 07:46:50.591774 scidmcli-0.0.1/setup.cfg
+drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 07:46:50.589594 scidmcli-0.0.1/src/
+drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 07:46:50.590674 scidmcli-0.0.1/src/scidmcli/
+-rw-r--r--   0 waue       (501) staff       (20)      101 2023-08-07 07:39:07.000000 scidmcli-0.0.1/src/scidmcli/__init__.py
+-rw-r--r--   0 waue       (501) staff       (20)        0 2023-08-07 02:40:19.000000 scidmcli-0.0.1/src/scidmcli/example.py
+drwxr-xr-x   0 waue       (501) staff       (20)        0 2023-08-07 07:46:50.591414 scidmcli-0.0.1/src/scidmcli.egg-info/
+-rw-r--r--   0 waue       (501) staff       (20)      300 2023-08-07 07:46:50.000000 scidmcli-0.0.1/src/scidmcli.egg-info/PKG-INFO
+-rw-r--r--   0 waue       (501) staff       (20)      291 2023-08-07 07:46:50.000000 scidmcli-0.0.1/src/scidmcli.egg-info/SOURCES.txt
+-rw-r--r--   0 waue       (501) staff       (20)        1 2023-08-07 07:46:50.000000 scidmcli-0.0.1/src/scidmcli.egg-info/dependency_links.txt
+-rw-r--r--   0 waue       (501) staff       (20)       44 2023-08-07 07:46:50.000000 scidmcli-0.0.1/src/scidmcli.egg-info/entry_points.txt
+-rw-r--r--   0 waue       (501) staff       (20)       33 2023-08-07 07:46:50.000000 scidmcli-0.0.1/src/scidmcli.egg-info/requires.txt
+-rw-r--r--   0 waue       (501) staff       (20)        9 2023-08-07 07:46:50.000000 scidmcli-0.0.1/src/scidmcli.egg-info/top_level.txt
```

