# Comparing `tmp/konbinine-0.1.4.tar.gz` & `tmp/konbinine-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konbinine-0.1.4.tar", last modified: Mon Jul 24 10:12:24 2023, max compression
+gzip compressed data, was "konbinine-0.1.5.tar", last modified: Mon Aug  7 08:50:52 2023, max compression
```

## Comparing `konbinine-0.1.4.tar` & `konbinine-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 10:12:24.949967 konbinine-0.1.4/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.4/LICENSE
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-07-24 10:12:24.949967 konbinine-0.1.4/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     2128 2023-07-24 10:10:35.000000 konbinine-0.1.4/README.md
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 10:12:24.949967 konbinine-0.1.4/konbinine/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    27357 2023-07-24 10:11:47.000000 konbinine-0.1.4/konbinine/__init__.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.4/konbinine/enums.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.4/konbinine/exceptions.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.4/konbinine/logs.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     7084 2023-07-24 08:53:23.000000 konbinine-0.1.4/konbinine/models.py
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      487 2023-06-29 09:15:35.000000 konbinine-0.1.4/konbinine/utils.py
-drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-07-24 10:12:24.949967 konbinine-0.1.4/konbinine.egg-info/
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/PKG-INFO
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      382 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/SOURCES.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/dependency_links.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/requires.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-07-24 10:12:24.000000 konbinine-0.1.4/konbinine.egg-info/top_level.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.4/konbinine.egg-info/zip-safe
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1268 2023-07-24 09:56:01.000000 konbinine-0.1.4/pyproject.toml
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.4/requirements.txt
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-07-24 10:12:24.949967 konbinine-0.1.4/setup.cfg
--rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.4/setup.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-07 08:50:52.824005 konbinine-0.1.5/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1066 2023-06-29 09:15:35.000000 konbinine-0.1.5/LICENSE
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-08-07 08:50:52.824005 konbinine-0.1.5/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     2128 2023-07-24 10:10:35.000000 konbinine-0.1.5/README.md
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-07 08:50:52.814005 konbinine-0.1.5/konbinine/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)    29922 2023-08-07 08:45:43.000000 konbinine-0.1.5/konbinine/__init__.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      873 2023-06-29 09:15:35.000000 konbinine-0.1.5/konbinine/enums.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      392 2023-07-03 01:33:22.000000 konbinine-0.1.5/konbinine/exceptions.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      365 2023-08-07 08:14:30.000000 konbinine-0.1.5/konbinine/fields.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      145 2023-07-03 01:33:22.000000 konbinine-0.1.5/konbinine/logs.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     7844 2023-08-07 08:45:31.000000 konbinine-0.1.5/konbinine/models.py
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1828 2023-08-07 08:07:50.000000 konbinine-0.1.5/konbinine/utils.py
+drwxr-xr-x   0 hueyyeng  (1000) hueyyeng  (1000)        0 2023-08-07 08:50:52.824005 konbinine-0.1.5/konbinine.egg-info/
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     4450 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/PKG-INFO
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)      402 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/SOURCES.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/dependency_links.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/requires.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       10 2023-08-07 08:50:52.000000 konbinine-0.1.5/konbinine.egg-info/top_level.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)        1 2023-07-24 09:52:07.000000 konbinine-0.1.5/konbinine.egg-info/zip-safe
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1268 2023-07-24 09:56:01.000000 konbinine-0.1.5/pyproject.toml
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       37 2023-07-07 02:46:56.000000 konbinine-0.1.5/requirements.txt
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)     1058 2023-08-07 08:50:52.824005 konbinine-0.1.5/setup.cfg
+-rw-r--r--   0 hueyyeng  (1000) hueyyeng  (1000)       38 2023-07-24 09:47:46.000000 konbinine-0.1.5/setup.py
```

### Comparing `konbinine-0.1.4/LICENSE` & `konbinine-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.4/PKG-INFO` & `konbinine-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.4
+Version: 0.1.5
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
```

### Comparing `konbinine-0.1.4/README.md` & `konbinine-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.4/konbinine/__init__.py` & `konbinine-0.1.5/konbinine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 import calendar
 import datetime
 import logging
 import os
 from typing import List, Optional, Set, Union
 
 import shotgun_api3
 from urllib3.exceptions import ProtocolError
 
 from konbinine.enums import SgEntity, SgHumanUserStatus
 from konbinine.exceptions import MissingValueError
