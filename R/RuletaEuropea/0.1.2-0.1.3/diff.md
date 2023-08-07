# Comparing `tmp/RuletaEuropea-0.1.2.tar.gz` & `tmp/RuletaEuropea-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RuletaEuropea-0.1.2.tar", last modified: Mon Aug  7 04:00:38 2023, max compression
+gzip compressed data, was "RuletaEuropea-0.1.3.tar", last modified: Mon Aug  7 04:09:07 2023, max compression
```

## Comparing `RuletaEuropea-0.1.2.tar` & `RuletaEuropea-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-07 04:00:38.717403 RuletaEuropea-0.1.2/
--rw-rw-rw-   0        0        0       85 2023-08-07 04:00:38.716395 RuletaEuropea-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-07 04:00:38.664265 RuletaEuropea-0.1.2/RuletaEuropea/
--rw-rw-rw-   0        0        0     2457 2023-08-07 03:16:39.000000 RuletaEuropea-0.1.2/RuletaEuropea/Apuesta.py
--rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.2/RuletaEuropea/Constantes.py
--rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.2/RuletaEuropea/Numero.py
--rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.2/RuletaEuropea/Ruleta.py
--rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.2/RuletaEuropea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-07 04:00:38.710887 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/
--rw-rw-rw-   0        0        0       85 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-08-07 04:00:38.000000 RuletaEuropea-0.1.2/RuletaEuropea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-07 04:00:38.717403 RuletaEuropea-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      167 2023-08-07 04:00:19.000000 RuletaEuropea-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:09:07.777254 RuletaEuropea-0.1.3/
+-rw-rw-rw-   0        0        0       85 2023-08-07 04:09:07.776255 RuletaEuropea-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-07 04:09:07.757222 RuletaEuropea-0.1.3/RuletaEuropea/
+-rw-rw-rw-   0        0        0     2450 2023-08-07 04:08:14.000000 RuletaEuropea-0.1.3/RuletaEuropea/Apuesta.py
+-rw-rw-rw-   0        0        0      854 2023-08-03 04:49:11.000000 RuletaEuropea-0.1.3/RuletaEuropea/Constantes.py
+-rw-rw-rw-   0        0        0     2932 2023-08-03 04:49:22.000000 RuletaEuropea-0.1.3/RuletaEuropea/Numero.py
+-rw-rw-rw-   0        0        0     2419 2023-08-03 04:49:30.000000 RuletaEuropea-0.1.3/RuletaEuropea/Ruleta.py
+-rw-rw-rw-   0        0        0        0 2023-08-03 04:45:02.000000 RuletaEuropea-0.1.3/RuletaEuropea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-07 04:09:07.775254 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/
+-rw-rw-rw-   0        0        0       85 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-07 04:09:07.000000 RuletaEuropea-0.1.3/RuletaEuropea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 04:09:07.777254 RuletaEuropea-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      167 2023-08-07 04:08:40.000000 RuletaEuropea-0.1.3/setup.py
```

### Comparing `RuletaEuropea-0.1.2/RuletaEuropea/Apuesta.py` & `RuletaEuropea-0.1.3/RuletaEuropea/Apuesta.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,21 +24,21 @@
         self.cantidad_apostada = int(cantidad_apostada)
         self.cantidad_a_ganar = self.calcular_paga()
 
     def __str__(self):
         return f"Usuario: {self.usuario}, Apuesta: {self.apuesta}, Jugada: {self.jugada}, Cantidad apostada: {self.cantidad_apostada}, Cantidad a ganar: {self.cantidad_a_ganar}"
 
     def str_apuesta(self):
-        return f"{self.usuario} apostó ¢ {self.cantidad_apostada} jugando {self.apuesta} {self.jugada}!"
+        return f"{self.usuario} apostó $ {self.cantidad_apostada} jugando {self.apuesta} {self.jugada}!"
 
     def str_ganador(self):
-        return f"{self.usuario} apostó ¢ {self.cantidad_apostada} jugando {self.apuesta} {self.jugada} y ganó ¢ {self.cantidad_ganada()}!"
+        return f"{self.usuario} apostó $ {self.cantidad_apostada} jugando {self.apuesta} {self.jugada} y ganó $ {self.cantidad_ganada()}!"
     
     def str_perdedor(self):
-        return f"{self.usuario} perdió ¢ {self.cantidad_apostada} jugando {self.apuesta} {self.jugada} :c"
+        return f"{self.usuario} perdió $ {self.cantidad_apostada} jugando {self.apuesta} {self.jugada}"
 
     def calcular_paga(self):
         if self.apuesta == APUESTA_COLOR:
             if self.jugada == VERDE:
                 return self.cantidad_apostada * PAGA_COLOR_VERDE
             else:
                 return self.cantidad_apostada * PAGA_COLOR_NEGRO_ROJO
```

### Comparing `RuletaEuropea-0.1.2/RuletaEuropea/Constantes.py` & `RuletaEuropea-0.1.3/RuletaEuropea/Constantes.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.2/RuletaEuropea/Numero.py` & `RuletaEuropea-0.1.3/RuletaEuropea/Numero.py`

 * *Files identical despite different names*

### Comparing `RuletaEuropea-0.1.2/RuletaEuropea/Ruleta.py` & `RuletaEuropea-0.1.3/RuletaEuropea/Ruleta.py`

 * *Files identical despite different names*

