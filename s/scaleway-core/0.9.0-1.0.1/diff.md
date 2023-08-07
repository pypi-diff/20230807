# Comparing `tmp/scaleway_core-0.9.0.tar.gz` & `tmp/scaleway_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway_core-0.9.0.tar", max compression
+gzip compressed data, was "scaleway_core-1.0.1.tar", max compression
```

## Comparing `scaleway_core-0.9.0.tar` & `scaleway_core-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       29 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/README.md
--rw-r--r--   0        0        0     1138 2023-03-08 16:40:56.922549 scaleway_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/__init__.py
--rw-r--r--   0        0        0     4443 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/api.py
--rw-r--r--   0        0        0      981 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/__init__.py
--rw-r--r--   0        0        0     1468 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/money.py
--rw-r--r--   0        0        0      188 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/region.py
--rw-r--r--   0        0        0      950 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/scwfile.py
--rw-r--r--   0        0        0     1304 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/serviceinfo.py
--rw-r--r--   0        0        0     2186 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/timeseries.py
--rw-r--r--   0        0        0      444 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/bridge/zone.py
--rw-r--r--   0        0        0     3669 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/client.py
--rw-r--r--   0        0        0      670 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/__init__.py
--rw-r--r--   0        0        0      774 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/env.py
--rw-r--r--   0        0        0      351 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/file.py
--rw-r--r--   0        0        0     6312 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/profile/profile.py
--rw-r--r--   0        0        0        0 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/py.typed
--rw-r--r--   0        0        0      770 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/__init__.py
--rw-r--r--   0        0        0     2119 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/fetch_all_pages.py
--rw-r--r--   0        0        0      600 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/project_or_organization_id.py
--rw-r--r--   0        0        0    50787 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/random_name.py
--rw-r--r--   0        0        0     1092 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/resolve_one_of.py
--rw-r--r--   0        0        0      111 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/strenum.py
--rw-r--r--   0        0        0      508 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/validate_path_param.py
--rw-r--r--   0        0        0     3532 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/utils/waiter.py
--rw-r--r--   0        0        0        0 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/validations/__init__.py
--rw-r--r--   0        0        0      998 2023-03-08 16:40:36.918432 scaleway_core-0.9.0/scaleway_core/validations/string_validation.py
--rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 scaleway_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/README.md
+-rw-r--r--   0        0        0     1138 2023-08-07 09:35:52.187467 scaleway_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/__init__.py
+-rw-r--r--   0        0        0     4445 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/api.py
+-rw-r--r--   0        0        0     1133 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/__init__.py
+-rw-r--r--   0        0        0     1468 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/money.py
+-rw-r--r--   0        0        0      188 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/region.py
+-rw-r--r--   0        0        0      950 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/scwfile.py
+-rw-r--r--   0        0        0     1304 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/serviceinfo.py
+-rw-r--r--   0        0        0     2186 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/timeseries.py
+-rw-r--r--   0        0        0      444 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/bridge/zone.py
+-rw-r--r--   0        0        0     3669 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/client.py
+-rw-r--r--   0        0        0      670 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/profile/__init__.py
+-rw-r--r--   0        0        0      810 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/profile/env.py
+-rw-r--r--   0        0        0      351 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/profile/file.py
+-rw-r--r--   0        0        0     7002 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/profile/profile.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/py.typed
+-rw-r--r--   0        0        0      770 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/__init__.py
+-rw-r--r--   0        0        0     2119 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/fetch_all_pages.py
+-rw-r--r--   0        0        0      600 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/project_or_organization_id.py
+-rw-r--r--   0        0        0    50787 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/random_name.py
+-rw-r--r--   0        0        0     1092 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/resolve_one_of.py
+-rw-r--r--   0        0        0      111 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/strenum.py
+-rw-r--r--   0        0        0      508 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/validate_path_param.py
+-rw-r--r--   0        0        0     3532 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/utils/waiter.py
+-rw-r--r--   0        0        0        0 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/validations/__init__.py
+-rw-r--r--   0        0        0      998 2023-08-07 09:35:29.060034 scaleway_core-1.0.1/scaleway_core/validations/string_validation.py
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 scaleway_core-1.0.1/PKG-INFO
```

### Comparing `scaleway_core-0.9.0/pyproject.toml` & `scaleway_core-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway-core"
-version = "0.9.0"
+version = "1.0.1"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
```

### Comparing `scaleway_core-0.9.0/scaleway_core/api.py` & `scaleway_core-1.0.1/scaleway_core/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
 class API:
     def __init__(self, client: Client, *, bypass_validation: bool = False):
         if not bypass_validation:
             client.validate()
 
         self.client = client
