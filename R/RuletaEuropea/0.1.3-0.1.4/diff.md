# Comparing `tmp/RuletaEuropea-0.1.3.tar.gz` & `tmp/RuletaEuropea-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RuletaEuropea-0.1.3.tar", last modified: Mon Aug  7 04:09:07 2023, max compression
+gzip compressed data, was "RuletaEuropea-0.1.4.tar", last modified: Mon Aug  7 04:18:27 2023, max compression
```

## Comparing `RuletaEuropea-0.1.3.tar` & `RuletaEuropea-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 04:09:07.777254 RuletaEuropea-0.1.3/
--rw-rw-rw-   0        0        0       85 2023-08-07 04:09:07.776255 RuletaEuropea-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 04:09:07.757222 RuletaEuropea-0.1.3/RuletaEuropea/
--rw-rw-rw-   0        0        0     2450 2023-08-07 04:08:14.000000 RuletaEuropea-0.1.3/RuletaEuropea/Apuesta.py
--rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.3/RuletaEuropea/Constantes.py
--rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.3/RuletaEuropea/Numero.py
--rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.3/RuletaEuropea/Ruleta.py
--rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.3/RuletaEuropea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 04:09:07.775254 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/
--rw-rw-rw-   0        0        0       85 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 04:09:07.777254 RuletaEuropea-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      167 2023-08-07 04:08:40.000000 RuletaEuropea-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:18:27.647596 RuletaEuropea-0.1.4/
+-rw-rw-rw-   0        0        0      146 2023-08-07 04:18:27.645597 RuletaEuropea-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 04:18:27.599463 RuletaEuropea-0.1.4/RuletaEuropea/
+-rw-rw-rw-   0        0        0     2450 2023-08-07 04:08:14.000000 RuletaEuropea-0.1.4/RuletaEuropea/Apuesta.py
+-rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.4/RuletaEuropea/Constantes.py
+-rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.4/RuletaEuropea/Numero.py
+-rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.4/RuletaEuropea/Ruleta.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.4/RuletaEuropea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:18:27.643588 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/
+-rw-rw-rw-   0        0        0      146 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 04:18:27.000000 RuletaEuropea-0.1.4/RuletaEuropea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 04:18:27.647596 RuletaEuropea-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      240 2023-08-07 04:17:54.000000 RuletaEuropea-0.1.4/setup.py
```

### Comparing `RuletaEuropea-0.1.3/RuletaEuropea/Apuesta.py` & `RuletaEuropea-0.1.4/RuletaEuropea/Apuesta.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.3/RuletaEuropea/Constantes.py` & `RuletaEuropea-0.1.4/RuletaEuropea/Constantes.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.3/RuletaEuropea/Numero.py` & `RuletaEuropea-0.1.4/RuletaEuropea/Numero.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.3/RuletaEuropea/Ruleta.py` & `RuletaEuropea-0.1.4/RuletaEuropea/Ruleta.py`

 * *Files identical despite different names*

