# Comparing `tmp/dfipy-1.0.2.tar.gz` & `tmp/dfipy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-1.0.2.tar", max compression
+gzip compressed data, was "dfipy-2.0.0.tar", max compression
```

## Comparing `dfipy-1.0.2.tar` & `dfipy-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      568 2023-07-06 09:33:03.982869 dfipy-1.0.2/LICENCE
--rw-r--r--   0        0        0     1808 2023-07-06 09:33:03.982869 dfipy-1.0.2/README.md
--rw-r--r--   0        0        0       99 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/__init__.py
--rw-r--r--   0        0        0    14187 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/analyse.py
--rw-r--r--   0        0        0     1418 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/client.py
--rw-r--r--   0        0        0     3662 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/connect.py
--rw-r--r--   0        0        0    20008 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/get.py
--rw-r--r--   0        0        0     1320 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/models.py
--rw-r--r--   0        0        0     2803 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/polygons.py
--rw-r--r--   0        0        0     5196 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/show.py
--rw-r--r--   0        0        0    11102 2023-07-06 09:33:03.982869 dfipy-1.0.2/dfi/validate.py
--rw-r--r--   0        0        0     2371 2023-07-06 09:33:05.506949 dfipy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 dfipy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      568 2023-08-07 09:49:34.555634 dfipy-2.0.0/LICENCE
+-rw-r--r--   0        0        0     1808 2023-08-07 09:49:34.555634 dfipy-2.0.0/README.md
+-rw-r--r--   0        0        0       99 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/__init__.py
+-rw-r--r--   0        0        0     1683 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/client.py
+-rw-r--r--   0        0        0     4913 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/connect.py
+-rw-r--r--   0        0        0     1320 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/models.py
+-rw-r--r--   0        0        0    13485 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/analyse.py
+-rw-r--r--   0        0        0     2285 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/delete.py
+-rw-r--r--   0        0        0    19814 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/get.py
+-rw-r--r--   0        0        0     5168 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/info.py
+-rw-r--r--   0        0        0     6033 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/ingest.py
+-rw-r--r--   0        0        0     8596 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/polygons.py
+-rw-r--r--   0        0        0     4813 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/services/show.py
+-rw-r--r--   0        0        0    13524 2023-08-07 09:49:34.555634 dfipy-2.0.0/dfi/validate.py
+-rw-r--r--   0        0        0     2393 2023-08-07 09:49:41.095737 dfipy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 dfipy-2.0.0/PKG-INFO
```

### Comparing `dfipy-1.0.2/LICENCE` & `dfipy-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.2/README.md` & `dfipy-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.2/dfi/analyse.py` & `dfipy-2.0.0/dfi/services/analyse.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import geopandas as gpd
 import h3.api.numpy_int as h3
 import pandas as pd
 from shapely.geometry import Polygon
 
 from dfi import models, validate
 from dfi.connect import Connect
-from dfi.get import Get
+from dfi.services.get import Get
 
 _logger = logging.getLogger(__name__)
 
 
 class Analyse:
     """
     Class with analytical methods to build use cases on top of the DFI's queries.
@@ -38,15 +38,15 @@
     dfi = Client(dfi_token, instance_name, namespace, base_url)
     dfi.analyse.records_in_hexagons(uid, resolution, period)
     ```
 
     Or access only the Analyse class directly:
     ```python
     from dfi.connect import Connect
-    from dfi.get import Analyse
+    from dfi.services.get import Analyse
 
     conn = dfi.Connect(api_token, namespace, instance_name, base_url)
     dfi_analyse = dfi.Analyse(conn)
 
     dfi_analyse.records_in_hexagons(uid, resolution, period)
     ```
     """
