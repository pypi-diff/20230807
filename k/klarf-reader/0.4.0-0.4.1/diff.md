# Comparing `tmp/klarf-reader-0.4.0.tar.gz` & `tmp/klarf-reader-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.4.0.tar", last modified: Fri Aug  4 12:03:48 2023, max compression
+gzip compressed data, was "klarf-reader-0.4.1.tar", last modified: Mon Aug  7 11:20:19 2023, max compression
```

## Comparing `klarf-reader-0.4.0.tar` & `klarf-reader-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.640182 klarf-reader-0.4.0/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-08-04 12:03:48.639187 klarf-reader-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.592837 klarf-reader-0.4.0/klarf_reader/
--rw-rw-rw-   0        0        0     1218 2023-07-27 09:09:59.000000 klarf-reader-0.4.0/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.620850 klarf-reader-0.4.0/klarf_reader/models/
--rw-rw-rw-   0        0        0     2559 2023-07-27 09:12:12.000000 klarf-reader-0.4.0/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.624847 klarf-reader-0.4.0/klarf_reader/readers/
--rw-rw-rw-   0        0        0    14566 2023-08-04 12:01:40.000000 klarf-reader-0.4.0/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.628602 klarf-reader-0.4.0/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.4.0/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.616227 klarf-reader-0.4.0/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-08-04 12:03:48.000000 klarf-reader-0.4.0/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-08-04 12:03:48.000000 klarf-reader-0.4.0/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 12:03:48.000000 klarf-reader-0.4.0/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-04 12:03:48.000000 klarf-reader-0.4.0/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-04 12:03:48.000000 klarf-reader-0.4.0/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 12:03:48.641182 klarf-reader-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-08-04 12:03:23.000000 klarf-reader-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 12:03:48.633933 klarf-reader-0.4.0/tests/
--rw-rw-rw-   0        0        0     4720 2023-08-04 11:42:04.000000 klarf-reader-0.4.0/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.906060 klarf-reader-0.4.1/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-08-07 11:20:19.902900 klarf-reader-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.863757 klarf-reader-0.4.1/klarf_reader/
+-rw-rw-rw-   0        0        0     1522 2023-08-07 10:02:48.000000 klarf-reader-0.4.1/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.888852 klarf-reader-0.4.1/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2635 2023-08-07 10:00:30.000000 klarf-reader-0.4.1/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.891780 klarf-reader-0.4.1/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    14918 2023-08-07 09:59:59.000000 klarf-reader-0.4.1/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.894781 klarf-reader-0.4.1/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.4.1/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.883310 klarf-reader-0.4.1/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-08-07 11:20:19.000000 klarf-reader-0.4.1/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-08-07 11:20:19.000000 klarf-reader-0.4.1/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 11:20:19.000000 klarf-reader-0.4.1/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-07 11:20:19.000000 klarf-reader-0.4.1/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-07 11:20:19.000000 klarf-reader-0.4.1/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-07 11:20:19.906560 klarf-reader-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-08-07 11:18:57.000000 klarf-reader-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 11:20:19.897781 klarf-reader-0.4.1/tests/
+-rw-rw-rw-   0        0        0     5382 2023-08-07 10:04:01.000000 klarf-reader-0.4.1/tests/test_klarf.py
```

### Comparing `klarf-reader-0.4.0/LICENSE.txt` & `klarf-reader-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.4.0/PKG-INFO` & `klarf-reader-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.4.0
+Version: 0.4.1
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.4.0.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.4.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.4.0/README.md` & `klarf-reader-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.4.0/klarf_reader/models/klarf_content.py` & `klarf-reader-0.4.1/klarf_reader/models/klarf_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Tuple
+from typing import Any, Dict, Generator, List, Tuple, Union
 from dataclasses import dataclass, field
 
 
 @dataclass
 class SetupId:
     name: str
     date: str
@@ -78,15 +78,17 @@
 
 @dataclass
 class Wafer:
     id: str
     slot: int
     die_origin: DieOrigin
     sample_center_location: SampleCenterLocation
-    defects: List[Defect] = field(default_factory=lambda: [])
+    defects: Union[List[Defect], Generator[Defect, Any, None]] = field(
+        default_factory=lambda: []
+    )
     tests: List[Test] = field(default_factory=lambda: [])
     custom_attribute: Dict[str, any] = None
     summary: Summary = None
 
 
 @dataclass
 class InspectionStationId:
```

### Comparing `klarf-reader-0.4.0/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.4.1/klarf_reader/readers/klarf_file_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # MODULES
 import re
 import os
 from pathlib import Path
