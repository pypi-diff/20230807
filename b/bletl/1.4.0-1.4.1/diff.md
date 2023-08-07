# Comparing `tmp/bletl-1.4.0.tar.gz` & `tmp/bletl-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bletl-1.4.0.tar", last modified: Thu Aug  3 11:26:33 2023, max compression
+gzip compressed data, was "bletl-1.4.1.tar", last modified: Mon Aug  7 08:05:45 2023, max compression
```

## Comparing `bletl-1.4.0.tar` & `bletl-1.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.965824 bletl-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34452 2023-08-03 11:13:45.000000 bletl-1.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 11:13:45.000000 bletl-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-03 11:26:33.965824 bletl-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-03 11:13:45.000000 bletl-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.957825 bletl-1.4.0/bletl/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/heuristics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.961825 bletl-1.4.0/bletl/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/parsing/bl1.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/parsing/blpro.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/splines.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-03 11:13:45.000000 bletl-1.4.0/bletl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.961825 bletl-1.4.0/bletl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 11:13:55.000000 bletl-1.4.0/bletl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 11:26:33.000000 bletl-1.4.0/bletl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-03 11:13:45.000000 bletl-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 11:26:33.965824 bletl-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-03 11:13:45.000000 bletl-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 11:26:33.965824 bletl-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-03 11:13:45.000000 bletl-1.4.0/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:05:45.548105 bletl-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34452 2023-08-07 07:52:24.000000 bletl-1.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 07:52:24.000000 bletl-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-07 08:05:45.548105 bletl-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-07 07:52:24.000000 bletl-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:05:45.544105 bletl-1.4.1/bletl/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/heuristics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:05:45.544105 bletl-1.4.1/bletl/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/parsing/bl1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22053 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/parsing/blpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/splines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-08-07 07:52:24.000000 bletl-1.4.1/bletl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:05:45.544105 bletl-1.4.1/bletl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-07 08:05:45.000000 bletl-1.4.1/bletl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-07 08:05:45.000000 bletl-1.4.1/bletl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 08:05:45.000000 bletl-1.4.1/bletl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 07:52:31.000000 bletl-1.4.1/bletl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-07 08:05:45.000000 bletl-1.4.1/bletl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-07 08:05:45.000000 bletl-1.4.1/bletl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-07 07:52:24.000000 bletl-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 08:05:45.548105 bletl-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-07 07:52:24.000000 bletl-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 08:05:45.548105 bletl-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-08-07 07:52:24.000000 bletl-1.4.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-07 07:52:24.000000 bletl-1.4.1/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-08-07 07:52:24.000000 bletl-1.4.1/tests/test_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-07 07:52:24.000000 bletl-1.4.1/tests/test_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-07 07:52:24.000000 bletl-1.4.1/tests/test_splines.py
```

### Comparing `bletl-1.4.0/LICENSE.md` & `bletl-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/PKG-INFO` & `bletl-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bletl
-Version: 1.4.0
+Version: 1.4.1
 Summary: Package for parsing and transforming BioLector raw data.
 Home-page: https://github.com/jubiotech/bletl
 Author: Michael Osthege
 Author-email: m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3.0
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `bletl-1.4.0/README.md` & `bletl-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/__init__.py` & `bletl-1.4.1/bletl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     InvalidLotNumberError,
     LotInformationError,
     LotInformationMismatch,
     LotInformationNotFound,
     NoMeasurementData,
 )
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
```

### Comparing `bletl-1.4.0/bletl/core.py` & `bletl-1.4.1/bletl/core.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/features.py` & `bletl-1.4.1/bletl/features.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/growth.py` & `bletl-1.4.1/bletl/growth.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/heuristics.py` & `bletl-1.4.1/bletl/heuristics.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/parsing/bl1.py` & `bletl-1.4.1/bletl/parsing/bl1.py`

 * *Files 5% similar despite different names*

