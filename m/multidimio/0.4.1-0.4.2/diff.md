# Comparing `tmp/multidimio-0.4.1.tar.gz` & `tmp/multidimio-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidimio-0.4.1.tar", max compression
+gzip compressed data, was "multidimio-0.4.2.tar", max compression
```

## Comparing `multidimio-0.4.1.tar` & `multidimio-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    10203 2023-07-24 19:16:15.809080 multidimio-0.4.1/LICENSE
--rw-r--r--   0        0        0     6043 2023-07-24 19:16:15.809080 multidimio-0.4.1/README.md
--rw-r--r--   0        0        0     2806 2023-07-24 19:16:29.829316 multidimio-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      474 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/__init__.py
--rw-r--r--   0        0        0     2697 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/__main__.py
--rw-r--r--   0        0        0      127 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/__init__.py
--rw-r--r--   0        0        0    24779 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/accessor.py
--rw-r--r--   0        0        0     2322 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/convenience.py
--rw-r--r--   0        0        0     4451 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/api/io_utils.py
--rw-r--r--   0        0        0      105 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/commands/__init__.py
--rw-r--r--   0        0        0    12573 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/commands/segy.py
--rw-r--r--   0        0        0      529 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/constants.py
--rw-r--r--   0        0        0      141 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/__init__.py
--rw-r--r--   0        0        0      597 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/exceptions.py
--rw-r--r--   0        0        0     6510 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/mdio.py
--rw-r--r--   0        0        0    13393 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/converters/segy.py
--rw-r--r--   0        0        0      143 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/__init__.py
--rw-r--r--   0        0        0     3811 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/dimension.py
--rw-r--r--   0        0        0      268 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/exceptions.py
--rw-r--r--   0        0        0     3694 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/grid.py
--rw-r--r--   0        0        0     2917 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/indexing.py
--rw-r--r--   0        0        0     2727 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/serialization.py
--rw-r--r--   0        0        0      429 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/core/utils_write.py
--rw-r--r--   0        0        0     1646 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/py.typed
--rw-r--r--   0        0        0       44 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/__init__.py
--rw-r--r--   0        0        0      636 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/_standards_common.py
--rw-r--r--   0        0        0     9384 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/_standards_rev0.py
--rw-r--r--   0        0        0     8377 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/_workers.py
--rw-r--r--   0        0        0    11128 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/blocked_io.py
--rw-r--r--   0        0        0     2048 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/byte_utils.py
--rw-r--r--   0        0        0     9408 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/creation.py
--rw-r--r--   0        0        0     4856 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/ebcdic.py
--rw-r--r--   0        0        0     1946 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/exceptions.py
--rw-r--r--   0        0        0    10719 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/geometry.py
--rw-r--r--   0        0        0     2748 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/headers.py
--rw-r--r--   0        0        0     3561 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/headers_text.py
--rw-r--r--   0        0        0     1120 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/helpers_segy.py
--rw-r--r--   0        0        0     5785 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/ibm_float.py
--rw-r--r--   0        0        0     4916 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/parsers.py
--rw-r--r--   0        0        0     5170 2023-07-24 19:16:15.825080 multidimio-0.4.1/src/mdio/segy/utilities.py
--rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    10203 2023-08-07 17:32:52.684488 multidimio-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6043 2023-08-07 17:32:52.684488 multidimio-0.4.2/README.md
+-rw-r--r--   0        0        0     2806 2023-08-07 17:33:08.501453 multidimio-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/__init__.py
+-rw-r--r--   0        0        0     2697 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/__main__.py
+-rw-r--r--   0        0        0      127 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/api/__init__.py
+-rw-r--r--   0        0        0    24766 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/api/accessor.py
+-rw-r--r--   0        0        0     2322 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/api/convenience.py
+-rw-r--r--   0        0        0     4451 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/api/io_utils.py
+-rw-r--r--   0        0        0      105 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/commands/__init__.py
+-rw-r--r--   0        0        0    12573 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/commands/segy.py
+-rw-r--r--   0        0        0      529 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/constants.py
+-rw-r--r--   0        0        0      141 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/converters/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/converters/exceptions.py
+-rw-r--r--   0        0        0     6510 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/converters/mdio.py
+-rw-r--r--   0        0        0    15117 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/converters/segy.py
+-rw-r--r--   0        0        0      143 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/__init__.py
+-rw-r--r--   0        0        0     3811 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/dimension.py
+-rw-r--r--   0        0        0      268 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/exceptions.py
+-rw-r--r--   0        0        0     3694 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/grid.py
+-rw-r--r--   0        0        0     2917 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/indexing.py
+-rw-r--r--   0        0        0     2727 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/serialization.py
+-rw-r--r--   0        0        0      429 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/core/utils_write.py
+-rw-r--r--   0        0        0     1646 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/py.typed
+-rw-r--r--   0        0        0       44 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/__init__.py
+-rw-r--r--   0        0        0      636 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/_standards_common.py
+-rw-r--r--   0        0        0     9384 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/_standards_rev0.py
+-rw-r--r--   0        0        0     8377 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/_workers.py
+-rw-r--r--   0        0        0    11128 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/blocked_io.py
+-rw-r--r--   0        0        0     2048 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/byte_utils.py
+-rw-r--r--   0        0        0     9408 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/creation.py
+-rw-r--r--   0        0        0     4856 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/ebcdic.py
+-rw-r--r--   0        0        0     1946 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/exceptions.py
+-rw-r--r--   0        0        0    10719 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/geometry.py
+-rw-r--r--   0        0        0     2748 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/headers.py
+-rw-r--r--   0        0        0     3561 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/headers_text.py
+-rw-r--r--   0        0        0     1120 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/helpers_segy.py
+-rw-r--r--   0        0        0     5785 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/ibm_float.py
+-rw-r--r--   0        0        0     4916 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/parsers.py
+-rw-r--r--   0        0        0     5170 2023-08-07 17:32:52.700489 multidimio-0.4.2/src/mdio/segy/utilities.py
+-rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 multidimio-0.4.2/PKG-INFO
```

### Comparing `multidimio-0.4.1/LICENSE` & `multidimio-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/README.md` & `multidimio-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/pyproject.toml` & `multidimio-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multidimio"
-version = "0.4.1"
+version = "0.4.2"
 description = "Cloud-native, scalable, and user-friendly multi dimensional energy data!"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `multidimio-0.4.1/src/mdio/__main__.py` & `multidimio-0.4.2/src/mdio/__main__.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/api/accessor.py` & `multidimio-0.4.2/src/mdio/api/accessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
                     f"{mdio_dim.name} dimension does not have "
                     f"coordinate(s) {query_diff}"
                 )
                 raise ValueError(msg)
 
             sorter = mdio_dim.coords.argsort()
             dim_idx = np.searchsorted(mdio_dim, dim_query_coords, sorter=sorter)
-            dim_idx = dim_idx.astype("uint16")  # cast to minimize memory. max: 65,535
+            dim_idx = dim_idx.astype("uint32")  # cast max: 2,147,483,647
             dim_indices += (dim_idx,)
 
         return dim_indices if len(dim_indices) > 1 else dim_indices[0]
 
     def copy(
         self,
         dest_path_or_buffer: str,
```

