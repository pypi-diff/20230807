# Comparing `tmp/vnac-0.1.1.tar.gz` & `tmp/vnac-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnac-0.1.1.tar", max compression
+gzip compressed data, was "vnac-0.1.2.tar", max compression
```

## Comparing `vnac-0.1.1.tar` & `vnac-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      878 2023-08-04 08:27:23.581636 vnac-0.1.1/README.md
--rw-r--r--   0        0        0      961 2023-08-04 08:30:08.983707 vnac-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 02:08:52.463150 vnac-0.1.1/vnac/__init__.py
--rw-r--r--   0        0        0     5585 2023-08-04 06:58:41.733549 vnac-0.1.1/vnac/corrector.py
--rw-r--r--   0        0        0     1433 2023-08-04 06:31:11.542491 vnac-0.1.1/vnac/schemas.py
--rw-r--r--   0        0        0       96 2023-08-02 02:08:25.035092 vnac-0.1.1/vnac/utils.py
--rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 vnac-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      878 2023-08-04 08:27:23.581636 vnac-0.1.2/README.md
+-rw-r--r--   0        0        0      941 2023-08-07 01:27:50.787849 vnac-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 02:08:52.463150 vnac-0.1.2/vnac/__init__.py
+-rw-r--r--   0        0        0     5590 2023-08-07 01:07:19.853997 vnac-0.1.2/vnac/corrector.py
+-rw-r--r--   0        0        0     1280 2023-08-07 01:20:21.771201 vnac-0.1.2/vnac/schemas.py
+-rw-r--r--   0        0        0       96 2023-08-02 02:08:25.035092 vnac-0.1.2/vnac/utils.py
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 vnac-0.1.2/PKG-INFO
```

### Comparing `vnac-0.1.1/README.md` & `vnac-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vnac-0.1.1/pyproject.toml` & `vnac-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vnac"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Ngô Trần Ngọc Sơn <ntns1607@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/jasonntn/VNAddressCorrector"
 keywords = ["Vietnam", "division", "address", "locality"]
 classifiers = [
     'Natural Language :: Vietnamese',
@@ -15,15 +15,14 @@
     'Programming Language :: Python :: 3 :: Only',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Development Status :: 4 - Beta',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = "^2.1.1"
 vietnam-provinces = "^0.5.0"
 rapidfuzz = "^3.1.2"
 python-rapidjson = "^1.10"
 loguru = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `vnac-0.1.1/vnac/corrector.py` & `vnac-0.1.2/vnac/corrector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import re
 from typing import List, Tuple, Union
 
 import rapidjson
 from loguru import logger
 from rapidfuzz import fuzz, process
 from rapidfuzz.distance import Indel
@@ -82,15 +83,15 @@
                 logger.debug("Corrected: {} -> {}", region, corrected)
 
         return match, corrected
 
     def correct(self, address: Union[Address, str]) -> Address:
         if isinstance(address, str):
             address = Address.from_str(address)
-        corrected_address = address.model_copy(deep=True)
+        corrected_address = copy.deepcopy(address)
 
         if address.province:
             match_province, corrected_province = self.correct_region(address.province.name, self.provinces.keys())
             if corrected_province:
                 corrected_address.province.name = corrected_province
             if match_province:
                 corrected_address.province.code = self.provinces[match_province]
```

### Comparing `vnac-0.1.1/vnac/schemas.py` & `vnac-0.1.2/vnac/schemas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 import re
-from typing import Optional
-
-from pydantic import BaseModel, field_validator
+from dataclasses import dataclass
 
 from vnac.utils import clean_str
 
 
-class Division(BaseModel):
-    name: str
-    code: Optional[str] = None
-
-    @field_validator("name", mode="before")
-    @classmethod
-    def clean(cls, v):
-        return clean_str(v)
+@dataclass
+class Division:
+    name: str = None
+    code: str = None
 
 
-class Address(BaseModel):
-    country: Optional[Division] = None
-    province: Optional[Division] = None
-    district: Optional[Division] = None
-    ward: Optional[Division] = None
-    street: Optional[Division] = None
+@dataclass
+class Address:
+    country: Division = None
+    province: Division = None
+    district: Division = None
+    ward: Division = None
+    street: Division = None
 
     @classmethod
     def from_str(cls, s: str) -> "Address":
         """Create Address instance from string
 
         Args:
             s (str): address string
 
         Returns:
             Address: address instance
         """
         parts = clean_str(s).rsplit(",", 3)
-        match = re.findall("(việt\s*nam)", parts[-1], re.I)
-        country = Division(name=match[0]) if bool(match) else None
-        province = Division(name=parts[-1])
-        district = Division(name=parts[-2]) if len(parts) > 1 else None
-        ward = Division(name=parts[-3]) if len(parts) > 2 else None
-        street = Division(name=parts[-4]) if len(parts) > 3 else None
+        match = re.findall("(việt\\s*nam)", parts[-1], re.I)
+        country = Division(name=clean_str(match[0])) if bool(match) else None
+        province = Division(name=clean_str(parts[-1]))
+        district = Division(name=clean_str(parts[-2])) if len(parts) > 1 else None
+        ward = Division(name=clean_str(parts[-3])) if len(parts) > 2 else None
+        street = Division(name=clean_str(parts[-4])) if len(parts) > 3 else None
         return cls(country=country, province=province, district=district, ward=ward, street=street)
 
     def __str__(self) -> str:
         return ", ".join([i.name for i in [self.street, self.ward, self.district, self.province, self.country] if i])
```

### Comparing `vnac-0.1.1/PKG-INFO` & `vnac-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnac
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/jasonntn/VNAddressCorrector
 Keywords: Vietnam,division,address,locality
 Author: Ngô Trần Ngọc Sơn
 Author-email: ntns1607@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Localization
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: python-rapidjson (>=1.10,<2.0)
 Requires-Dist: rapidfuzz (>=3.1.2,<4.0.0)
 Requires-Dist: vietnam-provinces (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/jasonntn/VNAddressCorrector
 Description-Content-Type: text/markdown
 
 # VNAddressCorrector
```