```diff
@@ -192,16 +192,16 @@
         dpH: Optional[float] = None,
     ):
         headerlines, data = split_header_data(filepath)
 
         metadata = extract_metadata(headerlines)
         process_parameters = extract_process_parameters(headerlines)
         filtersets = extract_filtersets(headerlines)
-        comments = extract_comments(data)
         references = extract_references(data)
+        comments = extract_comments(data, references)
         measurements = extract_measurements(data)
 
         data = BLData(
             model=BioLectorModel.BL1,
             environment=extract_environment(data, process_parameters, comments),
             filtersets=filtersets,
             references=references,
@@ -373,24 +373,33 @@
         "shaking": float(headerlines[fs_start + 5].split(";")[13].strip()),
         "cycle_time": float(headerlines[fs_start + 6].split(";")[13].strip()),
         "exp_time": float(headerlines[fs_start + 7].split(";")[13].strip()),
     }
     return process_parameters
 
 
-def extract_comments(dfraw):
+def extract_comments(dfraw: pandas.DataFrame, references: pandas.DataFrame) -> pandas.DataFrame:
+    """This adds cycle numbers using timestamps from references."""
     ocol_ncol_type = [
         ("TIME [h]", "time", float),
         ("COMMENTS", "user_comment", str),
     ]
     df = utils.__to_typed_cols__(dfraw[dfraw["READING"] == "K"], ocol_ncol_type)
+
+    # Get the times when each cycle started
+    start_times = references.reset_index().drop_duplicates("cycle", keep="first").set_index("cycle").time
+    start_times.loc[1] = 0
+    # Add cycle numbers based on cycle start times and comment timestamps
+    df["cycle"] = [start_times[t > start_times].index[-1] for t in df["time"]]
+
     # TODO: automatically separate comments into user/sys
     df["sys_comment"] = None
     df.index = range(len(df))
-    return df
+    # Change column order
+    return df[["cycle", "time", "user_comment", "sys_comment"]]
 
 
 def extract_references(dfraw):
     dfref = dfraw[dfraw["READING"] == "R"].copy()
     ocol_ncol_type = [
         ("cycle", "cycle", int),
         ("TIME [h]", "time", float),
```

### Comparing `bletl-1.4.0/bletl/parsing/blpro.py` & `bletl-1.4.1/bletl/parsing/blpro.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import io
 import logging
 import os
 import pathlib
 import re
 import warnings
 import xml.etree.ElementTree