+from konbinine.fields import (
+    HUMANUSER_FIELDS,
+    PROJECT_FIELDS,
+)
 from konbinine.logs import KonbiniAdapter
-from konbinine.models import SgBooking, SgHumanUser, SgTimeLog
+from konbinine.models import (
+    SgBooking,
+    SgHumanUser,
+    SgProject,
+    SgTimeLog,
+)
 from konbinine.utils import SG_DATE_FORMAT
 
 logger = KonbiniAdapter(logging.getLogger(__name__), {})
 logger.setLevel(logging.ERROR)
 
 
 class Konbini:
@@ -89,14 +98,101 @@
         list
             The list of fields belonging to the entity type
 
         """
         fields = self.sg.schema_field_read(entity_type=entity)
         return list(fields.keys())
 
+    def get_sg_projects(
+            self,
+            project_id: Optional[int] = None,
+            custom_fields: Optional[List[str]] = None,
+    ) -> List[SgProject]:
+        """Get SG Projects
+
+        Parameters
+        ----------
+        project_id : int
+            ShotGrid Project ID. Default None which retrieve all Projects
+        custom_fields : list[str]
+            List of custom fields
+
+        Returns
+        -------
+        list of SgProject
+            List of SgProject or empty list if no results from ShotGrid
+
+        """
+        filters = []
+        if project_id:
+            filters = [
+                [
+                    "id",
+                    "is",
+                    project_id
+                ]
+            ]
+
+        fields = PROJECT_FIELDS
+        if custom_fields:
+            fields = custom_fields
+
+        _projects: List[dict] = self.sg.find(SgEntity.PROJECT, filters, fields)
+        if not _projects:
+            return []
+
+        projects = []
+        for project in _projects:
+            sg_project = SgProject.from_dict(project)
+            projects.append(sg_project)
+
+        return projects
+
+    def update_sg_project(self, data: SgProject) -> bool:
+        """Update SG Project
+
+        Parameters
+        ----------
+        data : SgProject
+            The SgProject data for update
+
+        Returns
+        -------
+        bool
+            True if update successfully
+
+        """
+        if not isinstance(data, SgProject):
+            raise Exception("Data must be instance of SgProject!")
+
+        if not data.id:
+            raise Exception("No SgProject ID found!")
+
+        is_updated = True
+        data_ = data.to_dict()
+
+        # Project start and end date is read only (only can be modified using Project Planning app on SG Web)
+        data_.pop("start_date", None)
+        data_.pop("end_date", None)
+        data_.pop("duration", None)
+        data_.pop("updated_at", None)
+
+        try:
+            self.sg.update(
+                entity_type=SgEntity.PROJECT,
+                entity_id=data.id,
+                data=data_,
+            )
+            logger.info(f"Update SgProject {data.id} successful")
+        except shotgun_api3.ShotgunError as e:
+            logger.error(f"Error updating SgProject {data.id}: {e}")
+            is_updated = False
+
+        return is_updated
+
     def get_sg_humanusers(
             self,
             humanuser_id: Optional[int] = None,
             custom_fields: Optional[List[str]] = None,
     ) -> List[SgHumanUser]:
         """Get SG HumanUsers
 
@@ -119,19 +215,15 @@
                 [
                     "id",
                     "is",
                     humanuser_id
                 ]
             ]
 
-        fields = [
-            "name",
-            "projects",
-            "groups",
-        ]
+        fields = HUMANUSER_FIELDS
         if custom_fields:
             fields = custom_fields
 
         _users: List[dict] = self.sg.find(SgEntity.HUMANUSER, filters, fields)
         if not _users:
             return []
 
@@ -163,18 +255,15 @@
             [
                 "sg_status_list",
                 "is",
                 SgHumanUserStatus.ACTIVE,
             ]
         ]
 
-        fields = [
-            "name",
-            "groups",
-        ]
+        fields = HUMANUSER_FIELDS
         if custom_fields:
             fields = custom_fields
 
         _users: List[dict] = self.sg.find(SgEntity.HUMANUSER, filters, fields)
         if not _users:
             return []
 
@@ -248,20 +337,26 @@
         if not isinstance(data, SgHumanUser):
             raise Exception("Data must be instance of SgHumanUser!")
 
         if not data.id:
             raise Exception("No SgHumanUser ID found!")
 
         is_updated = True
