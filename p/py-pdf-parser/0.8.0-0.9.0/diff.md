# Comparing `tmp/py-pdf-parser-0.8.0.tar.gz` & `tmp/py-pdf-parser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pdf-parser-0.8.0.tar", last modified: Thu May 13 08:10:30 2021, max compression
+gzip compressed data, was "py-pdf-parser-0.9.0.tar", last modified: Wed Jun  9 08:48:31 2021, max compression
```

## Comparing `py-pdf-parser-0.8.0.tar` & `py-pdf-parser-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/py_pdf_parser/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    18110 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/components.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    38745 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     6174 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/sectioning.py
--rw-r--r--   0 runner    (1001) docker     (121)    19167 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/py_pdf_parser/visualise/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/visualise/background.py
--rw-r--r--   0 runner    (1001) docker     (121)     2719 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/visualise/info_figure.py
--rw-r--r--   0 runner    (1001) docker     (121)    11118 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/visualise/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    12076 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/py_pdf_parser/visualise/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/py_pdf_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-05-13 08:10:30.000000 py-pdf-parser-0.8.0/py_pdf_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-05-13 08:10:30.000000 py-pdf-parser-0.8.0/py_pdf_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-13 08:10:30.000000 py-pdf-parser-0.8.0/py_pdf_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      406 2021-05-13 08:10:30.000000 py-pdf-parser-0.8.0/py_pdf_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-05-13 08:10:30.000000 py-pdf-parser-0.8.0/py_pdf_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    13665 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_components.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-13 08:10:30.664742 py-pdf-parser-0.8.0/tests/test_doc_examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_doc_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_doc_examples/test_element_ordering.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_doc_examples/test_extracting_text_from_figures.py
--rw-r--r--   0 runner    (1001) docker     (121)     4145 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_doc_examples/test_order_summary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_doc_examples/test_simple_memo.py
--rw-r--r--   0 runner    (1001) docker     (121)     6893 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_doc_examples/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)    51132 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     8821 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_sectioning.py
--rw-r--r--   0 runner    (1001) docker     (121)    37043 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-05-13 08:08:35.000000 py-pdf-parser-0.8.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:31.945556 py-pdf-parser-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-06-09 08:48:31.945556 py-pdf-parser-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:31.941556 py-pdf-parser-0.9.0/py_pdf_parser/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18110 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/components.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38745 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6174 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/sectioning.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19167 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:31.941556 py-pdf-parser-0.9.0/py_pdf_parser/visualise/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/visualise/background.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2719 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/visualise/info_figure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11137 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/visualise/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12076 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/py_pdf_parser/visualise/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:31.941556 py-pdf-parser-0.9.0/py_pdf_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-06-09 08:48:31.000000 py-pdf-parser-0.9.0/py_pdf_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-06-09 08:48:31.000000 py-pdf-parser-0.9.0/py_pdf_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-09 08:48:31.000000 py-pdf-parser-0.9.0/py_pdf_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2021-06-09 08:48:31.000000 py-pdf-parser-0.9.0/py_pdf_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-06-09 08:48:31.000000 py-pdf-parser-0.9.0/py_pdf_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-09 08:48:31.945556 py-pdf-parser-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1860 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:31.945556 py-pdf-parser-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2328 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13665 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_components.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:31.945556 py-pdf-parser-0.9.0/tests/test_doc_examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_doc_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3510 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_doc_examples/test_element_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_doc_examples/test_extracting_text_from_figures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4145 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_doc_examples/test_order_summary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2779 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_doc_examples/test_simple_memo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6893 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_doc_examples/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51132 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8821 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_sectioning.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37043 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-06-09 08:48:24.000000 py-pdf-parser-0.9.0/tests/utils.py
```

### Comparing `py-pdf-parser-0.8.0/LICENSE` & `py-pdf-parser-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/PKG-INFO` & `py-pdf-parser-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pdf-parser
-Version: 0.8.0
+Version: 0.9.0
 Summary: A tool to help extracting information from structured PDFs.
 Home-page: https://github.com/jstockwin/py-pdf-parser
 Author: Jake Stockwin
 Author-email: jstockwin@gmail.com
 License: BSD
 Description: # py-pdf-parser