### Comparing `multidimio-0.4.1/src/mdio/api/convenience.py` & `multidimio-0.4.2/src/mdio/api/convenience.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/api/io_utils.py` & `multidimio-0.4.2/src/mdio/api/io_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/commands/segy.py` & `multidimio-0.4.2/src/mdio/commands/segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/constants.py` & `multidimio-0.4.2/src/mdio/constants.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/converters/exceptions.py` & `multidimio-0.4.2/src/mdio/converters/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/converters/mdio.py` & `multidimio-0.4.2/src/mdio/converters/mdio.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/converters/segy.py` & `multidimio-0.4.2/src/mdio/converters/segy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Conversion from SEG-Y to MDIO."""
 
 
 from __future__ import annotations
 
+import logging
 from datetime import datetime
 from datetime import timezone
 from importlib import metadata
 from typing import Any
 from typing import Sequence
 
 import numpy as np
@@ -21,14 +22,16 @@
 from mdio.segy.byte_utils import Dtype
 from mdio.segy.helpers_segy import create_zarr_hierarchy
 from mdio.segy.parsers import parse_binary_header
 from mdio.segy.parsers import parse_text_header
 from mdio.segy.utilities import get_grid_plan
 
 
+logger = logging.getLogger(__name__)
+
 try:
     API_VERSION = metadata.version("multidimio")
 except metadata.PackageNotFoundError:
     API_VERSION = "unknown"
 
 BACKENDS = ["s3", "gcs", "gs", "az", "abfs"]
 
@@ -48,14 +51,58 @@
                 f"{list(Dtype.__members__.keys())}"
             )
             raise KeyError(msg) from exc
 
     return parsed_types
 
 