-        self._log = logging.getLogger(__name__)
+        self._log = logging.getLogger("scaleway")
 
     def _request(
         self,
         method: str,
         path: str,
         params: Params = {},
         headers: Dict[str, str] = {},
```

### Comparing `scaleway_core-0.9.0/scaleway_core/bridge/__init__.py` & `scaleway_core-1.0.1/scaleway_core/bridge/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from .serviceinfo import ServiceInfo
 from .serviceinfo import unmarshal_ServiceInfo
 from .serviceinfo import marshal_ServiceInfo
 
 from .timeseries import TimeSeriesPoint
 from .timeseries import TimeSeries
 from .timeseries import unmarshal_TimeSeries
+from .timeseries import marshal_TimeSeries
+from .timeseries import unmarshal_TimeSeriesPoint
 from .timeseries import marshal_TimeSeriesPoint
 
 __all__ = [
     "Money",
     "unmarshal_Money",
     "marshal_Money",
     "Region",
@@ -33,9 +35,11 @@
     "marshal_ScwFile",
     "ServiceInfo",
     "unmarshal_ServiceInfo",
     "marshal_ServiceInfo",
     "TimeSeriesPoint",
     "TimeSeries",
     "unmarshal_TimeSeries",
+    "marshal_TimeSeries",
+    "unmarshal_TimeSeriesPoint",
     "marshal_TimeSeriesPoint",
 ]
```

### Comparing `scaleway_core-0.9.0/scaleway_core/bridge/money.py` & `scaleway_core-1.0.1/scaleway_core/bridge/money.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/bridge/scwfile.py` & `scaleway_core-1.0.1/scaleway_core/bridge/scwfile.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/bridge/serviceinfo.py` & `scaleway_core-1.0.1/scaleway_core/bridge/serviceinfo.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/bridge/timeseries.py` & `scaleway_core-1.0.1/scaleway_core/bridge/timeseries.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/client.py` & `scaleway_core-1.0.1/scaleway_core/client.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/profile/__init__.py` & `scaleway_core-1.0.1/scaleway_core/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/profile/env.py` & `scaleway_core-1.0.1/scaleway_core/profile/env.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ENV_KEY_SCW_CONFIG_PATH = "SCW_CONFIG_PATH"
+ENV_KEY_SCW_PROFILE = "SCW_PROFILE"
 ENV_KEY_SCW_ACCESS_KEY = "SCW_ACCESS_KEY"
 ENV_KEY_SCW_SECRET_KEY = "SCW_SECRET_KEY"  # nosec B105
 ENV_KEY_SCW_API_URL = "SCW_API_URL"
 ENV_KEY_SCW_DEFAULT_ORGANIZATION_ID = "SCW_DEFAULT_ORGANIZATION_ID"
 ENV_KEY_SCW_DEFAULT_PROJECT_ID = "SCW_DEFAULT_PROJECT_ID"
 ENV_KEY_SCW_DEFAULT_REGION = "SCW_DEFAULT_REGION"
 ENV_KEY_SCW_DEFAULT_ZONE = "SCW_DEFAULT_ZONE"
```

### Comparing `scaleway_core-0.9.0/scaleway_core/profile/profile.py` & `scaleway_core-1.0.1/scaleway_core/profile/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 import os
 from dataclasses import dataclass
 from typing import Optional, Type, TypeVar
+import sys
 
 import yaml
-
 from scaleway_core import __version__
 from scaleway_core.profile.file import CONFIG_PROPERTIES_TO_PROFILE
 
-from .env import ENV_KEY_SCW_CONFIG_PATH, ENV_VARIABLES_TO_PROFILE
+from .env import ENV_KEY_SCW_CONFIG_PATH, ENV_KEY_SCW_PROFILE, ENV_VARIABLES_TO_PROFILE
 
 
 @dataclass
 class ProfileDefaults:
     default_organization_id: Optional[str] = None
     """
     Your organization ID is the identifier of your account inside Scaleway infrastructure.
@@ -92,23 +92,25 @@
         for field in dataclasses.fields(Profile):
             current_value = getattr(self, field.name)
 
             if current_value is None:
                 setattr(self, field.name, getattr(other, field.name))
 
     @classmethod
-    def from_env(cls: Type[ProfileSelf]) -> ProfileSelf:
+    def from_env(cls: Type[ProfileSelf], force_none: bool = False) -> ProfileSelf:
         """
         Loads profile from environment variables.
         """
         profile = cls()
         for env_variable, profile_property in ENV_VARIABLES_TO_PROFILE.items():
             value = os.environ.get(env_variable)
             if value is not None:
                 setattr(profile, profile_property, value)
+            elif force_none:
+                setattr(profile, profile_property, None)
 
         return profile
 
     @classmethod
     def get_default_config_directory(cls) -> str:
         xdg_config_path = os.environ.get("XDG_CONFIG_HOME")
         if xdg_config_path is not None and xdg_config_path != "":
@@ -128,28 +130,31 @@
         return os.path.join(Profile.get_default_config_directory(), "config.yaml")
 
     @classmethod
     def from_config_file(
         cls: Type[ProfileSelf],
         filepath: Optional[str] = None,
         profile_name: Optional[str] = "default",
+        force_none: bool = False,
     ) -> ProfileSelf:
         filepath = cls.get_default_config_file_path(filepath)
 
         with open(filepath, "r") as f:
             config = yaml.safe_load(f)
 
             if type(config) is not dict:
                 raise ValueError("Invalid config file")
 
             profile = cls()
             for file_property, profile_property in CONFIG_PROPERTIES_TO_PROFILE.items():
                 value = config.get(file_property)
                 if value is not None:
                     setattr(profile, profile_property, value)
+                elif force_none:
+                    setattr(profile, profile_property, None)
 
             if profile_name is not None and profile_name != "default":
                 has_profile = (
                     "profiles" in config
                     and type(config["profiles"]) is dict
                     and profile_name in config["profiles"]
                 )
@@ -165,32 +170,40 @@
                 for (
                     file_property,
                     profile_property,
                 ) in CONFIG_PROPERTIES_TO_PROFILE.items():
                     value = overrides.get(file_property)
                     if value is not None:
                         setattr(profile, profile_property, value)
+                    elif force_none:
+                        setattr(profile, profile_property, None)
 
             return profile
 
     @classmethod
     def from_config_file_and_env(
         cls: Type[ProfileSelf],
         filepath: Optional[str] = None,
-        profile_name: Optional[str] = "default",
+        profile_name: Optional[str] = os.environ.get(ENV_KEY_SCW_PROFILE, "default"),
     ) -> ProfileSelf:
         """
         Loads profile from a config file and environment variables.
 
         Environment variables override config file.
           - If config file is not found, the profile is still loaded from environment variables.
           - If you want it to throw an error in case of missing or invalid config file, use `Profile.from_config_file` and `Profile.from_env` instead.
         """
-        profile = cls.from_env()
 
+        has_config_profile = False
         try:
-            a = cls.from_config_file(filepath, profile_name)
-            profile.merge(a)
+            config_profile = cls.from_config_file(filepath, profile_name)
+            has_config_profile = True
         except Exception as e:
-            print(e)
+            logging.getLogger("scaleway").warning(
+                f"Could not load profile from config file: {e}"
+            )
+
+        env_profile = cls.from_env(force_none=has_config_profile)
+        if has_config_profile:
+            env_profile.merge(config_profile)
 
-        return profile
+        return env_profile
```

### Comparing `scaleway_core-0.9.0/scaleway_core/utils/__init__.py` & `scaleway_core-1.0.1/scaleway_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/utils/fetch_all_pages.py` & `scaleway_core-1.0.1/scaleway_core/utils/fetch_all_pages.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/utils/project_or_organization_id.py` & `scaleway_core-1.0.1/scaleway_core/utils/project_or_organization_id.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/utils/random_name.py` & `scaleway_core-1.0.1/scaleway_core/utils/random_name.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/utils/resolve_one_of.py` & `scaleway_core-1.0.1/scaleway_core/utils/resolve_one_of.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/utils/waiter.py` & `scaleway_core-1.0.1/scaleway_core/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/scaleway_core/validations/string_validation.py` & `scaleway_core-1.0.1/scaleway_core/validations/string_validation.py`

 * *Files identical despite different names*

### Comparing `scaleway_core-0.9.0/PKG-INFO` & `scaleway_core-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway-core
-Version: 0.9.0
+Version: 1.0.1
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -13,22 +13,18 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Scaleway Python SDK - Core
```