@@ -196,24 +196,20 @@
             time_resolution_min=time_resolution_min,
         )
 
     def add_heatmap_aggregation(
         self,
         df_records: pd.DataFrame,
         h3_resolution: int,
-        colorscale_column_name: str = "num_records",
-        colorscale_log_transform: bool = True,
     ) -> pd.DataFrame:
         """
         Aggregates the records by the H3 hexagons at the given resolution.
 
         :param df_records: Dataframe with the records we want to aggregate.
         :param h3_resolution: Uber's H3 resolution. Allowed numbers are > 1 and < 15.
-        :param colorscale_column_name: (not implemented) Name of the column with the colorscale for visualisation.
-        :param colorscale_log_transform: (not implemented) Log transform the colorscale.
 
         :returns: The given dataframe with extra `hex_id`, `num_records` and `color` columns.
 
         :example:
         ```python
         from dfi import Client
 
@@ -239,29 +235,25 @@
 
     def records_for_entity_id_with_heatmap_aggregation(
         self,
         entity_id: str,
         h3_resolution: int,
         time_interval: Optional[models.TimeInterval] = None,
         polygon: Optional[models.Polygon] = None,
-        colorscale_colum_name: str = "num_records",
-        colorscale_log_transform: bool = True,
     ) -> pd.DataFrame:
         """
         Aggregates the records by the H3 hexagons at the given resolution, from the parameters
         to a DFI query (entity_id, polygon, start_time, end_time)
 
         :param entity_id: unique identifier of a device we want to analyse.
         :param h3_resolution: Uber's H3 h3_resolution. Allowed numbers are > 1 and < 15.
         :param time_interval: Tuple of time bounds where (lower bound, upper bound).
         :param polygon:  List of vertices [[lon1, lat1], [lon2, lat2], ...] or a list of four
             floats representing the bounding box extremes as [lon_min, lat_min, lon_max, lat_max].
             Non valid input will raise an error.
-        :param colorscale_col:  Name of the column with the colorscale for visualisation.
-        :param colorscale_log_transform:  Log transform the colorscale.
 
         :returns: Returns the queried records dataframe with extra `hex_id`, `num_records` and `color` columns.
         :raises `DFIInputValueError`: If `time_interval` or `polygon` are ill-formed.
 
         :example:
         ```python
         from dfi import Client
@@ -293,20 +285,15 @@
                     "timestamp",
                     "hex_id",
                     "period_start",
                     "period end",
                 ]
             )
 
-        return self.add_heatmap_aggregation(
-            df_records,
-            h3_resolution=h3_resolution,
-            colorscale_colum_name=colorscale_colum_name,
-            colorscale_log_transform=colorscale_log_transform,
-        )
+        return self.add_heatmap_aggregation(df_records, h3_resolution=h3_resolution)
 
 
 def _aggregate_records(df_input: pd.DataFrame, hex_id: str) -> pd.DataFrame:
     return (
         df_input.groupby(hex_id)
         .agg(
             num_records=("entity_id", "count"),
```

### Comparing `dfipy-1.0.2/dfi/client.py` & `dfipy-2.0.0/dfi/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
 Class composition of all the other classes, to access the
 wrappers with syntactic sugar.
 """
-from dfi.analyse import Analyse
 from dfi.connect import Connect
-from dfi.get import Get
-from dfi.polygons import Polygons
-from dfi.show import Show
+from dfi.services.analyse import Analyse
+from dfi.services.delete import Delete
+from dfi.services.get import Get
+from dfi.services.info import Info
+from dfi.services.ingest import Ingest
+from dfi.services.polygons import Polygons
+from dfi.services.show import Show
 
 
 class Client:
     """
     Client class gathering all the classes and method in a single one. Facade of dfi.Connect.
 
     See documentation of dfi.Connect for its input values.
@@ -36,17 +39,20 @@
             api_token=api_token,
             instance_name=instance_name,
             namespace=namespace,
             base_url=base_url,
             query_timeout=query_timeout,
             progress_bar=progress_bar,
         )
-        self.get = Get(self.conn)
-        self.show = Show(self.conn)
         self.analyse = Analyse(self.conn)
+        self.delete = Delete(self.conn)
+        self.get = Get(self.conn)
+        self.info = Info(self.conn)
+        self.ingest = Ingest(self.conn)
         self.polygons = Polygons(self.conn)
