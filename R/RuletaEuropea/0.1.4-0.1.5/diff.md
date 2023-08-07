# Comparing `tmp/RuletaEuropea-0.1.4.tar.gz` & `tmp/RuletaEuropea-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RuletaEuropea-0.1.4.tar", last modified: Mon Aug  7 04:18:27 2023, max compression
+gzip compressed data, was "RuletaEuropea-0.1.5.tar", last modified: Mon Aug  7 04:21:13 2023, max compression
```

## Comparing `RuletaEuropea-0.1.4.tar` & `RuletaEuropea-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 04:18:27.647596 RuletaEuropea-0.1.4/
--rw-rw-rw-   0        0        0      146 2023-08-07 04:18:27.645597 RuletaEuropea-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 04:18:27.599463 RuletaEuropea-0.1.4/RuletaEuropea/
--rw-rw-rw-   0        0        0     2450 2023-08-07 04:08:14.000000 RuletaEuropea-0.1.4/RuletaEuropea/Apuesta.py
--rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.4/RuletaEuropea/Constantes.py
--rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.4/RuletaEuropea/Numero.py
--rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.4/RuletaEuropea/Ruleta.py
--rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.4/RuletaEuropea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 04:18:27.643588 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/
--rw-rw-rw-   0        0        0      146 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 04:18:27.647596 RuletaEuropea-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-08-07 04:17:54.000000 RuletaEuropea-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:21:13.122808 RuletaEuropea-0.1.5/
+-rw-rw-rw-   0        0        0      147 2023-08-07 04:21:13.117284 RuletaEuropea-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 04:21:13.107257 RuletaEuropea-0.1.5/RuletaEuropea/
+-rw-rw-rw-   0        0        0     2450 2023-08-07 04:08:14.000000 RuletaEuropea-0.1.5/RuletaEuropea/Apuesta.py
+-rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.5/RuletaEuropea/Constantes.py
+-rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.5/RuletaEuropea/Numero.py
+-rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.5/RuletaEuropea/Ruleta.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.5/RuletaEuropea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:21:13.113769 RuletaEuropea-0.1.5/RuletaEuropea.egg-info/
+-rw-rw-rw-   0        0        0      147 2023-08-07 04:21:12.000000 RuletaEuropea-0.1.5/RuletaEuropea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-07 04:21:13.000000 RuletaEuropea-0.1.5/RuletaEuropea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 04:21:12.000000 RuletaEuropea-0.1.5/RuletaEuropea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 04:21:12.000000 RuletaEuropea-0.1.5/RuletaEuropea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 04:21:13.124810 RuletaEuropea-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      241 2023-08-07 04:20:50.000000 RuletaEuropea-0.1.5/setup.py
```

### Comparing `RuletaEuropea-0.1.4/RuletaEuropea/Apuesta.py` & `RuletaEuropea-0.1.5/RuletaEuropea/Apuesta.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.4/RuletaEuropea/Constantes.py` & `RuletaEuropea-0.1.5/RuletaEuropea/Constantes.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.4/RuletaEuropea/Numero.py` & `RuletaEuropea-0.1.5/RuletaEuropea/Numero.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.4/RuletaEuropea/Ruleta.py` & `RuletaEuropea-0.1.5/RuletaEuropea/Ruleta.py`

 * *Files identical despite different names*