-from typing import List, Tuple
+from typing import Dict, Generator, List, Tuple
 
 # MODELS
 from ..models.klarf_content import (
     Defect,
     DieOrigin,
     DiePitch,
     InspectionStationId,
@@ -18,49 +18,60 @@
     Test,
     Wafer,
 )
 
 ACCEPTED_KLARF_VERSIONS = [1.1, 1.2]
 
 
+def _get_raw_content(klarf: Path):
+    with open(klarf, "r") as f:
+        for line in f.readlines():
+            yield line
+
+
 def readKlarf(
     klarf: Path,
     custom_columns_wafer: List[str] = None,
     custom_columns_defect: List[str] = None,
     parse_summary: bool = True,
-) -> Tuple[KlarfContent, List[str]]:
+    defects_as_generator: bool = False,
+) -> Tuple[KlarfContent, Generator[str, None, None],]:
     """this function open, read and parse a klarf file
 
     Args:
         klarf (Path): the path of the klarf file
 
     Returns:
         KlarfContent: the content of the klarf as a dataclass
     """
 
     if not os.path.exists(klarf):
         raise Exception(f"{klarf=} does not exists")
 
-    with open(klarf, "r") as f:
-        raw_content = f.readlines()
+    raw_content = _get_raw_content(klarf)
 