+        self.show = Show(self.conn)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.conn!r})"
 
     def __str__(self) -> str:
         return f"""Instance of dfi.{self.__class__.__name__} composed with: {self.conn!s}"""
```

### Comparing `dfipy-1.0.2/dfi/connect.py` & `dfipy-2.0.0/dfi/connect.py`

 * *Files 21% similar despite different names*

```diff
@@ -108,7 +108,49 @@
             json=payload,
             stream=stream,
             params=params,
             timeout=self.query_timeout,
         )
         validate.response(response, url, headers, params)
         return response
+
+    def api_put(
+        self,
+        endpoint: str,
+        stream: bool = True,
+        params: Optional[dict] = None,
+        data: Optional[dict] = None,
+    ) -> requests.models.Response:
+        """Helper wrapping requests.put method"""
+        headers = self.streaming_headers
+        url = f"{self.base_url}/{endpoint}"
+        response = requests.put(
+            url,
+            headers=headers,
+            data=data,
+            stream=stream,
+            params=params,
+            timeout=self.query_timeout,
+        )
+        validate.response(response, url, headers, params)
+        return response
+
+    def api_delete(
+        self,
+        endpoint: str,
+        stream: bool = True,
+        params: Optional[dict] = None,
+        payload: Optional[dict] = None,
+    ) -> requests.models.Response:
+        """Helper wrapping requests.delete method"""
+        headers = self.streaming_headers
+        url = f"{self.base_url}/{endpoint}"
+        response = requests.delete(
+            url,
+            headers=headers,
+            json=payload,
+            stream=stream,
+            params=params,
+            timeout=self.query_timeout,
+        )
+        validate.response(response, url, headers, params)
+        return response
```

### Comparing `dfipy-1.0.2/dfi/get.py` & `dfipy-2.0.0/dfi/services/get.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 _logger = logging.getLogger(__name__)
 
 NUM_ATTEMPTS = 3
 
 
 class Get:
     """
-    Class responsible to call the HTTP API and submit queries.
+    Class responsible to call the HTTP API and submit queries to get data from DFI.
 
     It can be accessed via the a dfi.Client class instance or it must be instantiated
     with a dfi.Connect instance as argument.
 
     :param conn: Instance of a Connect with the credentials and namespace of the DFI connection.
     :example:
     Access via the Client class:
@@ -40,15 +40,15 @@
     dfi.get.entities(time_interval=[start_time, end_time])
     ```
 
     Or access only the Get class directly:
 
     ```python
     from dfi.connect import Connect
-    from dfi.get import Get
+    from dfi.service.get import Get
 
     conn = dfi.Connect(api_token, instance_name, namespace, base_url)
     dfi_get = dfi.Get(conn)
     dfi_get.entities(time_interval=[start_time, end_time])
     ```
     """
 
@@ -57,21 +57,14 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.conn!r})"
 
     def __str__(self) -> str:
         return f"""Instance of dfi.{self.__class__.__name__} composed with: {self.conn!s}"""
 
-    def api_version(self) -> str:
-        """
-        Returns the version of the Data Flow Index API.
-        """
-        with self.conn.api_get("version", stream=False, params=None) as response:
-            return response.text
-
     def records_count(
         self,
         entities: Optional[List[str]] = None,
         polygon: Optional[models.Polygon] = None,
         time_interval: Optional[models.TimeInterval] = None,
     ) -> int:
         """
@@ -350,15 +343,15 @@
             params = {"instance": self.conn.qualified_instance_name}
             if time_interval is not None:
                 params["startTime"], params["endTime"] = unpack_and_convert_time_interval(time_interval)
             min_lng, min_lat, max_lng, max_lat = polygon
             with self.conn.api_get(
                 f"bounding-box/{min_lng}/{min_lat}/{max_lng}/{max_lat}/entities", params=params, stream=True
             ) as response:
-                self._receive_entities(response)
+                return self._receive_entities(response)
 
     def _receive_entities(self, response: requests.models.Response) -> List[Any]:
         """
         Helper function to parse clients events as entities and optionally show the progress bar.
         """
         client = sseclient.SSEClient(response)
         results = []
```

### Comparing `dfipy-1.0.2/dfi/models.py` & `dfipy-2.0.0/dfi/models.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.2/dfi/show.py` & `dfipy-2.0.0/dfi/services/show.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 :::{attention}
 This module should be considered experimental and subject to change.
 :::
 """
 
 import logging
 from copy import deepcopy
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Union
 
 import geopandas as gpd
 import pandas as pd
 from keplergl import KeplerGl
 from shapely.geometry import Polygon
 
 from dfi import validate
 from dfi.connect import Connect
 from dfi.models import Polygon as ModelPolygons
