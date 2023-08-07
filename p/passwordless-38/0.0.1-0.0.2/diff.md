# Comparing `tmp/passwordless-38-0.0.1.tar.gz` & `tmp/passwordless-38-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-38-0.0.1.tar", last modified: Tue Aug  1 22:27:27 2023, max compression
+gzip compressed data, was "passwordless-38-0.0.2.tar", last modified: Mon Aug  7 06:14:07 2023, max compression
```

## Comparing `passwordless-38-0.0.1.tar` & `passwordless-38-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:27:27.987113 passwordless-38-0.0.1/
--rw-rw-rw-   0        0        0      481 2023-08-01 22:27:27.987113 passwordless-38-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 22:27:27.986102 passwordless-38-0.0.1/passwordless_38.egg-info/
--rw-rw-rw-   0        0        0      481 2023-08-01 22:27:27.000000 passwordless-38-0.0.1/passwordless_38.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2023-08-01 22:27:27.000000 passwordless-38-0.0.1/passwordless_38.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:27:27.000000 passwordless-38-0.0.1/passwordless_38.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 22:27:27.000000 passwordless-38-0.0.1/passwordless_38.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 22:27:27.987113 passwordless-38-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-08-01 22:27:17.000000 passwordless-38-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 06:14:07.946242 passwordless-38-0.0.2/
+-rw-rw-rw-   0        0        0     4215 2023-08-07 06:14:07.945725 passwordless-38-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3587 2023-08-04 10:48:54.000000 passwordless-38-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 06:14:07.945209 passwordless-38-0.0.2/passwordless_38.egg-info/
+-rw-rw-rw-   0        0        0     4215 2023-08-07 06:14:07.000000 passwordless-38-0.0.2/passwordless_38.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-08-07 06:14:07.000000 passwordless-38-0.0.2/passwordless_38.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:14:07.000000 passwordless-38-0.0.2/passwordless_38.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-07 06:14:07.000000 passwordless-38-0.0.2/passwordless_38.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 06:14:07.000000 passwordless-38-0.0.2/passwordless_38.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 06:14:07.946756 passwordless-38-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-08-07 06:08:18.000000 passwordless-38-0.0.2/setup.py
```

