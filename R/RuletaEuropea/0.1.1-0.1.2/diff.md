# Comparing `tmp/RuletaEuropea-0.1.1.tar.gz` & `tmp/RuletaEuropea-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RuletaEuropea-0.1.1.tar", last modified: Mon Aug  7 03:53:16 2023, max compression
+gzip compressed data, was "RuletaEuropea-0.1.2.tar", last modified: Mon Aug  7 04:00:38 2023, max compression
```

## Comparing `RuletaEuropea-0.1.1.tar` & `RuletaEuropea-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 03:53:16.601745 RuletaEuropea-0.1.1/
--rw-rw-rw-   0        0        0       85 2023-08-07 03:53:16.599735 RuletaEuropea-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 03:53:16.598226 RuletaEuropea-0.1.1/RuletaEuropea.egg-info/
--rw-rw-rw-   0        0        0       85 2023-08-07 03:53:16.000000 RuletaEuropea-0.1.1/RuletaEuropea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2023-08-07 03:53:16.000000 RuletaEuropea-0.1.1/RuletaEuropea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 03:53:16.000000 RuletaEuropea-0.1.1/RuletaEuropea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 03:53:16.000000 RuletaEuropea-0.1.1/RuletaEuropea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 03:53:16.601745 RuletaEuropea-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      167 2023-08-07 03:53:08.000000 RuletaEuropea-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:00:38.717403 RuletaEuropea-0.1.2/
+-rw-rw-rw-   0        0        0       85 2023-08-07 04:00:38.716395 RuletaEuropea-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 04:00:38.664265 RuletaEuropea-0.1.2/RuletaEuropea/
+-rw-rw-rw-   0        0        0     2457 2023-08-07 03:16:39.000000 RuletaEuropea-0.1.2/RuletaEuropea/Apuesta.py
+-rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.2/RuletaEuropea/Constantes.py
+-rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.2/RuletaEuropea/Numero.py
+-rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.2/RuletaEuropea/Ruleta.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.2/RuletaEuropea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:00:38.710887 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/
+-rw-rw-rw-   0        0        0       85 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 04:00:38.717403 RuletaEuropea-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      167 2023-08-07 04:00:19.000000 RuletaEuropea-0.1.2/setup.py
```