```

### Comparing `py-pdf-parser-0.8.0/README.md` & `py-pdf-parser-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/common.py` & `py-pdf-parser-0.9.0/py_pdf_parser/common.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/components.py` & `py-pdf-parser-0.9.0/py_pdf_parser/components.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/exceptions.py` & `py-pdf-parser-0.9.0/py_pdf_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/filtering.py` & `py-pdf-parser-0.9.0/py_pdf_parser/filtering.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/loaders.py` & `py-pdf-parser-0.9.0/py_pdf_parser/loaders.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/sectioning.py` & `py-pdf-parser-0.9.0/py_pdf_parser/sectioning.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/tables.py` & `py-pdf-parser-0.9.0/py_pdf_parser/tables.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/visualise/background.py` & `py-pdf-parser-0.9.0/py_pdf_parser/visualise/background.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/visualise/info_figure.py` & `py-pdf-parser-0.9.0/py_pdf_parser/visualise/info_figure.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/visualise/main.py` & `py-pdf-parser-0.9.0/py_pdf_parser/visualise/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Dict, Tuple, Optional, TYPE_CHECKING
 
 import logging
 
 import matplotlib
 
-matplotlib.use("Qt5Agg", warn=False)  # noqa
+matplotlib.use("Qt5Agg")  # noqa
 from matplotlib import pyplot as plt
 from matplotlib.backend_bases import MouseButton
 
 from py_pdf_parser.components import PDFDocument
 from .background import get_pdf_background
 from .info_figure import get_clicked_element_info
 from .sections import SectionVisualiser
 
 if TYPE_CHECKING:
     from py_pdf_parser.filtering import ElementList
     from py_pdf_parser.components import PDFElement
     from matplotlib.figure import Figure, Text
     from matplotlib.axes import Axes
     from matplotlib.backend_bases import MouseEvent
