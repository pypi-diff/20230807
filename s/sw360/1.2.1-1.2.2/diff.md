# Comparing `tmp/sw360-1.2.1.tar.gz` & `tmp/sw360-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw360-1.2.1.tar", max compression
+gzip compressed data, was "sw360-1.2.2.tar", max compression
```

## Comparing `sw360-1.2.1.tar` & `sw360-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1127 2023-01-05 07:13:32.836394 sw360-1.2.1/License.md
--rw-r--r--   0        0        0     1200 2023-01-05 07:35:03.757741 sw360-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3038 2023-01-05 07:13:14.148210 sw360-1.2.1/Readme.md
--rw-r--r--   0        0        0      714 2019-04-08 11:15:46.185749 sw360-1.2.1/sw360/.editorconfig
--rw-r--r--   0        0        0      498 2022-12-26 08:44:04.736291 sw360-1.2.1/sw360/__init__.py
--rw-r--r--   0        0        0     9602 2023-01-05 07:16:15.346317 sw360-1.2.1/sw360/attachments.py
--rw-r--r--   0        0        0     1578 2022-12-26 08:44:04.744290 sw360-1.2.1/sw360/clearing.py
--rw-r--r--   0        0        0     9812 2022-12-26 08:44:04.748290 sw360-1.2.1/sw360/components.py
--rw-r--r--   0        0        0     4466 2022-12-26 08:44:04.753290 sw360-1.2.1/sw360/license.py
--rw-r--r--   0        0        0    18612 2022-12-26 08:44:04.759290 sw360-1.2.1/sw360/project.py
--rw-r--r--   0        0        0     8459 2022-12-26 08:44:04.765291 sw360-1.2.1/sw360/releases.py
--rw-r--r--   0        0        0     7005 2022-12-26 08:44:04.770295 sw360-1.2.1/sw360/sw360_api.py
--rw-r--r--   0        0        0     1229 2022-12-26 08:44:04.774296 sw360-1.2.1/sw360/sw360error.py
--rw-r--r--   0        0        0     4763 2022-12-26 08:44:04.778313 sw360-1.2.1/sw360/sw360oauth2.py
--rw-r--r--   0        0        0     3492 2022-12-26 08:44:04.784294 sw360-1.2.1/sw360/vendor.py
--rw-r--r--   0        0        0     1416 2022-12-26 08:44:04.788321 sw360-1.2.1/sw360/vulnerabilities.py
--rw-r--r--   0        0        0     3721 1970-01-01 00:00:00.000000 sw360-1.2.1/setup.py
--rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 sw360-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1221 2023-05-27 09:40:39.889958 sw360-1.2.2/License.md
+drwxr-xr-x   0        0        0        0 2023-05-27 09:26:46.746551 sw360-1.2.2/LICENSES/
+-rw-r--r--   0        0        0     1324 2023-08-07 20:52:18.840914 sw360-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3562 2023-05-27 15:38:47.328694 sw360-1.2.2/Readme.md
+-rw-r--r--   0        0        0      793 2023-05-27 09:32:04.067520 sw360-1.2.2/sw360/.editorconfig
+-rw-r--r--   0        0        0      505 2023-08-07 20:51:56.585640 sw360-1.2.2/sw360/__init__.py
+-rw-r--r--   0        0        0     9707 2023-08-07 20:14:05.496276 sw360-1.2.2/sw360/attachments.py
+-rw-r--r--   0        0        0     1595 2023-08-07 20:12:29.939763 sw360-1.2.2/sw360/clearing.py
+-rw-r--r--   0        0        0     9829 2023-08-07 20:12:29.939763 sw360-1.2.2/sw360/components.py
+-rw-r--r--   0        0        0     4490 2023-08-07 20:47:57.033968 sw360-1.2.2/sw360/license.py
+-rw-r--r--   0        0        0    18691 2023-08-07 20:50:54.713415 sw360-1.2.2/sw360/project.py
+-rw-r--r--   0        0        0     8476 2023-08-07 20:12:29.941762 sw360-1.2.2/sw360/releases.py
+-rw-r--r--   0        0        0     7012 2023-08-07 20:12:29.941762 sw360-1.2.2/sw360/sw360_api.py
+-rw-r--r--   0        0        0     1246 2023-08-07 20:12:29.942763 sw360-1.2.2/sw360/sw360error.py
+-rw-r--r--   0        0        0     4780 2023-08-07 20:50:13.710607 sw360-1.2.2/sw360/sw360oauth2.py
+-rw-r--r--   0        0        0     3509 2023-08-07 20:12:29.943762 sw360-1.2.2/sw360/vendor.py
+-rw-r--r--   0        0        0     1433 2023-08-07 20:12:29.943762 sw360-1.2.2/sw360/vulnerabilities.py
+-rw-r--r--   0        0        0     4540 1970-01-01 00:00:00.000000 sw360-1.2.2/PKG-INFO
```

### Comparing `sw360-1.2.1/License.md` & `sw360-1.2.2/License.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+<!--
+# SPDX-FileCopyrightText: (c) 2019-2023 Siemens
+# SPDX-License-Identifier: MIT
+-->
+
 # MIT License
 
 Copyright (c) 2019-2023 Siemens AG
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `sw360-1.2.1/pyproject.toml` & `sw360-1.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+# SPDX-FileCopyrightText: (c) 2018-2023 Siemens
+# SPDX-License-Identifier: MIT
+
 [tool.poetry]
 name = "sw360"
-version = "1.2.1"
+version = "1.2.2"
 description = "Python interface to the SW360 software component catalogue"
 authors = ["Thomas Graf <thomas.graf@siemens.com>",
 "Gernot Hillier <gernot.hillier@siemens.com>"]
 license = "MIT License"
 readme="Readme.md"
 include = ["LICENSE.md"]
 repository = "https://github.com/sw360/sw360python"
@@ -17,23 +20,24 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7" # because 3.7 is the minimum requirement for yarl
-requests = "^2.12.0"
+requests = "^2.31.0" # fix CVE-2023-32681
+urllib3 = "1.26.15"
 
 [tool.poetry.dev-dependencies]
 colorama = "0.3.7"
 sphinx = "^2.4.1"
 vcrpy = "4.0.2"
 yarl = "1.8.2" # force this version because 1.7.2 will not install
 flake8 = ">=3.7.8"
-responses = "^0.12.1"
-pytest = "6.2.5"
+responses = "^0.17"
+pytest = "^7.2.2"
 coverage = "5.3"
 types-requests = "2.27.11"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `sw360-1.2.1/Readme.md` & `sw360-1.2.2/Readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+<!--
