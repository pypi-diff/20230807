# Comparing `tmp/arcana_xnat-0.3.1.tar.gz` & `tmp/arcana_xnat-0.3.2.tar.gz`

## Comparing `arcana_xnat-0.3.1.tar` & `arcana_xnat-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/base.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/entrypoint.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/update_release.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_add_columns.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_dataset_export.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_store.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_xnat_images.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/__init__.py
--rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/api.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/cs.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/tests/test_store.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/__init__.py
--rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/command.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/image.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/utils/__init__.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/utils/testing.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/.gitignore
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/LICENSE
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/README.rst
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    21719 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/base.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/entrypoint.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/update_release.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_add_columns.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_dataset_export.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_store.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_xnat_images.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/__init__.py
+-rw-r--r--   0        0        0    24191 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/api.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/cs.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/data/tests/test_store.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/__init__.py
+-rw-r--r--   0        0        0    12992 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/command.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/image.py
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/deploy/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/utils/__init__.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/arcana/xnat/utils/testing.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/.gitignore
+-rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/README.rst
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    21749 2020-02-02 00:00:00.000000 arcana_xnat-0.3.2/PKG-INFO
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/cli/entrypoint.py` & `arcana_xnat-0.3.2/arcana/xnat/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/arcana/xnat/cli/update_release.py` & `arcana_xnat-0.3.2/arcana/xnat/cli/update_release.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_add_columns.py` & `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_add_columns.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     dataset.save(dataset_name)
 
     result = cli_runner(
         add_source,
         [
             dataset_locator,
             "a_source",
-            "fileformats.text:Plain",
+            "text/text-file",
             "--path",
             "file1",
             "--row-frequency",
             "session",
             "--quality",
             "questionable",
             "--order",
@@ -43,15 +43,15 @@
     dataset.save(dataset_name)
 
     result = cli_runner(
         add_sink,
         [
             dataset_locator,
             "a_sink",
-            "fileformats.text:Plain",
+            "text/text-file",
             "--path",
             "deriv",
             "--row-frequency",
             "session",
             "--salience",
             "qa",
         ],
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_dataset_export.py` & `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_dataset_export.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_store.py` & `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_xnat_images.py` & `arcana_xnat-0.3.2/arcana/xnat/cli/tests/test_cli_xnat_images.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/arcana/xnat/data/api.py` & `arcana_xnat-0.3.2/arcana/xnat/data/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from arcana.core.exceptions import (
     ArcanaError,
     ArcanaUsageError,
 )
 from arcana.core.utils.serialize import asdict
 from arcana.core.data.tree import DataTree
 from arcana.core.data.entry import DataEntry
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 
 
 logger = logging.getLogger("arcana")
 
 tag_parse_re = re.compile(r"\((\d+),(\d+)\)")
 
 RELEVANT_DICOM_TAG_TYPES = set(("UI", "CS", "DA", "TM", "SH", "LO", "PN", "ST", "AS"))
@@ -354,22 +354,22 @@
         with self.connection:
             # Download resource to zip file
             zip_path = op.join(download_dir, "download.zip")
             with open(zip_path, "wb") as f:
                 self.connection.download_stream(
                     entry.uri + "/files", f, format="zip", verbose=True
                 )
-            # Extract downloaded zip file
-            expanded_dir = download_dir / "expanded"
-            try:
-                with ZipFile(zip_path) as zip_file:
-                    zip_file.extractall(expanded_dir)
-            except BadZipfile as e:
-                raise ArcanaError(f"Could not unzip file '{zip_path}' ({e})") from e
-            data_path = glob(str(expanded_dir) + "/**/files", recursive=True)[0]
+        # Extract downloaded zip file
+        expanded_dir = download_dir / "expanded"
+        try:
+            with ZipFile(zip_path) as zip_file:
+                zip_file.extractall(expanded_dir)
+        except BadZipfile as e:
+            raise ArcanaError(f"Could not unzip file '{zip_path}' ({e})") from e
+        data_path = next(expanded_dir.glob("**/files"))
         return data_path
 
     def upload_files(self, cache_path: Path, entry: DataEntry):
         """Upload all files contained within `input_dir` to the specified entry in the
         data store
 
         Parameters
@@ -560,14 +560,17 @@
             if row.frequency == Clinical.dataset:
                 xrow = xproject
             elif row.frequency == Clinical.subject:
                 xrow = xproject.subjects[row.frequency_id("subject")]
             elif row.frequency == Clinical.session:
                 xrow = xproject.experiments[row.frequency_id("session")]
             else:
+                # For rows that don't have a place within the standard XNAT hierarchy,
+                # e.g. groups, we create a dummy subject with an escaped name to hold
+                # the associated data
                 xrow = self.connection.classes.SubjectData(
                     label=self.make_row_name(row), parent=xproject
                 )
             return xrow
 
     def get_dicom_header(self, uri: str):
         def convert(val, code):
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/data/cs.py` & `arcana_xnat-0.3.2/arcana/xnat/data/cs.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 containers
 """
 import os
 import re
 import logging
 from pathlib import Path
 import attrs
-from fileformats.core.base import FileSet
-from arcana.stdlib import Clinical
+from fileformats.core import FileSet
+from arcana.common import Clinical
 from arcana.core.data.space import DataSpace
 from arcana.core.data.row import DataRow
 from arcana.core.data.entry import DataEntry
 from arcana.core.exceptions import ArcanaNoDirectXnatMountException
 from .api import Xnat, path2label
 
 logger = logging.getLogger("arcana")
@@ -88,37 +88,36 @@
             "Getting %s from %s:%s row via direct access to archive directory",
             entry.path,
             entry.row.frequency,
             entry.row.id,
         )
         if entry.is_derivative:
             # entry is in input mount
-            stem_path = self.entry_fspath(entry)
-            fspaths = list(stem_path.iterdir())
+            resource_path = self.entry_fspath(entry)
         else:
             path = re.match(
                 r"/data/(?:archive/)?projects/[a-zA-Z0-9\-_]+/"
                 r"(?:subjects/[a-zA-Z0-9\-_]+/)?"
                 r"(?:experiments/[a-zA-Z0-9\-_]+/)?(?P<path>.*)$",
                 entry.uri,
             ).group("path")
             if "scans" in path:
                 path = path.replace("scans", "SCANS").replace("resources/", "")
             path = path.replace("resources", "RESOURCES")
             resource_path = input_mount / path
-            fspaths = list(resource_path.iterdir())
+        fspaths = list(p for p in resource_path.iterdir() if not p.name.endswith("_catalog.xml"))
         return datatype(fspaths)
 
     def put_fileset(self, fileset: FileSet, entry: DataEntry) -> FileSet:
         if not entry.is_derivative:
             super().put_fileset(fileset, entry)  # Fallback to API access
-        cached = fileset.copy_to(
+        cached = fileset.copy(
             dest_dir=self.output_mount,
             make_dirs=True,
-            stem=entry.path.split("/")[-1].split("@")[0],
+            new_stem=entry.path.split("/")[-1].split("@")[0],
             trim=False,
             overwrite=True,
         )
         logger.info(
             "Put %s into %s:%s row via direct access to archive directory",
             entry.path,
             entry.row.frequency,
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/data/tests/test_store.py` & `arcana_xnat-0.3.2/arcana/xnat/data/tests/test_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import operator as op
 import shutil
 import logging
 from pathlib import Path
 from functools import reduce
 import itertools
 import pytest
+from pydra.utils.hash import hash_single, Cache
 from fileformats.generic import File
 from fileformats.field import Text as TextField
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 from arcana.core.data.set import Dataset
 from arcana.xnat.data import XnatViaCS
 from arcana.core.utils.serialize import asdict
 
 if sys.platform == "win32":
 
     def get_perms(f):
@@ -174,7 +175,14 @@
 
     with data_store.connection:
         entry = data_store.create_entry("provtest@", datatype, simple_dataset.root)
         data_store.put(datatype(value), entry)  # Create the entry first
         data_store.put_provenance(provenance, entry)  # Save the provenance
         reloaded_provenance = data_store.get_provenance(entry)  # reload the provenance
         assert provenance == reloaded_provenance
+
+
+def test_dataset_bytes_hash(static_dataset):
+
+    hsh = hash_single(static_dataset, Cache({}))
+    # Check hashing is stable
+    assert hash_single(static_dataset, Cache({})) == hsh
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/deploy/command.py` & `arcana_xnat-0.3.2/arcana/xnat/deploy/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 import typing as ty
 import re
 import attrs
 from fileformats.core import FileSet
 from arcana.core.deploy.command.base import ContainerCommand
 from arcana.xnat.data import XnatViaCS
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 from arcana.core.utils.serialize import ClassResolver
 
 if ty.TYPE_CHECKING:
     from .image import XnatApp
 
 
 @attrs.define(kw_only=True)
 class XnatCommand(ContainerCommand):
 
-    image: XnatApp = None
+    image: ty.Optional[XnatApp] = None
 
     # Hard-code the data_space of XNAT commands to be clinical
     DATA_SPACE = Clinical
 
     def make_json(self):
         """Constructs the XNAT CS "command" JSON config, which specifies how XNAT
         should handle the containerised pipeline
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/deploy/image.py` & `arcana_xnat-0.3.2/arcana/xnat/deploy/image.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/arcana/xnat/deploy/tests/test_app.py` & `arcana_xnat-0.3.2/arcana/xnat/deploy/tests/test_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             "registry": "a.docker.registry.io",
             "packages": {
                 "system": ["git", "vim"],
                 "pip": [
                     "arcana",
                     "arcana-xnat",
                     "fileformats",
-                    "fileformats-testing",
                     "fileformats-medimage",
                     "pydra",
                 ],
             },
         }
         blueprint = TEST_XNAT_DATASET_BLUEPRINTS["concatenate_test"]
         project_id = run_prefix + "concatenate_test"
@@ -78,14 +77,15 @@
                 "system": ["git", "vim"],
                 "pip": [
                     "arcana",
                     "arcana-xnat",
                     "arcana-bids",
                     "fileformats",
                     "fileformats-medimage",
+                    "fileformats-medimage-extras",
                     "pydra",
                 ],
             },
             "command": bids_command_spec,
             "authors": [
                 {"name": "Some One Else", "email": "some.oneelse@an.email.org"}
             ],
```

### Comparing `arcana_xnat-0.3.1/arcana/xnat/utils/testing.py` & `arcana_xnat-0.3.2/arcana/xnat/utils/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as ty
 import time
 from pathlib import Path
 import logging
 import tempfile
 import attrs
 import xnat
-from arcana.stdlib import Clinical
+from arcana.common import Clinical
 from arcana.core.data.space import DataSpace
 from arcana.core.data.row import DataRow
 from arcana.testing.data.blueprint import TestDatasetBlueprint, FileSetEntryBlueprint
 from arcana.core.exceptions import ArcanaError
 
 
 logger = logging.getLogger("arcana")
@@ -26,17 +26,17 @@
 class TestXnatDatasetBlueprint(TestDatasetBlueprint):
 
     scans: ty.List[ScanBlueprint]
 
     # Overwrite attributes in core blueprint class
     space: type = Clinical
     hierarchy: list[DataSpace] = ["subject", "session"]
-    filesets: list[str] = None
+    filesets: ty.Optional[list[str]] = None
 
-    def make_entries(self, row: DataRow, source_data: Path = None):
+    def make_entries(self, row: DataRow, source_data: ty.Optional[Path] = None):
         logger.debug("Making entries in %s row: %s", row, self.scans)
         xrow = row.dataset.store.get_xrow(row)
         xclasses = xrow.xnat_session.classes
         for scan_id, scan_bp in enumerate(self.scans, start=1):
             xscan = xclasses.MrScanData(
                 id=scan_id, type=scan_bp.name, parent=xrow
             )
@@ -46,15 +46,15 @@
                 xresource = xscan.create_resource(resource_bp.path)
                 # Create the dummy files
                 item = resource_bp.make_item(
                     source_data=source_data,
                     source_fallback=True,
                     escape_source_name=False,
                 )
-                item.copy_to(tmp_dir)
+                item.copy(tmp_dir)
                 xresource.upload_dir(tmp_dir)
 
 
 def install_and_launch_xnat_cs_command(
     command_json: dict,
     project_id: str,
     session_id: str,
```

### Comparing `arcana_xnat-0.3.1/LICENSE` & `arcana_xnat-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/README.rst` & `arcana_xnat-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.1/pyproject.toml` & `arcana_xnat-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 [project]
 name = "arcana-xnat"
 description = "An extension of the Arcana framework to apply workflows and analyses on data stored within XNAT data repositories"
 readme = "README.rst"
 requires-python = ">=3.8"
 dependencies = [
     "arcana",
-    "fileformats[extended] >=0.3.3",
-    "fileformats-medimage[extended] >=0.2.1",
+    "fileformats >=0.3.3",
+    "fileformats-medimage >=0.2.1",
+    "fileformats-medimage-extras >=0.1.3",
     "xnat==0.4.3",
 ]
 license = {file = "LICENSE"}
 authors = [{name = "Thomas G. Close", email = "tom.g.close@gmail.com"}]
 maintainers = [{name = "Thomas G. Close", email = "tom.g.close@gmail.com"}]
 keywords = ["arcana"]
 classifiers = [
```

### Comparing `arcana_xnat-0.3.1/PKG-INFO` & `arcana_xnat-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-xnat
-Version: 0.3.1
+Version: 0.3.2
 Summary: An extension of the Arcana framework to apply workflows and analyses on data stored within XNAT data repositories
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-xnat.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
         
@@ -127,16 +127,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: arcana
-Requires-Dist: fileformats-medimage[extended]>=0.2.1
-Requires-Dist: fileformats[extended]>=0.3.3
+Requires-Dist: fileformats-medimage-extras>=0.1.3
+Requires-Dist: fileformats-medimage>=0.2.1
+Requires-Dist: fileformats>=0.3.3
 Requires-Dist: xnat==0.4.3
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

