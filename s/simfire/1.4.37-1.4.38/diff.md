# Comparing `tmp/simfire-1.4.37.tar.gz` & `tmp/simfire-1.4.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfire-1.4.37.tar", max compression
+gzip compressed data, was "simfire-1.4.38.tar", max compression
```

## Comparing `simfire-1.4.37.tar` & `simfire-1.4.38.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    10789 2023-05-15 20:54:59.340527 simfire-1.4.37/LICENSE
--rw-r--r--   0        0        0     2662 2023-05-15 20:54:59.340527 simfire-1.4.37/README.md
--rw-r--r--   0        0        0     1852 2023-05-15 20:54:59.536528 simfire-1.4.37/pyproject.toml
--rw-r--r--   0        0        0     1111 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/__init__.py
--rw-r--r--   0        0        0    10729 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/enums.py
--rw-r--r--   0        0        0       37 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/__init__.py
--rw-r--r--   0        0        0      874 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/_tests/__init__.py
--rw-r--r--   0        0        0    15523 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/_tests/test_game.py
--rw-r--r--   0        0        0     9928 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/_tests/test_sprites.py
--rw-r--r--   0        0        0    14937 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/game.py
--rw-r--r--   0        0        0     1318 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/image.py
--rw-r--r--   0        0        0      379 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.536528 simfire-1.4.37/simfire/game/managers/_tests/__init__.py
--rw-r--r--   0        0        0    18385 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/game/managers/_tests/test_fire.py
--rw-r--r--   0        0        0     8301 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/game/managers/_tests/test_mitigation.py
--rw-r--r--   0        0        0    29762 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/game/managers/fire.py
--rw-r--r--   0        0        0     7321 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/game/managers/mitigation.py
--rw-r--r--   0        0        0    15972 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/game/sprites.py
--rw-r--r--   0        0        0       49 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/sim/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/sim/_tests/__init__.py
--rw-r--r--   0        0        0    14392 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/sim/_tests/test_simulation.py
--rw-r--r--   0        0        0    37815 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/sim/simulation.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/__init__.py
--rw-r--r--   0        0        0     2771 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_config.py
--rw-r--r--   0        0        0     1925 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_configs/test_config.yml
--rw-r--r--   0        0        0       47 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_bad.yml
--rw-r--r--   0        0        0     1874 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
--rw-r--r--   0        0        0     1876 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_gaussian.yml
--rw-r--r--   0        0        0     1851 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
--rw-r--r--   0        0        0     4693 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_graph.py
--rw-r--r--   0        0        0    17172 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_layers.py
--rw-r--r--   0        0        0      622 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_log.py
--rw-r--r--   0        0        0     4495 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_terrain.py
--rw-r--r--   0        0        0     1472 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/_tests/test_units.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/assets/__init__.py
--rw-r--r--   0        0        0     1854 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/assets/fireline_logo.png
--rw-r--r--   0        0        0    39144 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/config.py
--rw-r--r--   0        0        0      499 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/decorators.py
--rw-r--r--   0        0        0     4153 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/generate_cfd_wind_layer.py
--rw-r--r--   0        0        0    10189 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/graph.py
--rw-r--r--   0        0        0    51105 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/layers.py
--rw-r--r--   0        0        0     2030 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/log.py
--rw-r--r--   0        0        0   143776 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
--rw-r--r--   0        0        0   143776 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
--rw-r--r--   0        0        0     3647 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/terrain.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/textures/__init__.py
--rw-r--r--   0        0        0   204702 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/textures/terrain.jpg
--rw-r--r--   0        0        0     2555 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/utils/units.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/world/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/world/_tests/__init__.py
--rw-r--r--   0        0        0     2184 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/world/_tests/test_cfd_wind.py
--rw-r--r--   0        0        0     2423 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/world/_tests/test_elevation_functions.py
--rw-r--r--   0        0        0     2821 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/world/_tests/test_rothermel.py
--rw-r--r--   0        0        0     1466 2023-05-15 20:54:59.540528 simfire-1.4.37/simfire/world/_tests/test_wind.py
--rw-r--r--   0        0        0     3703 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/elevation_functions.py
--rw-r--r--   0        0        0     1054 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/fuel_array_functions.py
--rw-r--r--   0        0        0     2306 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/parameters.py
--rw-r--r--   0        0        0     2083 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/presets.py
--rw-r--r--   0        0        0     4306 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/rothermel.py
--rw-r--r--   0        0        0        0 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/wind_mechanics/__init__.py
--rw-r--r--   0        0        0     8781 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/wind_mechanics/cfd_wind.py
--rw-r--r--   0        0        0     3132 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/wind_mechanics/perlin_wind.py
--rw-r--r--   0        0        0     6578 2023-05-15 20:54:59.544528 simfire-1.4.37/simfire/world/wind_mechanics/wind_controller.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 simfire-1.4.37/PKG-INFO
+-rw-r--r--   0        0        0    10789 2023-08-07 20:08:26.923408 simfire-1.4.38/LICENSE
+-rw-r--r--   0        0        0     2662 2023-08-07 20:08:26.923408 simfire-1.4.38/README.md
+-rw-r--r--   0        0        0     1852 2023-08-07 20:08:27.155418 simfire-1.4.38/pyproject.toml
+-rw-r--r--   0        0        0     1111 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/__init__.py
+-rw-r--r--   0        0        0    10729 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/enums.py
+-rw-r--r--   0        0        0       37 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/__init__.py
+-rw-r--r--   0        0        0      874 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/_tests/__init__.py
+-rw-r--r--   0        0        0    15523 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/_tests/test_game.py
+-rw-r--r--   0        0        0     9928 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/_tests/test_sprites.py
+-rw-r--r--   0        0        0    14937 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/game.py
+-rw-r--r--   0        0        0     1318 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/image.py
+-rw-r--r--   0        0        0      379 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/_tests/__init__.py
+-rw-r--r--   0        0        0    18385 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/_tests/test_fire.py
+-rw-r--r--   0        0        0     8301 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/_tests/test_mitigation.py
+-rw-r--r--   0        0        0    29897 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/fire.py
+-rw-r--r--   0        0        0     7321 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/managers/mitigation.py
+-rw-r--r--   0        0        0    15972 2023-08-07 20:08:27.155418 simfire-1.4.38/simfire/game/sprites.py
+-rw-r--r--   0        0        0       49 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/_tests/__init__.py
+-rw-r--r--   0        0        0    14392 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/_tests/test_simulation.py
+-rw-r--r--   0        0        0    37815 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/sim/simulation.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/__init__.py
+-rw-r--r--   0        0        0     2771 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_config.py
+-rw-r--r--   0        0        0     1925 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config.yml
+-rw-r--r--   0        0        0       47 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_bad.yml
+-rw-r--r--   0        0        0     1874 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_flat_simple.yml
+-rw-r--r--   0        0        0     1876 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_gaussian.yml
+-rw-r--r--   0        0        0     1851 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml
+-rw-r--r--   0        0        0     4693 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_graph.py
+-rw-r--r--   0        0        0    17172 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_layers.py
+-rw-r--r--   0        0        0      622 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_log.py
+-rw-r--r--   0        0        0     4495 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_terrain.py
+-rw-r--r--   0        0        0     1472 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/_tests/test_units.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/assets/__init__.py
+-rw-r--r--   0        0        0     1854 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/assets/fireline_logo.png
+-rw-r--r--   0        0        0    39144 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/config.py
+-rw-r--r--   0        0        0      499 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/decorators.py
+-rw-r--r--   0        0        0     4153 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/generate_cfd_wind_layer.py
+-rw-r--r--   0        0        0    10189 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/graph.py
+-rw-r--r--   0        0        0    51105 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/layers.py
+-rw-r--r--   0        0        0     2030 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/log.py
+-rw-r--r--   0        0        0   143776 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy
+-rw-r--r--   0        0        0   143776 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy
+-rw-r--r--   0        0        0     3647 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/terrain.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/textures/__init__.py
+-rw-r--r--   0        0        0   204702 2023-08-07 20:08:27.159418 simfire-1.4.38/simfire/utils/textures/terrain.jpg
+-rw-r--r--   0        0        0     2555 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/utils/units.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/__init__.py
+-rw-r--r--   0        0        0     2184 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_cfd_wind.py
+-rw-r--r--   0        0        0     2423 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_elevation_functions.py
+-rw-r--r--   0        0        0     2821 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_rothermel.py
+-rw-r--r--   0        0        0     1466 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/_tests/test_wind.py
+-rw-r--r--   0        0        0     3703 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/elevation_functions.py
+-rw-r--r--   0        0        0     1054 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/fuel_array_functions.py
+-rw-r--r--   0        0        0     2306 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/parameters.py
+-rw-r--r--   0        0        0     2083 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/presets.py
+-rw-r--r--   0        0        0     4306 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/rothermel.py
+-rw-r--r--   0        0        0        0 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/__init__.py
+-rw-r--r--   0        0        0     8781 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/cfd_wind.py
+-rw-r--r--   0        0        0     3132 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/perlin_wind.py
+-rw-r--r--   0        0        0     6578 2023-08-07 20:08:27.163418 simfire-1.4.38/simfire/world/wind_mechanics/wind_controller.py
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 simfire-1.4.38/PKG-INFO
```

### Comparing `simfire-1.4.37/LICENSE` & `simfire-1.4.38/LICENSE`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/README.md` & `simfire-1.4.38/README.md`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/pyproject.toml` & `simfire-1.4.38/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simfire"
-version = "1.4.37"
+version = "1.4.38"
 description = "Fire simulator built in Python"
 authors = ["Tim Welsh <twelsh@mitre.org>", "Marissa Dotter <mdotter@mitre.org>",
            "Michael Doyle <mdoyle@mitre.org>", "Dhanuj Gandikota <dgandikota@mitre.org>",
            "Chris Kempis <ckempis@mitre.org>", "Lauren Schambach <lschambach@mitre.org>",
            "Alex Tapley <atapley@mitre.org>", "Michael Threet <mthreet@mitre.org>"]
 readme = "README.md"
 include = ["simfire/utils/textures/terrain.jpg", "simfire/utils/assets/fireline_logo.png"]