-from typing import Optional, Union
+from typing import Any, DefaultDict, Dict, List, Optional, Tuple, Union
 
 import numpy
 import pandas
 
 from .. import utils
 from ..types import (
     BioLectorModel,
     BLData,
     BLDParser,
     FilterTimeSeries,
     FluidicsSource,
+    IncompatibleFileError,
     InvalidLotNumberError,
 )
 
 logger = logging.getLogger("blpro")
 
 
 _MF_WELL_NUMC_TO_ID = {
@@ -124,34 +125,37 @@
 def _parse_datalines(datalines) -> pandas.DataFrame:
     dfraw = pandas.read_csv(
         io.StringIO("".join(datalines)), sep=";", low_memory=False, converters={"Filterset": str}
     )
     return dfraw
 
 
-def parse_metadata_data(fp):
+def parse_metadata_data(fp) -> Tuple[Dict[str, Any], pandas.DataFrame]:
     with open(fp, "r", encoding="utf-8") as f:
         lines = f.readlines()
 
-    metadata = collections.defaultdict(dict)
-    datalines = collections.defaultdict(list)
+    metadata: DefaultDict[str, Any] = collections.defaultdict(dict)
     section = None
-    data_start = None
+    data_start: Optional[int] = None
 
     for l, line in enumerate(lines):
         if line.startswith("="):
             # any section header encountered
             section = line.strip().strip("=").strip()
             if not data_start and section == "data":
                 data_start = l + 1
+        elif section is None:
+            raise IncompatibleFileError("No metadata section header before first setting.")
         elif line.startswith("["):
             # register the value
             key, value = line.split("]")
             key = key.strip("[")
             metadata[section][key] = value.strip()
+    if data_start is None:
+        raise IncompatibleFileError("Section header 'data' not found.")
 
     # standardize the metadata keys
     metadata["date_start"] = datetime.datetime.strptime(
         metadata["process"]["start_date_time"], "%Y-%m-%d, %H:%M:%S"
     )
     if "end_process" in metadata and "end_date_time" in metadata["end_process"]:
         metadata["date_end"] = datetime.datetime.strptime(
@@ -191,15 +195,15 @@
             else:
                 defect_lines.append(data_start + l + 1)
         dfraw = _parse_datalines(filtered_datalines).drop_duplicates(keep="first")
         logger.warning(
             f"{fp} contains defects in lines {defect_lines}. Be extra skeptical about the parsed results."
         )
 
-    return metadata, dfraw[list(dfraw.columns)[:-1]]
+    return dict(metadata), dfraw[list(dfraw.columns)[:-1]]
 
 
 def standardize(df):
     if "time" in df.columns:
         df["time"] = df["time"] / 3600
     return df
 
@@ -254,14 +258,15 @@
         (None, "emission2", float),
     ]
     return utils.__to_typed_cols__(df, ocol_ncol_type)
 
 
 def extract_comments(dfraw):
     ocol_ncol_type = [
+        ("Cycle", "cycle", int),
         ("Time", "time", float),
         ("User_Comment", "user_comment", str),
         ("Sys_Comment", "sys_comment", str),
     ]
     df = utils.__to_typed_cols__(dfraw[dfraw["Type"] == "C"], ocol_ncol_type)
     return standardize(df)
 
@@ -311,14 +316,30 @@
     if ndrop:
         cdrop = df_M[mask]["Cycle"].to_list()
         warnings.warn(
             f"Dropped {ndrop} measurement rows from cycles {cdrop} because they have REFOVERLD.", UserWarning
         )
     df_M = df_M[~mask]
 
+    # Drop filtersets with non-monotonically increasing time
+    drop_idxs = []
+    for idx, fsblock in df_M.groupby(["Cycle", "Filterset"]):
+        t = fsblock["Time"].astype(int).to_numpy()
+        if any(t[1:] < t[:-1]):
+            drop_idxs.append(idx)
+    ndrop = len(drop_idxs)
+    if ndrop:
+        for dropC, dropF in drop_idxs:
+            mask = numpy.logical_and(df_M["Cycle"] == dropC, df_M["Filterset"] == dropF)
+            df_M = df_M[~mask]
+            warnings.warn(
+                f"Dropped cycle {dropC} filterset {dropF} because of non-monotonically increasing time values.",
+                UserWarning,
+            )
+
     # Convert to the expected data types
     df = utils.__to_typed_cols__(df_M, ocol_ncol_type)
     df = df.set_index(["filterset", "cycle", "well"])
     return standardize(df)
 
 
 def extract_environment(dfraw):
```

### Comparing `bletl-1.4.0/bletl/splines.py` & `bletl-1.4.1/bletl/splines.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/types.py` & `bletl-1.4.1/bletl/types.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl/utils.py` & `bletl-1.4.1/bletl/utils.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/bletl.egg-info/PKG-INFO` & `bletl-1.4.1/bletl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bletl
-Version: 1.4.0
+Version: 1.4.1
 Summary: Package for parsing and transforming BioLector raw data.
 Home-page: https://github.com/jubiotech/bletl
 Author: Michael Osthege
 Author-email: m.osthege@fz-juelich.de
 License: GNU Affero General Public License v3.0
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `bletl-1.4.0/bletl.egg-info/SOURCES.txt` & `bletl-1.4.1/bletl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/setup.py` & `bletl-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/tests/test_core.py` & `bletl-1.4.1/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,14 +460,25 @@
         return
 
     def test_parse_file_with_defects(self):
         # this file has some broken & duplicate data line lines 25857-25877
         bletl.parse(pathlib.Path(dir_testfiles, "BLPro", "line_duplication.csv"))
         pass
 
+    @pytest.mark.filterwarnings("ignore:cycle 2 filterset 02")
+    def test_drop_non_monotonically_increasing_time_filtersets(self):
+        """This happens when line/block defects accidentally result in a parseable CSV."""
+        with pytest.warns(UserWarning, match="cycle 2 filterset 02"):
+            bldata = bletl.parse(dir_testfiles / "BLPro" / "non_monotonic_time.csv")
+            assert len(bldata["BS5"].time) == 4
+            assert len(bldata["pH"].time) == 3
+            assert 2 not in bldata["pH"].time.index
+            assert len(bldata["DO"].time) == 4
+        pass
+
     def test_refoverld_issue12(self):
         with pytest.warns(UserWarning, match=r"cycles \[269, 636\].*REFOVERLD"):
             bldata = bletl.parse(dir_testfiles / "BLPro" / "issue12.csv")
         for fs, n in zip(["BS3", "DO", "pH"], [682, 684, 684]):
             t, y = bldata.get_timeseries(fs, "A01")
             assert len(t) == n
             assert len(y) == n
```

### Comparing `bletl-1.4.0/tests/test_features.py` & `bletl-1.4.1/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/tests/test_growth.py` & `bletl-1.4.1/tests/test_growth.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/tests/test_heuristics.py` & `bletl-1.4.1/tests/test_heuristics.py`

 * *Files identical despite different names*

### Comparing `bletl-1.4.0/tests/test_splines.py` & `bletl-1.4.1/tests/test_splines.py`

 * *Files identical despite different names*

