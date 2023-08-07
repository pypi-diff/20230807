# Comparing `tmp/french_cities-0.1.1a3.tar.gz` & `tmp/french_cities-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "french_cities-0.1.1a3.tar", max compression
+gzip compressed data, was "french_cities-0.1.1a4.tar", max compression
```

## Comparing `french_cities-0.1.1a3.tar` & `french_cities-0.1.1a4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10122 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/README.fr.md
--rw-r--r--   0        0        0     8563 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/README.md
--rw-r--r--   0        0        0      394 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/french_cities/__init__.py
--rw-r--r--   0        0        0    30549 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/french_cities/city_finder.py
--rw-r--r--   0        0        0     9317 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/french_cities/departement_finder.py
--rw-r--r--   0        0        0      519 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/french_cities/utils.py
--rw-r--r--   0        0        0     7956 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/french_cities/vintage.py
--rw-r--r--   0        0        0     1279 2023-08-07 10:20:45.520014 french_cities-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0    20232 1970-01-01 00:00:00.000000 french_cities-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0    10122 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/README.fr.md
+-rw-r--r--   0        0        0     8563 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/README.md
+-rw-r--r--   0        0        0      394 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/french_cities/__init__.py
+-rw-r--r--   0        0        0    30912 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/french_cities/city_finder.py
+-rw-r--r--   0        0        0     9317 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/french_cities/departement_finder.py
+-rw-r--r--   0        0        0      519 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/french_cities/utils.py
+-rw-r--r--   0        0        0     7956 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/french_cities/vintage.py
+-rw-r--r--   0        0        0     1279 2023-08-07 11:50:39.244466 french_cities-0.1.1a4/pyproject.toml
+-rw-r--r--   0        0        0    20232 1970-01-01 00:00:00.000000 french_cities-0.1.1a4/PKG-INFO
```

### Comparing `french_cities-0.1.1a3/README.fr.md` & `french_cities-0.1.1a4/README.fr.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.1a3/README.md` & `french_cities-0.1.1a4/README.md`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.1a3/french_cities/city_finder.py` & `french_cities-0.1.1a4/french_cities/city_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 from pynsee.geodata import get_geodata
 from pynsee.localdata import get_area_list
 import geopandas as gpd
 from pyproj import Transformer
 from datetime import date, timedelta
 from typing import Union
 import numpy as np
-from geopy.extra.rate_limiter import RateLimiter
-from geopy.geocoders import Nominatim
 from functools import partial
 from uuid import uuid4
 from tqdm import tqdm
 from pebble import ThreadPool
+try:
+    from geopy.extra.rate_limiter import RateLimiter
+    from geopy.geocoders import Nominatim
+except ModuleNotFoundError:
+    pass
+
 
 from french_cities.vintage import set_vintage
 from french_cities.departement_finder import find_departements
 from french_cities.utils import init_pynsee
 
 
 logger = logging.getLogger(__name__)
@@ -376,15 +380,16 @@
             if missing.empty:
                 continue
             missing = _find_with_nominatim_geolocation(
                 year=year,
                 look_for=missing[["query"]],
                 alias="insee_com_nominatim",
             )
-
+            if missing.empty:
+                continue
             missing = find_departements(
                 missing,
                 source="insee_com_nominatim",
                 alias="dep_nominatim",
                 type_code="insee",
             )
             temp = df.loc[ix]
@@ -451,15 +456,23 @@
     """
 
     logger.info(
         "Please read Nominatim Usage Policy at "
         "https://operations.osmfoundation.org/policies/nominatim/"
     )
     user_agent = f"french-cities-{uuid4()}"
-    geolocator = Nominatim(user_agent=user_agent)
+    try:
+        geolocator = Nominatim(user_agent=user_agent)
+    except NameError:
+        logger.error(
+            "geopy not installed - please install optional dependencies "
+            "to use Nominatim geocoder with: pip install french-cities[full]"
+        )
+        return pd.DataFrame()
+        
     geocode = RateLimiter(
         partial(
             geolocator.geocode,
             language="fr",
             country_codes="fr",
             featuretype="settlement ",
         ),
```

### Comparing `french_cities-0.1.1a3/french_cities/departement_finder.py` & `french_cities-0.1.1a4/french_cities/departement_finder.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.1a3/french_cities/utils.py` & `french_cities-0.1.1a4/french_cities/utils.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.1a3/french_cities/vintage.py` & `french_cities-0.1.1a4/french_cities/vintage.py`

 * *Files identical despite different names*

### Comparing `french_cities-0.1.1a3/pyproject.toml` & `french_cities-0.1.1a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "french-cities"
-version = "0.1.1a3"
+version = "0.1.1a4"
 description = "Toolbox on french cities: set vintage, find departments, find cities..."
 authors = ["thomas.grandjean <thomas.grandjean@developpement-durable.gouv.fr>"]
 license = "etalab-2.0"
 readme = ["README.md", "README.fr.md"]
 homepage = "https://github.com/tgrandje/french-cities/"
 repository = "https://github.com/tgrandje/french-cities/"
 documentation = "https://github.com/tgrandje/french-cities/"
```

### Comparing `french_cities-0.1.1a3/PKG-INFO` & `french_cities-0.1.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: french-cities
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: Toolbox on french cities: set vintage, find departments, find cities...
 Home-page: https://github.com/tgrandje/french-cities/
 License: etalab-2.0
 Keywords: france,cities
 Author: thomas.grandjean
 Author-email: thomas.grandjean@developpement-durable.gouv.fr
 Requires-Python: >=3.8,<4.0
```