-from dfi.polygons import Polygons
+from dfi.services.polygons import Polygons, from_bbox_to_polygon_list
 
 _logger = logging.getLogger(__name__)
 
 
 class Show:
     """
     Visualisation methods to build use case on top of the queries from DFI.
@@ -131,14 +131,7 @@
         if list_dfs is not None:
             for idx, df in enumerate(list_dfs):
                 kepler_data.update({f"df_{idx}": df.copy()})
 
         if config is None:
             return KeplerGl(data=deepcopy(kepler_data), height=map_height)
         return KeplerGl(data=deepcopy(kepler_data), height=map_height, config=config)
-
-
-def from_bbox_to_polygon_list(bounding_box: List[float]) -> Tuple[Tuple[float, float]]:
-    """Convert a bounding box, passed as a list `[min_lon, min_lat, max_lon, max_lat]` into a tuple of vertices."""
-    validate.bounding_box(bounding_box)
-    min_lon, min_lat, max_lon, max_lat = bounding_box
-    return ((max_lon, max_lat), (max_lon, min_lat), (min_lon, min_lat), (min_lon, max_lat), (max_lon, max_lat))
```

### Comparing `dfipy-1.0.2/dfi/validate.py` & `dfipy-2.0.0/dfi/validate.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,102 +10,223 @@
 validate.df_records(df_records)
 ```
 
 """
 import json
 import logging
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import pandas as pd
 import requests
 
 from dfi import models
 
 _logger = logging.getLogger(__name__)
 
 
-class DFIResponseError(Exception):
-    """Raised when an error propagated back from the HTTP API"""
+class DFIDataFrameColumnsNameError(Exception):
+    """Raised when the column names of a dataframe are not as expected"""
 
 
-class DFIResponseWarning(Warning):
-    """Raised when some exceptional case is propagated back from the HTTP API"""
+class DFIDataCSVConversionError(Exception):
+    """Raised when the user tries to ingest into DFI a csv that is wrongly formatted"""
 
 
-class DFIDataFrameColumnsNameError(Exception):
-    """Raised when the column names of a dataframe are not as expected"""
+class DFIDataJSONConversionError(Exception):
+    """Raised when the user tries to ingest into DFI a json that is wrongly formatted"""
+
+
+class DFIInputDataError(Exception):
+    """Raised when the user tries to ingest into DFI a piece of data wrongly formatted"""
 
 
 class DFIInputValueError(Exception):
     """Raised when the user passes a wrong input value to the DFI query"""
 
 
 class DFIInputValueOutOfBoundError(Exception):
     """Raised when the user passes a wrong input value to the DFI query"""
 
 