+def grid_density_qc(grid: Grid, num_traces: int) -> None:
+    """QC for sensible Grid density.
+
+    Basic qc of the grid to check density and provide warning/exception
+    when indexing is problematic to provide user with insights to the use.
+    If trace density on the specified grid is less than 50% a warning is
+    logged.  If denisty is less than 1% an exception is raised.
+
+    Args:
+        grid: The grid instance to check.
+        num_traces: Expected number of traces.
+
+    Raises:
+        GridTraceCountError: When the grid is too sparse.
+    """
+    grid_traces = np.prod(grid.shape[:-1], dtype=np.uint64)  # Exclude sample
+    dims = {k: v for k, v in zip(grid.dim_names, grid.shape)}  # noqa: B905
+
+    logger.debug(f"Dimensions: {dims}")
+    logger.debug(f"num_traces = {num_traces}")
+
+    # Extreme case where the grid is very sparse (usually user error)
+    if grid_traces > 10 * num_traces:
+        for dim_name in grid.dim_names:
+            dim_min = grid.get_min(dim_name)
+            dim_max = grid.get_max(dim_name)
+            logger.warning(f"{dim_name} min: {dim_min} max: {dim_max}")
+
+        msg = (
+            f"Grid shape: {grid.shape} but SEG-Y tracecount: {num_traces}. "
+            "This grid is very sparse and most likely user error with indexing."
+        )
+        raise GridTraceCountError(msg)
+
+    # Warning if we have above 50% sparsity.
+    if grid_traces > 2 * num_traces:
+        msg = (
+            f"Proposed ingestion grid is sparse. Ingestion grid: {dims}. "
+            f"SEG-Y trace count:{num_traces}, grid trace count: {grid_traces}."
+        )
+
+        logger.warning(msg)
+
+
 def segy_to_mdio(
     segy_path: str,
     mdio_path_or_buffer: str,
     index_bytes: Sequence[int],
     index_names: Sequence[str] | None = None,
     index_types: Sequence[str] | None = None,
     chunksize: Sequence[int] | None = None,
@@ -258,14 +305,17 @@
         binary_header=binary_header,
         return_headers=True,
         grid_overrides=grid_overrides,
     )
 
     # Make grid and build global live trace mask
     grid = Grid(dims=dimensions)
+
+    grid_density_qc(grid, num_traces)
+
     grid.build_map(index_headers)
 
     # Check grid validity by comparing trace numbers
     if np.sum(grid.live_mask) != num_traces:
         raise GridTraceCountError(np.sum(grid.live_mask), num_traces)
 
     zarr_root = create_zarr_hierarchy(
```

### Comparing `multidimio-0.4.1/src/mdio/core/dimension.py` & `multidimio-0.4.2/src/mdio/core/dimension.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/core/grid.py` & `multidimio-0.4.2/src/mdio/core/grid.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/core/indexing.py` & `multidimio-0.4.2/src/mdio/core/indexing.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/core/serialization.py` & `multidimio-0.4.2/src/mdio/core/serialization.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/exceptions.py` & `multidimio-0.4.2/src/mdio/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/_standards_common.py` & `multidimio-0.4.2/src/mdio/segy/_standards_common.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/_standards_rev0.py` & `multidimio-0.4.2/src/mdio/segy/_standards_rev0.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/_workers.py` & `multidimio-0.4.2/src/mdio/segy/_workers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/blocked_io.py` & `multidimio-0.4.2/src/mdio/segy/blocked_io.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/byte_utils.py` & `multidimio-0.4.2/src/mdio/segy/byte_utils.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/creation.py` & `multidimio-0.4.2/src/mdio/segy/creation.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/ebcdic.py` & `multidimio-0.4.2/src/mdio/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/exceptions.py` & `multidimio-0.4.2/src/mdio/segy/exceptions.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/geometry.py` & `multidimio-0.4.2/src/mdio/segy/geometry.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/headers.py` & `multidimio-0.4.2/src/mdio/segy/headers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/headers_text.py` & `multidimio-0.4.2/src/mdio/segy/headers_text.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/helpers_segy.py` & `multidimio-0.4.2/src/mdio/segy/helpers_segy.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/ibm_float.py` & `multidimio-0.4.2/src/mdio/segy/ibm_float.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/parsers.py` & `multidimio-0.4.2/src/mdio/segy/parsers.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/src/mdio/segy/utilities.py` & `multidimio-0.4.2/src/mdio/segy/utilities.py`

 * *Files identical despite different names*

### Comparing `multidimio-0.4.1/PKG-INFO` & `multidimio-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidimio
-Version: 0.4.1
+Version: 0.4.2
 Summary: Cloud-native, scalable, and user-friendly multi dimensional energy data!
 Home-page: https://mdio.dev
 License: Apache-2.0
 Keywords: mdio,multidimio,seismic,wind,data
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
```