+        data_ = data.to_dict()
+
+        # Requires Autodesk Account Portal to update the following fields
+        data_.pop("email", None)
+        data_.pop("firstname", None)
+        data_.pop("lastname", None)
 
         try:
             self.sg.update(
                 entity_type=SgEntity.HUMANUSER,
                 entity_id=data.id,
-                data=data.to_dict(),
+                data=data_,
             )
             logger.info(f"Update HumanUser {data.id} successful")
         except shotgun_api3.ShotgunError as e:
             logger.error(f"Error updating HumanUser {data.id}: {e}")
             is_updated = False
 
         return is_updated
```

### Comparing `konbinine-0.1.4/konbinine/enums.py` & `konbinine-0.1.5/konbinine/enums.py`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.4/konbinine/models.py` & `konbinine-0.1.5/konbinine/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import datetime
 import inspect
 from dataclasses import asdict, dataclass, field
 from typing import Any, Dict, List, Optional
 
 from konbinine.enums import SgEntity
-from konbinine.exceptions import InvalidSgDateFormatException
-from konbinine.utils import SG_DATE_FORMAT, validate_sg_date_format
+from konbinine.exceptions import (
+    InvalidSgDateFormatException,
+)
+from konbinine.utils import (
+    get_current_utc_dt,
+    SG_DATE_FORMAT,
+    validate_sg_date_format,
+)
 
 # TODO: Use Python 3.10+ kw_only but that is another headache for maintenance...
 
 
 @dataclass
 class SgIdMixin:
     id: int = 0
@@ -61,20 +67,34 @@
     type: str = SgEntity.NOTE
 
 
 @dataclass
 class SgProject(SgIdMixin, SgBaseModel):
     name: str = ""
     type: str = SgEntity.PROJECT
+    archived: bool = False
+    code: Optional[str] = None
+    sg_description: Optional[str] = None
+    sg_status: Optional[str] = None
+    sg_type: Optional[str] = None
+    start_date: Optional[str] = None  # Date uses YYYY-MM-DD format
+    end_date: Optional[str] = None
+    updated_at: Optional[datetime.datetime] = None  # Example 2023-08-07T06:29:35Z
+    image: Optional[str] = None
+    duration: Optional[int] = None  # Number of days
+
+    def validate_stale_data(self) -> bool:
+        current_dt = get_current_utc_dt()
+        return self.updated_at > current_dt
 
 
 @dataclass
 class _SgPipelineStep(SgBaseModel):
     code: str  # The nice name (e.g. Model)
-    short_name: str  # Self explanatory (e.g. MOD)
+    short_name: str  # Self-explanatory (e.g. MOD)
     type: str = SgEntity.STEP
 
 
 @dataclass
 class SgPipelineStep(SgIdMixin, _SgPipelineStep):
     pass
 
@@ -200,16 +220,22 @@
 @dataclass
 class SgPlaylist(SgIdMixin, _SgPlaylist):
     pass
 
 
 @dataclass
 class _SgHumanUser(SgBaseModel):
+    login: str
     name: str = ""
+    firstname: str = ""
+    lastname: str = ""
+    email: str = ""
+    file_access: bool = False
     type: str = SgEntity.HUMANUSER
+    image: Optional[str] = None
     projects: Optional[List[dict]] = None
     groups: Optional[List[dict]] = None
 
     def to_dict(self) -> Dict[str, Any]:
         dict_ = {
             k: v for k, v in asdict(self).items() if v
         }
```

### Comparing `konbinine-0.1.4/konbinine.egg-info/PKG-INFO` & `konbinine-0.1.5/konbinine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konbinine
-Version: 0.1.4
+Version: 0.1.5
 Summary: Opinionated Autodesk Shotgun/ShotGrid API Wrapper.
 Home-page: https://github.com/hueyyeng/konbini
 Author: Huey Yeng
 Author-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 Maintainer: Huey Yeng
 Maintainer-email: Huey Yeng <huey.yeng.mmu@gmail.com>
 License: MIT License
```

### Comparing `konbinine-0.1.4/pyproject.toml` & `konbinine-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konbinine-0.1.4/setup.cfg` & `konbinine-0.1.5/setup.cfg`

 * *Files identical despite different names*