+class DFIResponseError(Exception):
+    """Raised when an error propagated back from the HTTP API"""
+
+
+class DFIResponseWarning(Warning):
+    """Raised when some exceptional case is propagated back from the HTTP API"""
+
+
+def bounding_box(list_bbox: Optional[List[float]]) -> None:
+    """
+    Check input list of coordinates correspond to a bounding box, with lon, lat within the range.
+
+    :param list_bbox: a bbox
+    :returns: `None`
+    :raises `DFIInputValueError`: If `polygon` is ill-formed.
+    :raises `DFIInputValueOutOfBoundError`: If not -180.0 < longitude <= 180.0 or not -90 < latitude <= 90.0.
+    """
+    if list_bbox is None:
+        return
+    if len(list_bbox) != 4:
+        raise DFIInputValueError(f"Input bounding box parameters must be a list of 4 floats. User passed {list_bbox}")
+    for value in list_bbox:
+        if not isinstance(value, float):
+            raise DFIInputValueError(f"Input value {value} of type {type(value)} must be a float.")
+
+    min_lng, min_lat, max_lng, max_lat = list_bbox
+
+    if not -180 < min_lng <= 180:
+        raise DFIInputValueOutOfBoundError(f"Input min longitude {min_lng} is out of range.")
+    if not -180 < max_lng <= 180:
+        raise DFIInputValueOutOfBoundError(f"Input max longitude {max_lng} is out of range.")
+    if not -90 < min_lat < 90:
+        raise DFIInputValueOutOfBoundError(f"Input min latitude {min_lat} is out of range.")
+    if not -90 < max_lat < 90:
+        raise DFIInputValueOutOfBoundError(f"Input max latitude {max_lat} is out of range.")
+
+
+def data(list_data: List[dict]) -> None:
+    """
+    Check that the input is a list of dict with correct keys.
+
+    :param list_data: a list of dictionaries with keys "coordinate", "time", "id", "payload".
+    :returns: `None`
+    :raises `DFIInputDataError`: if the input dictionaries do not have the correct keys.
+    :raises `DFIInputValueOutOfBoundError`: if the input coordinates are out of bound.
+
+    """
+    expected_keys = {"coordinate", "time", "id", "payload"}
+    for dict_data in list_data:
+        if not expected_keys.issubset(set(dict_data.keys())):
+            raise DFIInputDataError(f"Keys expected {expected_keys}. Found instead {set(dict_data.keys())}")
+        if not isinstance(dict_data["coordinate"], (list, tuple)):
+            raise DFIInputDataError(f"Coordinates passed are {dict_data['coordinate']}. Expecting a tuple or a list.")
+        if len(dict_data["coordinate"]) != 2:
+            raise DFIInputDataError(
+                f"Coordinates passed are {dict_data['coordinate']}. Expecting a tuple or a list with two elements."
+            )
+        lng, lat = dict_data["coordinate"]
+        if not -180 < lng <= 180:
+            raise DFIInputValueOutOfBoundError(f"Input max longitude {lng} is out of range.")
+        if not -90 < lat < 90:
+            raise DFIInputValueOutOfBoundError(f"Input min latitude {lat} is out of range.")
+
+
+def df_hexes(df_h3: pd.DataFrame) -> None:
+    """
+    Check the column names are correct.
+
+    :param df_h3: A dataframe with a `"hex_id"` column.
+    :returns: `None`
+    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
+        `["entity_id", "latitude", "longitude", "timestamp", "hex_id"]`
+    """
+    for col_name in ["entity_id", "latitude", "longitude", "timestamp", "hex_id"]:
+        if col_name not in df_h3.columns:
+            raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
+
+
+def df_hexes_heatmap(df_h3: pd.DataFrame) -> None:
+    """
+    Check the column names are correct.
+
+    :param df_h3: A dataframe with a `"hex_id"` column.
+    :returns: `None`
+    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
+        `["entity_id", "latitude", "longitude", "timestamp", "hex_id", "period_start", "period end"]`
+    """
+    for col_name in ["entity_id", "latitude", "longitude", "timestamp", "hex_id", "period_start", "period end"]:
+        if col_name not in df_h3.columns:
+            raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
+
+
 def df_records(df_rec: pd.DataFrame) -> None:
     """
     Check the column names are correct.
 
     :param h3_res: A dataframe of records
     :returns `None`:
     :raises `DFIDataFrameColumnsNameError`: If a column name is not in
         `["entity_id", "latitude", "longitude", "timestamp"]`
     """
     for col_name in ["entity_id", "latitude", "longitude", "timestamp"]:
         if col_name not in df_rec.columns:
             raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
 
 
