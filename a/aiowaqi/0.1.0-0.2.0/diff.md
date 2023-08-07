# Comparing `tmp/aiowaqi-0.1.0.tar.gz` & `tmp/aiowaqi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiowaqi-0.1.0.tar", max compression
+gzip compressed data, was "aiowaqi-0.2.0.tar", max compression
```

## Comparing `aiowaqi-0.1.0.tar` & `aiowaqi-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     5203 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/README.md
--rw-r--r--   0        0        0     3601 2023-08-07 20:28:09.497540 aiowaqi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      694 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/src/aiowaqi/__init__.py
--rw-r--r--   0        0        0      438 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/src/aiowaqi/exceptions.py
--rw-r--r--   0        0        0     3720 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/src/aiowaqi/models.py
--rw-r--r--   0        0        0        0 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/src/aiowaqi/py.typed
--rw-r--r--   0        0        0     5627 2023-08-07 20:27:51.905164 aiowaqi-0.1.0/src/aiowaqi/waqi.py
--rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 aiowaqi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     5203 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/README.md
+-rw-r--r--   0        0        0     3601 2023-08-07 21:20:31.890514 aiowaqi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      694 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/src/aiowaqi/__init__.py
+-rw-r--r--   0        0        0      438 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/src/aiowaqi/exceptions.py
+-rw-r--r--   0        0        0     4369 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/src/aiowaqi/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/src/aiowaqi/py.typed
+-rw-r--r--   0        0        0     5627 2023-08-07 21:20:14.698195 aiowaqi-0.2.0/src/aiowaqi/waqi.py
+-rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 aiowaqi-0.2.0/PKG-INFO
```

### Comparing `aiowaqi-0.1.0/LICENSE.md` & `aiowaqi-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiowaqi-0.1.0/README.md` & `aiowaqi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aiowaqi-0.1.0/pyproject.toml` & `aiowaqi-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiowaqi"
-version = "0.1.0"
+version = "0.2.0"
 description = "Asynchronous Python client for WAQI API."
 authors = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 maintainers = ["Joost Lekkerkerker <joostlek@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joostlek/python-waqi"
 repository = "https://github.com/joostlek/python-waqi"
```

### Comparing `aiowaqi-0.1.0/src/aiowaqi/__init__.py` & `aiowaqi-0.2.0/src/aiowaqi/__init__.py`

 * *Files identical despite different names*

### Comparing `aiowaqi-0.1.0/src/aiowaqi/models.py` & `aiowaqi-0.2.0/src/aiowaqi/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 """Asynchronous Python client for the WAQI API."""
 from __future__ import annotations
 
 from contextlib import suppress
 from dataclasses import dataclass
+from datetime import datetime
+from enum import Enum
+from typing import Any
 
 try:
     from pydantic.v1 import BaseModel, Field, validator
 except ImportError:  # pragma: no cover
     from pydantic import (  # type: ignore[assignment] # pragma: no cover
         BaseModel,
         Field,
         validator,
     )
 
 
+class Pollutant(str, Enum):
+    """Enum of pollutants."""
+
+    CARBON_MONOXIDE = "co"
+    NITROGEN_DIOXIDE = "no2"
+    OZONE = "o3"
+    SULPHUR_DIOXIDE = "so2"
+    PM10 = "pm10"
+    PM25 = "pm25"
+
+
 class Attribution(BaseModel):
     """Represents an attribution."""
 
     url: str = Field(...)
     name: str = Field(...)
     logo: str | None = Field(None)
 
@@ -105,27 +119,39 @@
     """Represents the air quality data from WAQI."""
 
     air_quality_index: int | None = Field(None, alias="aqi")
     station_id: int = Field(..., alias="idx")
     attributions: list[Attribution] = Field([])
     city: City = Field(...)
     extended_air_quality: WAQIExtendedAirQuality = Field(..., alias="iaqi")
+    dominant_pollutant: Pollutant = Field(..., alias="dominentpol")
+    measured_at: datetime = Field(..., alias="time")
 
     @validator(
         "air_quality_index",
         pre=True,
         allow_reuse=True,
     )
     @classmethod
     def get_value(cls, value: int | str) -> int | None:
         """Handle invalid string."""
         with suppress(ValueError):
             return int(value)
         return None
 
+    @validator(
+        "measured_at",
+        pre=True,
+        allow_reuse=True,
+    )
+    @classmethod
+    def get_datetime(cls, value: dict[str, Any]) -> datetime:
+        """Get measuring date."""
+        return datetime.fromisoformat(value["iso"])
+
 
 class WAQISearchResult(BaseModel):
     """Represents a search result from the WAQI api."""
 
     air_quality_index: int | None = Field(None, alias="aqi")
     station_id: int = Field(..., alias="uid")
     station: Station = Field(...)
```

### Comparing `aiowaqi-0.1.0/src/aiowaqi/waqi.py` & `aiowaqi-0.2.0/src/aiowaqi/waqi.py`

 * *Files identical despite different names*

### Comparing `aiowaqi-0.1.0/PKG-INFO` & `aiowaqi-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiowaqi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Asynchronous Python client for WAQI API.
 Home-page: https://github.com/joostlek/python-waqi
 License: MIT
 Keywords: WAQI,api,async,client
 Author: Joost Lekkerkerker
 Author-email: joostlek@outlook.com
 Maintainer: Joost Lekkerkerker
```