+# SPDX-FileCopyrightText: (c) 2019-2023 Siemens
+# SPDX-License-Identifier: MIT
+-->
+
 # SW360 Base Library for Python
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/tngraf/Python-GitHub-Example/blob/main/LICENSE)
-[![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8%2C3.9-yellow?logo=python)](https://www.python.org/doc/versions/)
-[![PyPI version](https://badge.fury.io/py/sw360.svg)](https://badge.fury.io/py/sw360)
-[![Static checks](https://github.com/sw360/sw360python/actions/workflows/python-package.yml/badge.svg)](https://github.com/sw360/sw360python/actions/workflows/python-package.yml)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/sw360python/blob/master/License.md)
+[![Python Version](https://img.shields.io/badge/python-3.7%2C3.8%2C3.9-yellow?logo=python)](https://www.python.org/doc/versions/)
+[![PyPI version](https://img.shields.io/badge/pypi%20package-1.2.1-green)](https://pypi.org/project/sw360/)
+[![Static checks](https://github.com/sw360/sw360python/actions/workflows/static-checks.yml/badge.svg)](https://github.com/sw360/sw360python/actions/workflows/static-checks.yml)
 [![Unit tests](https://github.com/sw360/sw360python/actions/workflows/unit-test.yml/badge.svg)](https://github.com/sw360/sw360python/actions/workflows/unit-test.yml)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/tngraf/6ab639b6f9d1f6161d3db52d348d2997/raw/666fa870981726e1fa3469b6aa668c20fdd9d1b2/sw360python-cobertura-coverage.json&color=green)](https://github.com/sw360/sw360python/actions/workflows/unit-test.yml)
+[![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)
 
 This Python project implements the REST API of [SW360](https://www.eclipse.org/sw360/)
 and allows an easy way to interact with SW360.
 
 ## Documentation
 
 Have a look at the documentation: https://sw360.github.io/sw360python/
```

### Comparing `sw360-1.2.1/sw360/.editorconfig` & `sw360-1.2.2/sw360/.editorconfig`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-
-
 # EditorConfig is awesome: https://EditorConfig.org
 
+# SPDX-FileCopyrightText: (c) 2018-2023 Siemens
+# SPDX-License-Identifier: MIT
+
 # top-most EditorConfig file
 root = true
 
 # Unix-style newlines with a newline ending every file
 [*]
 end_of_line = crlf
 insert_final_newline = true
```

### Comparing `sw360-1.2.1/sw360/attachments.py` & `sw360-1.2.2/sw360/attachments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
@@ -165,15 +165,18 @@
 
         API endpoint: GET /attachments
         """
 
         hdr = self.api_headers.copy()
         hdr["Accept"] = "application/*"
         req = requests.get(download_url, allow_redirects=True, headers=hdr)
-        open(filename, "wb").write(req.content)
+        if req.ok:
+            open(filename, "wb").write(req.content)
+        else:
+            raise SW360Error(req, download_url)
 
     def _upload_resource_attachment(self, resource_type, resource_id, upload_file,
                                     upload_type="SOURCE", upload_comment=""):
         """Upload `upload_file` as attachment to SW360 for the resource with the given id
         using `upload_comment` for it. `upload_type` can be
         "DOCUMENT"
         "SOURCE"
```

### Comparing `sw360-1.2.1/sw360/clearing.py` & `sw360-1.2.2/sw360/clearing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/sw360/components.py` & `sw360-1.2.2/sw360/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/sw360/license.py` & `sw360-1.2.2/sw360/license.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
@@ -18,15 +18,15 @@
 
 class LicenseMixin:
     def create_new_license(
         self,
         shortName: str,
         fullName: str,
         text: str,
-        checked: False,
+        checked: bool = False,
         license_details={},
     ) -> Any:
         """Create a new component
 
         API endpoint: POST /licenses
 
         :param shortName: short license name. i.e "MIT"
```

### Comparing `sw360-1.2.1/sw360/project.py` & `sw360-1.2.2/sw360/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2023 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
@@ -59,15 +59,15 @@
         :return: a project
         :rtype: JSON project object
         :raises SW360Error: if there is a negative HTTP response
         """
         resp = self.api_get(url)
         return resp
 
-    def get_projects(self, all_details=False, page=-1, page_size=-1):
+    def get_projects(self, all_details: bool = False, page: int = -1, page_size: int = -1):
         """Get all projects
 
         API endpoint: GET /projects
 
         :param all_details: retrieve all project details (optional))
         :type all_details: bool
         :return: list of projects
@@ -129,15 +129,15 @@
         projects = projects["_embedded"]["sw360:projects"]
 
         for key in projects:
             resp.append(key["name"] + ", " + key["version"])
 
         return resp
 
-    def get_projects_by_name(self, name):
+    def get_projects_by_name(self, name: str):
         """Get a project by its name
 
         API endpoint: GET /projects
 
         :param name: the project name or a prefix of it
         :type name: string
         :return: list of projects
@@ -153,15 +153,15 @@
 
         if "sw360:projects" not in resp["_embedded"]:
             return None
 
         resp = resp["_embedded"]["sw360:projects"]
         return resp
 
-    def get_projects_by_external_id(self, ext_id_name, ext_id_value=""):
+    def get_projects_by_external_id(self, ext_id_name: str, ext_id_value: str = ""):
         """Get projects by external id. `ext_id_value` can be left blank to
         search for all projects with `ext_id_name`.
 
         API endpoint: GET /projects
 
         :param ext_id_name: the name of the external id to look for
         :param ext_id_value: the value of the external id to look for
@@ -181,15 +181,15 @@
 
         if "sw360:projects" not in resp["_embedded"]:
             return None
 
         resp = resp["_embedded"]["sw360:projects"]
         return resp
 
-    def get_projects_by_group(self, group, all_details=False):
+    def get_projects_by_group(self, group: str, all_details: bool = False):
         """Get projects by group.
 
         API endpoint: GET /projects?group=
 
         :param group: the group the projects shall belong to
         :type group: string
         :return: list of projects
@@ -209,15 +209,15 @@
 
         if "sw360:projects" not in resp["_embedded"]:
             return None
 
         resp = resp["_embedded"]["sw360:projects"]
         return resp
 
-    def get_projects_by_tag(self, tag):
+    def get_projects_by_tag(self, tag: str):
         """Get projects by tag.
 
         API endpoint: GET /projects?tag=
 
         :param group: the group the projects shall belong to
         :type group: string
         :return: list of projects
@@ -234,15 +234,15 @@
 
         if "sw360:projects" not in resp["_embedded"]:
             return None
 
         resp = resp["_embedded"]["sw360:projects"]
         return resp
 
-    def get_project_vulnerabilities(self, project_id):
+    def get_project_vulnerabilities(self, project_id: str):
         """Get the security vulnerabilities for the specified project.
 
         API endpoint: GET /projects/id/vulnerabilities
 
         :param project_id: the id of the project
         :type project_id: string
         :return: list of security vulnerabilities
```

### Comparing `sw360-1.2.1/sw360/releases.py` & `sw360-1.2.2/sw360/releases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/sw360/sw360_api.py` & `sw360-1.2.2/sw360/sw360_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
+# Copyright (c) 2019-2022 Siemens
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/sw360/sw360error.py` & `sw360-1.2.2/sw360/sw360error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/sw360/sw360oauth2.py` & `sw360-1.2.2/sw360/sw360oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -------------------------------------------------------------------------------
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
 
@@ -57,15 +57,15 @@
         except Exception as ex:
             raise SW360Error(None, url, message="Unable to connect to oauth2 service: " + repr(ex))
 
         data = response.json()[0]
         self._client_id = data["client_id"]
         self._client_secret = data["client_secret"]
 
-    def create_client(self, description: str, writeable: False) -> None:
+    def create_client(self, description: str, writeable: bool = False) -> None:
         """Create an OAuth2 client
 
         Args:
             description (str): Some description of the client
             writeable (bool): Create the id read/writeable
 
         Raises:
```

### Comparing `sw360-1.2.1/sw360/vendor.py` & `sw360-1.2.2/sw360/vendor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/sw360/vulnerabilities.py` & `sw360-1.2.2/sw360/vulnerabilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------------
-# (c) 2019-2022 Siemens AG
-# (c) 2022 BMW CarIT GmbH
+# Copyright (c) 2019-2022 Siemens
+# Copyright (c) 2022 BMW CarIT GmbH
 # All Rights Reserved.
 # Authors: thomas.graf@siemens.com, gernot.hillier@siemens.com
 # Authors: helio.chissini-de-castro@bmw.de
 #
 # Licensed under the MIT license.
 # SPDX-License-Identifier: MIT
 # -------------------------------------------------------------------------------
```

### Comparing `sw360-1.2.1/PKG-INFO` & `sw360-1.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw360
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python interface to the SW360 software component catalogue
 Home-page: https://github.com/sw360/sw360python
 License: MIT
 Author: Thomas Graf
 Author-email: thomas.graf@siemens.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,25 +16,33 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: requests (>=2.12.0,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: urllib3 (==1.26.15)
 Project-URL: Repository, https://github.com/sw360/sw360python
 Description-Content-Type: text/markdown
 
+<!--
+# SPDX-FileCopyrightText: (c) 2019-2023 Siemens
+# SPDX-License-Identifier: MIT
+-->
+
 # SW360 Base Library for Python
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/tngraf/Python-GitHub-Example/blob/main/LICENSE)
-[![Python Version](https://img.shields.io/badge/python-3.6%2C3.7%2C3.8%2C3.9-yellow?logo=python)](https://www.python.org/doc/versions/)
-[![PyPI version](https://badge.fury.io/py/sw360.svg)](https://badge.fury.io/py/sw360)
-[![Static checks](https://github.com/sw360/sw360python/actions/workflows/python-package.yml/badge.svg)](https://github.com/sw360/sw360python/actions/workflows/python-package.yml)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/sw360/sw360python/blob/master/License.md)
+[![Python Version](https://img.shields.io/badge/python-3.7%2C3.8%2C3.9-yellow?logo=python)](https://www.python.org/doc/versions/)
+[![PyPI version](https://img.shields.io/badge/pypi%20package-1.2.1-green)](https://pypi.org/project/sw360/)
+[![Static checks](https://github.com/sw360/sw360python/actions/workflows/static-checks.yml/badge.svg)](https://github.com/sw360/sw360python/actions/workflows/static-checks.yml)
 [![Unit tests](https://github.com/sw360/sw360python/actions/workflows/unit-test.yml/badge.svg)](https://github.com/sw360/sw360python/actions/workflows/unit-test.yml)
+[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/tngraf/6ab639b6f9d1f6161d3db52d348d2997/raw/666fa870981726e1fa3469b6aa668c20fdd9d1b2/sw360python-cobertura-coverage.json&color=green)](https://github.com/sw360/sw360python/actions/workflows/unit-test.yml)
+[![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)
 
 This Python project implements the REST API of [SW360](https://www.eclipse.org/sw360/)
 and allows an easy way to interact with SW360.
 
 ## Documentation
 
 Have a look at the documentation: https://sw360.github.io/sw360python/
```

