# Comparing `tmp/wbFontParts-0.2.1.tar.gz` & `tmp/wbFontParts-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbFontParts-0.2.1.tar", last modified: Thu Aug  3 07:11:17 2023, max compression
+gzip compressed data, was "wbFontParts-0.2.2.tar", last modified: Mon Aug  7 10:51:18 2023, max compression
```

## Comparing `wbFontParts-0.2.1.tar` & `wbFontParts-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.867367 wbFontParts-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.862367 wbFontParts-0.2.1/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.866367 wbFontParts-0.2.1/Lib/wbFontParts/
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/bPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/color.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/component.py
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/contour.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/features.py
--rw-rw-rw-   0 root         (0) root         (0)     9918 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/font.py
--rw-rw-rw-   0 root         (0) root         (0)     5810 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/groups.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/guideline.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/image.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/info.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/kerning.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/layer.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/lib.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/point.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/Lib/wbFontParts/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 07:11:17.867367 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2038 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      689 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-08-03 07:11:17.000000 wbFontParts-0.2.1/Lib/wbFontParts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2038 2023-08-03 07:11:17.867367 wbFontParts-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2249 2023-08-03 07:11:17.868367 wbFontParts-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-03 07:11:16.000000 wbFontParts-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:51:18.960581 wbFontParts-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:51:18.954581 wbFontParts-0.2.2/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:51:18.958581 wbFontParts-0.2.2/Lib/wbFontParts/
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/bPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/color.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     9918 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/font.py
+-rw-rw-rw-   0 root         (0) root         (0)     5810 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/guideline.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/image.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      656 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/kerning.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/point.py
+-rw-rw-rw-   0 root         (0) root         (0)      537 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/Lib/wbFontParts/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 10:51:18.960581 wbFontParts-0.2.2/Lib/wbFontParts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-08-07 10:51:18.000000 wbFontParts-0.2.2/Lib/wbFontParts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      689 2023-08-07 10:51:18.000000 wbFontParts-0.2.2/Lib/wbFontParts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 10:51:18.000000 wbFontParts-0.2.2/Lib/wbFontParts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-08-07 10:51:18.000000 wbFontParts-0.2.2/Lib/wbFontParts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-07 10:51:18.000000 wbFontParts-0.2.2/Lib/wbFontParts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-08-07 10:51:18.960581 wbFontParts-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2249 2023-08-07 10:51:18.960581 wbFontParts-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-08-07 10:51:17.000000 wbFontParts-0.2.2/setup.py
```

### Comparing `wbFontParts-0.2.1/LICENSE` & `wbFontParts-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/anchor.py` & `wbFontParts-0.2.2/Lib/wbFontParts/anchor.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/bPoint.py` & `wbFontParts-0.2.2/Lib/wbFontParts/bPoint.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/color.py` & `wbFontParts-0.2.2/Lib/wbFontParts/color.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/component.py` & `wbFontParts-0.2.2/Lib/wbFontParts/component.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/contour.py` & `wbFontParts-0.2.2/Lib/wbFontParts/contour.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/features.py` & `wbFontParts-0.2.2/Lib/wbFontParts/features.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/font.py` & `wbFontParts-0.2.2/Lib/wbFontParts/font.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/glyph.py` & `wbFontParts-0.2.2/Lib/wbFontParts/glyph.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/groups.py` & `wbFontParts-0.2.2/Lib/wbFontParts/groups.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/guideline.py` & `wbFontParts-0.2.2/Lib/wbFontParts/guideline.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/image.py` & `wbFontParts-0.2.2/Lib/wbFontParts/image.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/info.py` & `wbFontParts-0.2.2/Lib/wbFontParts/info.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/kerning.py` & `wbFontParts-0.2.2/Lib/wbFontParts/kerning.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/layer.py` & `wbFontParts-0.2.2/Lib/wbFontParts/layer.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/lib.py` & `wbFontParts-0.2.2/Lib/wbFontParts/lib.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/point.py` & `wbFontParts-0.2.2/Lib/wbFontParts/point.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts/segment.py` & `wbFontParts-0.2.2/Lib/wbFontParts/segment.py`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts.egg-info/PKG-INFO` & `wbFontParts-0.2.2/Lib/wbFontParts.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbFontParts
-Version: 0.2.1
+Version: 0.2.2
 Summary: A wrapper around fontParts for UFO Workbench.
 Home-page: https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Project-URL: Documentation, https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts/
 Project-URL: Tracker, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts/-/issues
@@ -31,26 +31,7 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-# wbFontParts
-
-## A wrapper around fontParts for Workbench applications.
-
-[fontparts](https://pypi.org/project/fontParts/) is an API for interacting 
-with the parts of fonts during the font development process.
-
-This provides the API layer for UFO-Workbench.
-
-## Installation
-
-```shell
-pip install wbFontParts
-```
-
-## Documentation
-
-For details read the [Documentation](https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts).
```

### Comparing `wbFontParts-0.2.1/Lib/wbFontParts.egg-info/SOURCES.txt` & `wbFontParts-0.2.2/Lib/wbFontParts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wbFontParts-0.2.1/PKG-INFO` & `wbFontParts-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbFontParts
-Version: 0.2.1
+Version: 0.2.2
 Summary: A wrapper around fontParts for UFO Workbench.
 Home-page: https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 Project-URL: Documentation, https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts/
 Project-URL: Tracker, https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts/-/issues
@@ -31,26 +31,7 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: Topic :: Multimedia :: Graphics
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-# wbFontParts
-
-## A wrapper around fontParts for Workbench applications.
-
-[fontparts](https://pypi.org/project/fontParts/) is an API for interacting 
-with the parts of fonts during the font development process.
-
-This provides the API layer for UFO-Workbench.
-
-## Installation
-
-```shell
-pip install wbFontParts
-```
-
-## Documentation
-
-For details read the [Documentation](https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts).
```

### Comparing `wbFontParts-0.2.1/setup.cfg` & `wbFontParts-0.2.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.2.2
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
@@ -12,15 +12,15 @@
 replace = __version__ = "{new_version}"
 
 [metadata]
 name = wbFontParts
 version = attr: wbFontParts.__version__
 author = Andreas Eigendorf
 description = A wrapper around fontParts for UFO Workbench.
-long_description = file: readme.md
+long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 url = https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 project_urls = 
 	Source = https://gitlab.com/workbench2/WorkBenchExtensions/wbFontParts
 	Documentation = https://workbench2.gitlab.io/WorkBenchExtensions/wbFontParts/
@@ -61,15 +61,15 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	wbDefcon>=0.2.3
 	compreffor>=0.5.4
 	glyphsLib>=6.3.0
 	psautohint>=2.4.0
-	ufo2ft>=2.33.3
+	ufo2ft>=2.33.4
 
 [options.packages.find]
 where = Lib
 
 [tox:tox]
 min_version = 4.6
 env_list =
```