-    import PyQt5
+    from PyQt5 import QtWidgets
 logger = logging.getLogger("PDFParser")
 
 
 STYLES = {
     "untagged": {"color": "#00a9f4", "linewidth": 1, "alpha": 0.5},
     "tagged": {"color": "#007ac1", "linewidth": 1, "alpha": 0.5},
     "ignored": {"color": "#67daff", "linewidth": 1, "alpha": 0.2, "linestyle": ":"},
@@ -40,18 +40,18 @@
 
     document: PDFDocument
     current_page: int
     __ax: "Axes"
     __fig: "Figure"
     __info_fig: Optional["Figure"] = None
     __info_text: Optional["Text"] = None
-    __first_page_button: "PyQt5.QtWidgets.QAction" = None
-    __previous_page_button: "PyQt5.QtWidgets.QAction" = None
-    __next_page_button: "PyQt5.QtWidgets.QAction" = None
-    __last_page_button: "PyQt5.QtWidgets.QAction" = None
+    __first_page_button: Optional["QtWidgets.QAction"] = None
+    __previous_page_button: Optional["QtWidgets.QAction"] = None
+    __next_page_button: Optional["QtWidgets.QAction"] = None
+    __last_page_button: Optional["QtWidgets.QAction"] = None
     __section_visualiser: "SectionVisualiser"
 
     __clicked_elements: Dict[MouseButton, "PDFElement"] = {}
 
     def __init__(
         self,
         document: PDFDocument,
```

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser/visualise/sections.py` & `py-pdf-parser-0.9.0/py_pdf_parser/visualise/sections.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser.egg-info/PKG-INFO` & `py-pdf-parser-0.9.0/py_pdf_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pdf-parser
-Version: 0.8.0
+Version: 0.9.0
 Summary: A tool to help extracting information from structured PDFs.
 Home-page: https://github.com/jstockwin/py-pdf-parser
 Author: Jake Stockwin
 Author-email: jstockwin@gmail.com
 License: BSD
 Description: # py-pdf-parser
```

### Comparing `py-pdf-parser-0.8.0/py_pdf_parser.egg-info/SOURCES.txt` & `py-pdf-parser-0.9.0/py_pdf_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/setup.py` & `py-pdf-parser-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ROOT_DIR = os.path.dirname(__file__)
 
 
 setup(
     name="py-pdf-parser",
     packages=find_packages(),
     exclude=["tests.*", "tests", "docs", "docs.*"],
-    version="0.8.0",
+    version="0.9.0",
     url="https://github.com/jstockwin/py-pdf-parser",
     license="BSD",
     description="A tool to help extracting information from structured PDFs.",
     long_description=open(os.path.join(ROOT_DIR, "README.md")).read(),
     long_description_content_type="text/markdown",
     author="Jake Stockwin",
     author_email="jstockwin@gmail.com",
@@ -29,35 +29,35 @@
         "pdfminer.six==20201018",
         "docopt==0.6.2",
         "wand==0.6.6",
         "PyYAML==5.4.1",
     ],
     extras_require={
         "dev": [
-            "matplotlib==3.1.2",
+            "matplotlib==3.4.2",
             "pillow==8.1.1",
-            "pyqt5==5.14.1",
+            "pyqt5==5.15.4",
             "pyvoronoi==1.0.5",
             "shapely==1.7.1",
         ],
         "test": [
-            "black==21.5b1",
+            "black==21.5b2",
             "ddt==1.4.2",
-            "matplotlib==3.1.2",
+            "matplotlib==3.4.2",
             "mock==4.0.3",
             "mypy==0.812",
             "nose==1.3.7",
             "pillow==8.1.1",
             "pycodestyle==2.7.0",
-            "pyqt5==5.14.1",
-            "pytype==2021.5.11",
+            "pyqt5==5.15.4",
+            "pytype==2021.5.25",
             "recommonmark==0.7.1",
             "sphinx-autobuild==2021.3.14",
             "sphinx-rtd-theme==0.5.2",
-            "Sphinx==4.0.1",
+            "Sphinx==4.0.2",
             # This is a sub-dependency but is pinned because the next version doesn't
             # install correctly. See:
             # https://github.com/scikit-build/ninja-python-distributions/issues/27
             "ninja==1.10.0.post2",
         ],
     },
 )
```

### Comparing `py-pdf-parser-0.8.0/tests/base.py` & `py-pdf-parser-0.9.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_common.py` & `py-pdf-parser-0.9.0/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_components.py` & `py-pdf-parser-0.9.0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_doc_examples/test_element_ordering.py` & `py-pdf-parser-0.9.0/tests/test_doc_examples/test_element_ordering.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_doc_examples/test_extracting_text_from_figures.py` & `py-pdf-parser-0.9.0/tests/test_doc_examples/test_extracting_text_from_figures.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_doc_examples/test_order_summary.py` & `py-pdf-parser-0.9.0/tests/test_doc_examples/test_order_summary.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_doc_examples/test_simple_memo.py` & `py-pdf-parser-0.9.0/tests/test_doc_examples/test_simple_memo.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_doc_examples/test_tables.py` & `py-pdf-parser-0.9.0/tests/test_doc_examples/test_tables.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_filtering.py` & `py-pdf-parser-0.9.0/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_loaders.py` & `py-pdf-parser-0.9.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_sectioning.py` & `py-pdf-parser-0.9.0/tests/test_sectioning.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/test_tables.py` & `py-pdf-parser-0.9.0/tests/test_tables.py`

 * *Files identical despite different names*

### Comparing `py-pdf-parser-0.8.0/tests/utils.py` & `py-pdf-parser-0.9.0/tests/utils.py`

 * *Files identical despite different names*