```

### Comparing `simfire-1.4.37/simfire/__init__.py` & `simfire-1.4.38/simfire/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/enums.py` & `simfire-1.4.38/simfire/enums.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/_tests/__init__.py` & `simfire-1.4.38/simfire/game/_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/_tests/test_game.py` & `simfire-1.4.38/simfire/game/_tests/test_game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/_tests/test_sprites.py` & `simfire-1.4.38/simfire/game/_tests/test_sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/game.py` & `simfire-1.4.38/simfire/game/game.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/image.py` & `simfire-1.4.38/simfire/game/image.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/managers/_tests/test_fire.py` & `simfire-1.4.38/simfire/game/managers/_tests/test_fire.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/managers/_tests/test_mitigation.py` & `simfire-1.4.38/simfire/game/managers/_tests/test_mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/managers/fire.py` & `simfire-1.4.38/simfire/game/managers/fire.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,14 +339,17 @@
         self.U, self.U_dir = self._get_environment_parameters(environment)
 
         # Keep track of how much each pixel has burned.
         # This is needed since each pixel represents a specific number of feet
         # and it might take more than one update to burn
         self.burn_amounts = np.zeros_like(self.terrain.fuels)
 
+        # Keep track of how much each pixel is currently burning
+        self.rate_of_spread = np.zeros_like(self.terrain.fuels)
+
         # Pre-compute the slope magnitudes and directions for use with
         # Rothermel calculation
         self.slope_mag, self.slope_dir = self._compute_slopes()
 
         # Create a FireSpreadGraph to track the fire
         self.fs_graph = FireSpreadGraph(self.terrain.screen_size)
 