+def entities(input_entities: Optional[List[str]]) -> None:
+    """
+    Validate a given list of entities is a list of strings.
+
+    :param `input_entities`: a list of entity ids
+    :returns: `None`
+    :raises `DFIInputValueError`: If `input_entities` is not a list of string or is empty or has duplicates.
+    """
+    if input_entities is None:
+        return
+    if not isinstance(input_entities, list):
+        raise DFIInputValueError(f"Entities must be a list of strings. Received {input_entities}")
+    if len(input_entities) == 0:
+        raise DFIInputValueError("Entities must be a list of strings. Received an empty list")
+    if len(set(input_entities)) < len(input_entities):
+        duplicates_found = set([x for x in input_entities if input_entities.count(x) > 1])
+        raise DFIInputValueError(f"Entities list must not contain duplicates. Duplicates found {duplicates_found}")
+
+
 def h3_resolution(h3_res: int) -> None:
     """
     check the input is within an acceptable range.
 
     :param `h3_res`: An H3 resolution
     :returns: `None`
     :raises `DFIInputValueOutOfBoundError`:  If not 1<= h3_res <= 15
     """
     if (h3_res < 1) or (h3_res > 15):
         raise DFIInputValueOutOfBoundError(
             f"Resolution is incorrect. It must be between 1 and 15. User passed {h3_res}"
         )
 
 
-def vertices_response(vert: Optional[models.Polygon], resp: requests.models.Response) -> None:
+def list_polygons_response(vert: Optional[models.Polygon], resp: requests.models.Response) -> None:
     """
     :param vert:
     :returns: `None`
     :raises `DFIResponseError`: If there was an error querying the DFI API.
 
     :::{TODO}
     Display error from API.
     :::
     """
     if vert is None:
-        msg = f"Polygon vertices can not be retrieved from the json response: {resp.json()}"
+        msg = f"Polygon list can not be retrieved from the json response: {resp.json()}"
         _logger.error(msg)
         raise DFIResponseError(msg)
 
 
-def list_polygons_response(vert: Optional[models.Polygon], resp: requests.models.Response) -> None:
+def polygon(poly: Optional[models.Polygon]) -> None:
     """
-    :param vert:
-    :returns: `None`
-    :raises `DFIResponseError`: If there was an error querying the DFI API.
+    Check input list of coordinates correspond to a list of vertices, or a bounding box.
 
-    :::{TODO}
-    Display error from API.
-    :::
+    :param poly: A list of vertices or bbox.
+    :returns `None`:
+    :raises `DFIInputValueError`: If `polygon` is ill-formed.
     """