-    return convert_raw_to_klarf_content(
-        raw_content=raw_content,
-        custom_columns_wafer=custom_columns_wafer,
-        custom_columns_defect=custom_columns_defect,
-        parse_summary=parse_summary,
+    return (
+        convert_raw_to_klarf_content(
+            raw_content=_get_raw_content(klarf),
+            custom_columns_wafer=custom_columns_wafer,
+            custom_columns_defect=custom_columns_defect,
+            parse_summary=parse_summary,
+            defects_as_generator=defects_as_generator,
+        ),
+        raw_content,
     )
 
 
 def convert_raw_to_klarf_content(
-    raw_content: List[str],
+    raw_content: Generator[str, None, None],
     custom_columns_wafer: List[str] = None,
     custom_columns_defect: List[str] = None,
     parse_summary: bool = True,
-) -> Tuple[KlarfContent, List[str]]:
+    defects_as_generator: bool = False,
+) -> KlarfContent:
 
     RAW_DEFECT_COLUMNS = [
         "DEFECTID",
         "XREL",
         "YREL",
         "XINDEX",
         "YINDEX",
@@ -311,15 +322,17 @@
 
                 wafers.append(
                     Wafer(
                         id=wafer_id,
                         slot=slot,
                         die_origin=die_origin,
                         sample_center_location=sample_center_location,
-                        defects=defects,
+                        defects=(defect for defect in defects)
+                        if defects_as_generator
+                        else defects,
                         tests=tests.copy(),
                         custom_attribute=custom_columns_wafer_dict,
                     )
                 )
 
                 tests.clear()
 
@@ -360,34 +373,31 @@
                 y = int(sample_test_plan_value[1])
                 sample_plan_test_y.append(y)
             if line.rstrip().endswith(";"):
                 next_line_has_sample_test_plan = False
                 skip_next_sample_test_plan = True
             continue
 
-    return (
-        KlarfContent(
-            file_version=file_version,
-            file_timestamp=file_timestamp,
-            inspection_station_id=inspection_station_id,
-            sample_type=sample_type,
-            result_timestamp=result_timestamp,
-            lot_id=lot_id,
-            device_id=device_id,
-            sample_size=sample_size,
-            step_id=step_id,
-            sample_orientation_mark_type=sample_orientation_mark_type,
-            orientation_mark_location=orientation_mark_location,
-            die_pitch=die_pitch,
-            setup_id=setup_id,
-            has_sample_test_plan=has_sample_test_plan,
-            sample_plan_test=SamplePlanTest(x=sample_plan_test_x, y=sample_plan_test_y),
-            wafers=wafers,
-        ),
-        raw_content,
+    return KlarfContent(
+        file_version=file_version,
+        file_timestamp=file_timestamp,
+        inspection_station_id=inspection_station_id,
+        sample_type=sample_type,
+        result_timestamp=result_timestamp,
+        lot_id=lot_id,
+        device_id=device_id,
+        sample_size=sample_size,
+        step_id=step_id,
+        sample_orientation_mark_type=sample_orientation_mark_type,
+        orientation_mark_location=orientation_mark_location,
+        die_pitch=die_pitch,
+        setup_id=setup_id,
+        has_sample_test_plan=has_sample_test_plan,
+        sample_plan_test=SamplePlanTest(x=sample_plan_test_x, y=sample_plan_test_y),
+        wafers=wafers,
     )
 
 
 def convert_coordinates(
     die_pitch: DiePitch,
     sample_center_location: SampleCenterLocation,
     xrel: float,
```

### Comparing `klarf-reader-0.4.0/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.4.1/klarf_reader/utils/klarf_convert.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.4.0/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.4.1/klarf_reader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.4.0
+Version: 0.4.1
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.4.0.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.4.1.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.4.0/setup.py` & `klarf-reader-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.4.0"
+version = "0.4.1"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.4.0/tests/test_klarf.py` & `klarf-reader-0.4.1/tests/test_klarf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,15 @@
 from tests.utils import *
 
 
 ASSETS_PATH: Path = Path(__file__).parent / "assets"
 ASSETS_SAVED_PATH: Path = ASSETS_PATH / "saved"
 
 
-class TestKlarf(unittest.TestCase):
-    def setUp(self) -> None:
-        self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
-        self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
-        self.path_klarf_1_1_multi_wafers = ASSETS_PATH / "KLARF_1_1.000"
-
+class _TestKlarfReader(unittest.TestCase):
     def assertListOfDictEqual(self, first: list[dict], second: list[dict]):
         self.assertEqual(len(first), len(second))
         for index, item in enumerate(first):
             if isinstance(item, dict):
                 self.assertNestedDictEqual(item, second[index])
             else:
                 self.assertEqual(item, second[index])
@@ -42,14 +37,25 @@
             if isinstance(value, (list, tuple)):
                 self.assertListOfDictEqual(value, second_value)
             elif isinstance(value, dict):
                 self.assertNestedDictEqual(value, second_value)
             else:
                 self.assertEqual(value, second_value)
 
+
+class TestKlarf(_TestKlarfReader):
+    def setUp(self) -> None:
+        self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
+        self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
+        self.path_klarf_1_1_multi_wafers = ASSETS_PATH / "KLARF_1_1.000"
+        self.path_klarf_1_1_single_wafer = ASSETS_PATH / "KLARF_1_1_SINGLE.001"
+        self.path_klarf_1_2_large_single_wafer = (
+            ASSETS_PATH / "CB8_SI_90_OA_1483573.001"
+        )
+
     @load_expected_data(saved_path=ASSETS_SAVED_PATH)
     def test_klarf_single_wafer(self, expected_data, saved_path) -> None:
         # When
         content = Klarf.load_from_file(filepath=self.path_klarf_single_wafer)
         content_dict = asdict(content)
 
         save_as_json(
@@ -72,45 +78,56 @@
         content = Klarf.load_from_file(
             filepath=self.path_klarf_single_wafer,
             custom_columns_wafer=custom_columns_lot,
             custom_columns_defect=custom_columns_defects,
         )
         content_dict = asdict(content)
 
-        save_as_json(
-            saved_path,
-            dict=content_dict,
-        )
+        save_as_json(saved_path, dict=content_dict)
 
         # Then
         self.assertNestedDictEqual(content_dict, expected_data)
 
     def test_klarf_single_wafer_with_raw_content(self) -> None:
         # Given
         expected_raw_content_length = 13356
 
         # When
         _, raw_content = Klarf.load_from_file_with_raw_content(
             filepath=self.path_klarf_single_wafer
         )
 
         # Then
-        self.assertEqual(len(raw_content), expected_raw_content_length)
+        self.assertEqual(len(list(raw_content)), expected_raw_content_length)
 
     @load_expected_data(saved_path=ASSETS_SAVED_PATH)
     def test_klarf_1_1_multi_wafers(self, expected_data, saved_path) -> None:
         # When
         content = Klarf.load_from_file(filepath=self.path_klarf_1_1_multi_wafers)
         content_dict = asdict(content)
 
         save_as_json(
             saved_path,
             dict=content_dict,
         )
 
+        # Then
+        self.assertNestedDictEqual(content_dict, expected_data)
+
+    @load_expected_data(saved_path=ASSETS_SAVED_PATH)
+    def test_klarf_1_1_single_wafer(self, expected_data, saved_path) -> None:
+        # When
+        content = Klarf.load_from_file(filepath=self.path_klarf_1_1_single_wafer)
+        content_dict = asdict(content)
+
+        save_as_json(
+            saved_path,
+            dict=content_dict,
+        )
+
         # Then
         self.assertNestedDictEqual(content_dict, expected_data)
 
     @load_expected_data(saved_path=ASSETS_SAVED_PATH)
     def test_klarf_multi_wafers(self, expected_data, saved_path) -> None:
         # When
         content = Klarf.load_from_file(filepath=self.path_klarf_multi_wafers)
```