@@ -673,15 +676,15 @@
         # Create a rate_of_spread variable that takes the same shape as self.burn_amounts
         # and fire_map
         rate_of_spread = np.zeros_like(self.burn_amounts)
         rate_of_spread[y_coords, x_coords] = R
 
         # Update the burn_amounts dependent on if there are control lines there
         # And only update if specified in the class
-        rate_of_spread = self._update_rate_of_spread(rate_of_spread, fire_map)
+        self.rate_of_spread = self._update_rate_of_spread(rate_of_spread, fire_map)
         self.burn_amounts += rate_of_spread
 
         # Update the fire_map with new burning locations and update self.sprites and
         # self.durations
         fire_map = self._update_with_new_locs(y_coords, x_coords, fire_map)
 
         # Save the new elapsed_time value
```

### Comparing `simfire-1.4.37/simfire/game/managers/mitigation.py` & `simfire-1.4.38/simfire/game/managers/mitigation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/game/sprites.py` & `simfire-1.4.38/simfire/game/sprites.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/sim/_tests/test_simulation.py` & `simfire-1.4.38/simfire/sim/_tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/sim/simulation.py` & `simfire-1.4.38/simfire/sim/simulation.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_config.py` & `simfire-1.4.38/simfire/utils/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_configs/test_config.yml` & `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_flat_simple.yml` & `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_flat_simple.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_gaussian.yml` & `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_gaussian.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml` & `simfire-1.4.38/simfire/utils/_tests/test_configs/test_config_rothermel_manager.yml`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_graph.py` & `simfire-1.4.38/simfire/utils/_tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_layers.py` & `simfire-1.4.38/simfire/utils/_tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_log.py` & `simfire-1.4.38/simfire/utils/_tests/test_log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_terrain.py` & `simfire-1.4.38/simfire/utils/_tests/test_terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/_tests/test_units.py` & `simfire-1.4.38/simfire/utils/_tests/test_units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/assets/fireline_logo.png` & `simfire-1.4.38/simfire/utils/assets/fireline_logo.png`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/config.py` & `simfire-1.4.38/simfire/utils/config.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/generate_cfd_wind_layer.py` & `simfire-1.4.38/simfire/utils/generate_cfd_wind_layer.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/graph.py` & `simfire-1.4.38/simfire/utils/graph.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/layers.py` & `simfire-1.4.38/simfire/utils/layers.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/log.py` & `simfire-1.4.38/simfire/utils/log.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy` & `simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_directions.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy` & `simfire-1.4.38/simfire/utils/pregenerated_wind_files/generated_wind_magnitudes.npy`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/terrain.py` & `simfire-1.4.38/simfire/utils/terrain.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/textures/terrain.jpg` & `simfire-1.4.38/simfire/utils/textures/terrain.jpg`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/utils/units.py` & `simfire-1.4.38/simfire/utils/units.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/_tests/test_cfd_wind.py` & `simfire-1.4.38/simfire/world/_tests/test_cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/_tests/test_elevation_functions.py` & `simfire-1.4.38/simfire/world/_tests/test_elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/_tests/test_rothermel.py` & `simfire-1.4.38/simfire/world/_tests/test_rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/_tests/test_wind.py` & `simfire-1.4.38/simfire/world/_tests/test_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/elevation_functions.py` & `simfire-1.4.38/simfire/world/elevation_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/fuel_array_functions.py` & `simfire-1.4.38/simfire/world/fuel_array_functions.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/parameters.py` & `simfire-1.4.38/simfire/world/parameters.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/presets.py` & `simfire-1.4.38/simfire/world/presets.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/rothermel.py` & `simfire-1.4.38/simfire/world/rothermel.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/wind_mechanics/cfd_wind.py` & `simfire-1.4.38/simfire/world/wind_mechanics/cfd_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/wind_mechanics/perlin_wind.py` & `simfire-1.4.38/simfire/world/wind_mechanics/perlin_wind.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/simfire/world/wind_mechanics/wind_controller.py` & `simfire-1.4.38/simfire/world/wind_mechanics/wind_controller.py`

 * *Files identical despite different names*

### Comparing `simfire-1.4.37/PKG-INFO` & `simfire-1.4.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfire
-Version: 1.4.37
+Version: 1.4.38
 Summary: Fire simulator built in Python
 Home-page: https://gitlab.mitre.org/fireline/simfire
 Keywords: python,reinforcement learning,simulation,fire
 Author: Tim Welsh
 Author-email: twelsh@mitre.org
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
```