-    if vert is None:
-        msg = f"Polygon list can not be retrieved from the json response: {resp.json()}"
-        _logger.error(msg)
-        raise DFIResponseError(msg)
+    if poly is None:
+        return
+    if not isinstance(poly, (list, tuple)):
+        raise DFIInputValueError(f"Polygon {poly} must be of type list or tuple.")
+    if len(poly) == 0:
+        raise DFIInputValueError(f"Given polygon {poly} is empty.")
+    if not isinstance(poly[0], (list, tuple, float)):
+        raise DFIInputValueError(f"Polygon {poly} must be a list of tuples or floats.")
+    if isinstance(poly[0], float):
+        bounding_box(poly)
+    if isinstance(poly[0], (list, tuple)):
+        vertices(poly)
 
 
 def response(
     resp: requests.models.Response,
     url: str,
     headers: dict,
     params: dict,
@@ -183,31 +304,29 @@
         raise DFIInputValueError(msg)
 
     if not start_time < end_time:
         msg = f"Start time {start_time} happened after than end time {end_time}."
         raise DFIInputValueError(msg)
 
 
-def entities(input_entities: Optional[List[str]]) -> None:
+def url_s3(url_object: Union[str, List[str]]) -> None:
     """
-    Validate a given list of entities is a list of strings.
+    Validate input S3 URL, which can be a string or a list of strings.
 
-    :param `input_entities`: a list of entity ids
+    :param url_object: - a string with an S3 URL or a list or S3 UR:.
     :returns: `None`
-    :raises `DFIInputValueError`: If `input_entities` is not a list of string or is empty or has duplicates.
+    :raises `DFIInputValueError`: if the types are not as expected.
     """
-    if input_entities is None:
-        return
-    if not isinstance(input_entities, list):
-        raise DFIInputValueError(f"Entities must be a list of strings. Received {input_entities}")
-    if len(input_entities) == 0:
-        raise DFIInputValueError("Entities must be a list of strings. Received an empty list")
-    if len(set(input_entities)) < len(input_entities):
-        duplicates_found = set([x for x in input_entities if input_entities.count(x) > 1])
-        raise DFIInputValueError(f"Entities list must not contain duplicates. Duplicates found {duplicates_found}")
+    msg = f"Given URL can be either a list of strings or a list. User passed {url_object}"
+    if not isinstance(url_object, (str, list)):
+        raise DFIInputValueError(msg)
+    if isinstance(url_object, list):
+        for url_item in url_object:
+            if not isinstance(url_item, str):
+                raise DFIInputValueError(msg)
 
 
 def vertices(input_vertices: Optional[List[List[float]]]) -> None:
     """
     Check input list of vertices correspond to a polygon.
     It does not check if the polygon is simple.
 
@@ -233,84 +352,21 @@
         if not -90 < lat < 90:
             raise DFIInputValueOutOfBoundError(f"Input  latitude {lat} is out of range.")
 
     if not input_vertices[0] == input_vertices[-1]:
         raise DFIInputValueError("First and last vertices are expected to be identical points.")
 
 
-def bounding_box(list_bbox: Optional[List[float]]) -> None:
-    """
-    Check input list of coordinates correspond to a bounding box, with lon, lat within the range.
-
-    :param list_bbox: a bbox
-    :returns: `None`
-    :raises `DFIInputValueError`: If `polygon` is ill-formed.
-    :raises `DFIInputValueOutOfBoundError`: If not -180.0 < longitude <= 180.0 or not -90 < latitude <= 90.0.
-    """
-    if list_bbox is None:
-        return
-    if len(list_bbox) != 4:
-        raise DFIInputValueError(f"Input bounding box parameters must be a list of 4 floats. User passed {list_bbox}")
-    for value in list_bbox:
-        if not isinstance(value, float):
-            raise DFIInputValueError(f"Input value {value} of type {type(value)} must be a float.")
-
-    min_lng, min_lat, max_lng, max_lat = list_bbox
-
-    if not -180 < min_lng <= 180:
-        raise DFIInputValueOutOfBoundError(f"Input min longitude {min_lng} is out of range.")
-    if not -180 < max_lng <= 180:
-        raise DFIInputValueOutOfBoundError(f"Input max longitude {max_lng} is out of range.")
-    if not -90 < min_lat < 90:
-        raise DFIInputValueOutOfBoundError(f"Input min latitude {min_lat} is out of range.")
-    if not -90 < max_lat < 90:
-        raise DFIInputValueOutOfBoundError(f"Input max latitude {max_lat} is out of range.")
-
-
-def polygon(poly: Optional[models.Polygon]) -> None:
-    """
-    Check input list of coordinates correspond to a list of vertices, or a bounding box.
-
-    :param poly: A list of vertices or bbox.
-    :returns `None`:
-    :raises `DFIInputValueError`: If `polygon` is ill-formed.
-    """
-    if poly is None:
-        return
-    if not isinstance(poly, (list, tuple)):
-        raise DFIInputValueError(f"Polygon {poly} must be of type list or tuple.")
-    if len(poly) == 0:
-        raise DFIInputValueError(f"Given polygon {poly} is empty.")
-    if not isinstance(poly[0], (list, tuple, float)):
-        raise DFIInputValueError(f"Polygon {poly} must be a list of tuples or floats.")
-    if isinstance(poly[0], float):
-        bounding_box(poly)
-    if isinstance(poly[0], (list, tuple)):
-        vertices(poly)
-
-
-def df_hexes_heatmap(df_h3: pd.DataFrame) -> None:
+def vertices_response(vert: Optional[models.Polygon], resp: requests.models.Response) -> None:
     """
-    Check the column names are correct.
-
-    :param df_h3: A dataframe with a `"hex_id"` column.
+    :param vert:
     :returns: `None`
-    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
-        `["entity_id", "latitude", "longitude", "timestamp", "hex_id", "period_start", "period end"]`
-    """
-    for col_name in ["entity_id", "latitude", "longitude", "timestamp", "hex_id", "period_start", "period end"]:
-        if col_name not in df_h3.columns:
-            raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
-
-
-def df_hexes(df_h3: pd.DataFrame) -> None:
-    """
-    Check the column names are correct.
+    :raises `DFIResponseError`: If there was an error querying the DFI API.
 
-    :param df_h3: A dataframe with a `"hex_id"` column.
-    :returns: `None`
-    :raises `DFIDataFrameColumnsNameError`: If a column name is not in
-        `["entity_id", "latitude", "longitude", "timestamp", "hex_id"]`
+    :::{TODO}
+    Display error from API.
+    :::
     """
-    for col_name in ["entity_id", "latitude", "longitude", "timestamp", "hex_id"]:
-        if col_name not in df_h3.columns:
-            raise DFIDataFrameColumnsNameError(f"Column name {col_name} expected in df_records but not found.")
+    if vert is None:
+        msg = f"Polygon vertices can not be retrieved from the json response: {resp.json()}"
+        _logger.error(msg)
+        raise DFIResponseError(msg)
```

### Comparing `dfipy-1.0.2/pyproject.toml` & `dfipy-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,58 +60,57 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "1.0.2"
+version = "2.0.0"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@generalsystem.com>",
   "Sebastiano Ferraris <sebastiano.ferraris@generalsystem.com>",
 ]
 readme = "README.md"
 homepage = "https://www.generalsystem.com/"
 repository = "https://github.com/thegeneralsystem/dfipy"
 documentation = "https://dfipy.docs.generalsystem.com/"
 include = ["LICENCE"]
 packages = [{ include = "dfi" }]
 
 [tool.poetry.dependencies]
-python = "^3.8.1"
+certifi = "^2023.07.22"
+geopandas = "^0.13.0"
 h3 = "^3.7.6"
+keplergl = "^0.3.2"
+numpy = "^1.24.3"
 pandas = "^2.0.1"
 pydeck = "^0.8.0"
+python = "^3.8.1"
 requests = "^2.30.0"
+setuptools = "^67.8.0"
 shapely = "^2.0.1"
 sseclient-py = "^1.7.2"
 tqdm = "^4.65.0"
-numpy = "^1.24.3"
-geopandas = "^0.13.0"
-keplergl = "^0.3.2"
-setuptools = "^67.8.0"
-
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
+coverage = "^7.2.5"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
+pylance = "^0.4.19"
 pylint = "^2.17.4"
 pytest = "^7.3.1"
-coverage = "^7.2.5"
-pylance = "^0.4.19"
 
 [tool.poetry.group.docs.dependencies]
 myst_parser = "^2.0.0"
 pydata-sphinx-theme = "^0.13.3"
 sphinx = "^7.0.1"
 sphinx-autodoc2 = "^0.4.2"
 sphinx-favicon = "^1.0.1"
 sphinxcontrib-napoleon = "^0.7"
 sphinx-copybutton = "^0.5.2"
 
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dfipy-1.0.2/PKG-INFO` & `dfipy-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 1.0.2
+Version: 2.0.0
 Summary: DFI api python wrapper
 Home-page: https://www.generalsystem.com/
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@generalsystem.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: certifi (>=2023.07.22,<2024.0.0)
 Requires-Dist: geopandas (>=0.13.0,<0.14.0)
 Requires-Dist: h3 (>=3.7.6,<4.0.0)
 Requires-Dist: keplergl (>=0.3.2,<0.4.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pydeck (>=0.8.0,<0.9.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
```

