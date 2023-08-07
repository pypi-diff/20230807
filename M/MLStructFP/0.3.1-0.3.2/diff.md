# Comparing `tmp/MLStructFP-0.3.1.tar.gz` & `tmp/MLStructFP-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLStructFP-0.3.1.tar", last modified: Fri Jan 27 21:47:37 2023, max compression
+gzip compressed data, was "MLStructFP-0.3.2.tar", last modified: Mon Aug  7 00:41:16 2023, max compression
```

## Comparing `MLStructFP-0.3.1.tar` & `MLStructFP-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.350000 MLStructFP-0.3.1/
--rw-rw-rw-   0        0        0     1086 2023-01-16 00:18:50.000000 MLStructFP-0.3.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.370000 MLStructFP-0.3.1/MLStructFP/
--rw-rw-rw-   0        0        0      639 2023-01-27 21:45:48.000000 MLStructFP-0.3.1/MLStructFP/__init__.py
--rw-rw-rw-   0        0        0      309 2023-01-22 21:54:56.000000 MLStructFP-0.3.1/MLStructFP/_types.py
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.410000 MLStructFP-0.3.1/MLStructFP/db/
--rw-rw-rw-   0        0        0      225 2023-01-16 00:38:24.000000 MLStructFP-0.3.1/MLStructFP/db/__init__.py
--rw-rw-rw-   0        0        0     1505 2023-01-12 14:48:22.000000 MLStructFP-0.3.1/MLStructFP/db/_c.py
--rw-rw-rw-   0        0        0     4692 2023-01-13 19:38:00.000000 MLStructFP-0.3.1/MLStructFP/db/_c_rect.py
--rw-rw-rw-   0        0        0     3099 2023-01-12 14:48:22.000000 MLStructFP-0.3.1/MLStructFP/db/_c_slab.py
--rw-rw-rw-   0        0        0     2390 2023-01-16 00:38:24.000000 MLStructFP-0.3.1/MLStructFP/db/_db_loader.py
--rw-rw-rw-   0        0        0     6376 2023-01-22 21:54:56.000000 MLStructFP-0.3.1/MLStructFP/db/_floor.py
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.430000 MLStructFP-0.3.1/MLStructFP/db/image/
--rw-rw-rw-   0        0        0      188 2023-01-16 00:38:24.000000 MLStructFP-0.3.1/MLStructFP/db/image/__init__.py
--rw-rw-rw-   0        0        0     4121 2023-01-27 21:45:48.000000 MLStructFP-0.3.1/MLStructFP/db/image/_base.py
--rw-rw-rw-   0        0        0     7732 2023-01-27 21:45:48.000000 MLStructFP-0.3.1/MLStructFP/db/image/_rect_binary.py
--rw-rw-rw-   0        0        0    19312 2023-01-25 13:21:10.000000 MLStructFP-0.3.1/MLStructFP/db/image/_rect_photo.py
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.460000 MLStructFP-0.3.1/MLStructFP/utils/
--rw-rw-rw-   0        0        0      215 2023-01-27 21:45:48.000000 MLStructFP-0.3.1/MLStructFP/utils/__init__.py
--rw-rw-rw-   0        0        0    11693 2023-01-22 21:54:56.000000 MLStructFP-0.3.1/MLStructFP/utils/_geometry.py
--rw-rw-rw-   0        0        0      867 2023-01-06 20:30:26.000000 MLStructFP-0.3.1/MLStructFP/utils/_mathlib.py
--rw-rw-rw-   0        0        0      293 2023-01-27 21:45:48.000000 MLStructFP-0.3.1/MLStructFP/utils/_path.py
--rw-rw-rw-   0        0        0     2824 2023-01-07 16:28:26.000000 MLStructFP-0.3.1/MLStructFP/utils/_plot.py
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.390000 MLStructFP-0.3.1/MLStructFP.egg-info/
--rw-rw-rw-   0        0        0     2021 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/MLStructFP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/MLStructFP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/MLStructFP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/MLStructFP.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/MLStructFP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2021 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-01-23 13:13:34.000000 MLStructFP-0.3.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-01-27 21:47:38.000000 MLStructFP-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1712 2023-01-25 13:20:46.000000 MLStructFP-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-27 21:47:37.480000 MLStructFP-0.3.1/test/
--rw-rw-rw-   0        0        0     3918 2023-01-25 13:21:10.000000 MLStructFP-0.3.1/test/test_db.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.900000 MLStructFP-0.3.2/
+-rw-rw-rw-   0        0        0     1086 2023-01-16 00:18:50.000000 MLStructFP-0.3.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.910000 MLStructFP-0.3.2/MLStructFP/
+-rw-rw-rw-   0        0        0      639 2023-08-07 00:16:52.000000 MLStructFP-0.3.2/MLStructFP/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-01-22 21:54:56.000000 MLStructFP-0.3.2/MLStructFP/_types.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.930000 MLStructFP-0.3.2/MLStructFP/db/
+-rw-rw-rw-   0        0        0      225 2023-01-16 00:38:24.000000 MLStructFP-0.3.2/MLStructFP/db/__init__.py
+-rw-rw-rw-   0        0        0     1505 2023-01-12 14:48:22.000000 MLStructFP-0.3.2/MLStructFP/db/_c.py
+-rw-rw-rw-   0        0        0     4692 2023-01-13 19:38:00.000000 MLStructFP-0.3.2/MLStructFP/db/_c_rect.py
+-rw-rw-rw-   0        0        0     3099 2023-01-12 14:48:22.000000 MLStructFP-0.3.2/MLStructFP/db/_c_slab.py
+-rw-rw-rw-   0        0        0     3031 2023-08-07 00:15:52.000000 MLStructFP-0.3.2/MLStructFP/db/_db_loader.py
+-rw-rw-rw-   0        0        0     6376 2023-08-07 00:13:18.000000 MLStructFP-0.3.2/MLStructFP/db/_floor.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.940000 MLStructFP-0.3.2/MLStructFP/db/image/
+-rw-rw-rw-   0        0        0      188 2023-01-16 00:38:24.000000 MLStructFP-0.3.2/MLStructFP/db/image/__init__.py
+-rw-rw-rw-   0        0        0     4121 2023-01-27 21:45:48.000000 MLStructFP-0.3.2/MLStructFP/db/image/_base.py
+-rw-rw-rw-   0        0        0     7732 2023-01-27 21:45:48.000000 MLStructFP-0.3.2/MLStructFP/db/image/_rect_binary.py
+-rw-rw-rw-   0        0        0    19312 2023-01-25 13:21:10.000000 MLStructFP-0.3.2/MLStructFP/db/image/_rect_photo.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.950000 MLStructFP-0.3.2/MLStructFP/utils/
+-rw-rw-rw-   0        0        0      215 2023-01-27 21:45:48.000000 MLStructFP-0.3.2/MLStructFP/utils/__init__.py
+-rw-rw-rw-   0        0        0    11693 2023-01-22 21:54:56.000000 MLStructFP-0.3.2/MLStructFP/utils/_geometry.py
+-rw-rw-rw-   0        0        0      867 2023-01-06 20:30:26.000000 MLStructFP-0.3.2/MLStructFP/utils/_mathlib.py
+-rw-rw-rw-   0        0        0      293 2023-01-27 21:45:48.000000 MLStructFP-0.3.2/MLStructFP/utils/_path.py
+-rw-rw-rw-   0        0        0     2824 2023-01-07 16:28:26.000000 MLStructFP-0.3.2/MLStructFP/utils/_plot.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.920000 MLStructFP-0.3.2/MLStructFP.egg-info/
+-rw-rw-rw-   0        0        0     8513 2023-08-07 00:41:16.000000 MLStructFP-0.3.2/MLStructFP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-08-07 00:41:16.000000 MLStructFP-0.3.2/MLStructFP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-07 00:41:16.000000 MLStructFP-0.3.2/MLStructFP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2023-08-07 00:41:16.000000 MLStructFP-0.3.2/MLStructFP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-07 00:41:16.000000 MLStructFP-0.3.2/MLStructFP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8513 2023-08-07 00:41:18.000000 MLStructFP-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7473 2023-08-07 00:40:38.000000 MLStructFP-0.3.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-07 00:41:18.000000 MLStructFP-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1770 2023-08-07 00:15:52.000000 MLStructFP-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-07 00:41:15.960000 MLStructFP-0.3.2/test/
+-rw-rw-rw-   0        0        0     3941 2023-08-07 00:38:48.000000 MLStructFP-0.3.2/test/test_db.py
```

### Comparing `MLStructFP-0.3.1/LICENSE` & `MLStructFP-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/__init__.py` & `MLStructFP-0.3.2/MLStructFP/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 """
 
 # Basic information
 __author__ = 'Pablo Pizarro R.'
 __description__ = 'Machine learning structural floor plan dataset'
 __keywords__ = ['ml', 'ai', 'dataset', 'calc', 'matrix analysis', 'cnn', 'structural analysis', 'structural design']
 __email__ = 'pablo@ppizarror.com'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 # URL
 __url__ = 'https://github.com/MLSTRUCT/MLSTRUCT_FP'
 __url_bug_tracker__ = 'https://github.com/MLSTRUCT/MLSTRUCT_FP/issues'
 __url_documentation__ = 'https://github.com/MLSTRUCT/MLSTRUCT_FP'
 __url_source_code__ = 'https://github.com/MLSTRUCT/MLSTRUCT_FP'
```

### Comparing `MLStructFP-0.3.1/MLStructFP/db/_c.py` & `MLStructFP-0.3.2/MLStructFP/db/_c.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/db/_c_rect.py` & `MLStructFP-0.3.2/MLStructFP/db/_c_rect.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/db/_c_slab.py` & `MLStructFP-0.3.2/MLStructFP/db/_c_slab.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/db/_db_loader.py` & `MLStructFP-0.3.2/MLStructFP/db/_db_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from MLStructFP.db._floor import Floor
 from MLStructFP.db._c_rect import Rect
 from MLStructFP.db._c_slab import Slab
 from MLStructFP._types import Tuple
 
 import json
 import os
+import tabulate
 
+from IPython.display import HTML, display
 from pathlib import Path
 from typing import Dict
 
 
 class DbLoader(object):
     """
     Dataset loader.
@@ -68,9 +70,26 @@
                     slab_id=int(slab_id),
                     floor=self.floor[slab_data['floorID']],
                     x=slab_data['x'],
                     y=slab_data['y']
                 )
 
     @property
-    def floors(self) -> Tuple['Floor']:
+    def floors(self) -> Tuple['Floor', ...]:
+        # noinspection PyTypeChecker
         return tuple(self.floor.values())
+
+    def tabulate(self) -> None:
+        """
+        Tabulates each floor, with their file and number of rects.
+        """
+        table = [['#', 'Floor ID', 'No. rects', 'Floor image path']]
+        for j in range(len(self.floors)):
+            f = self.floors[j]
+            table.append([j, f.id, len(f.rect), f.image_path])
+        display(HTML(tabulate.tabulate(
+            table,
+            headers='firstrow',
+            numalign='center',
+            stralign='center',
+            tablefmt='html'
+        )))
```

### Comparing `MLStructFP-0.3.1/MLStructFP/db/_floor.py` & `MLStructFP-0.3.2/MLStructFP/db/_floor.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/db/image/_base.py` & `MLStructFP-0.3.2/MLStructFP/db/image/_base.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/db/image/_rect_binary.py` & `MLStructFP-0.3.2/MLStructFP/db/image/_rect_binary.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/db/image/_rect_photo.py` & `MLStructFP-0.3.2/MLStructFP/db/image/_rect_photo.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/utils/_geometry.py` & `MLStructFP-0.3.2/MLStructFP/utils/_geometry.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/utils/_mathlib.py` & `MLStructFP-0.3.2/MLStructFP/utils/_mathlib.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP/utils/_plot.py` & `MLStructFP-0.3.2/MLStructFP/utils/_plot.py`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/MLStructFP.egg-info/SOURCES.txt` & `MLStructFP-0.3.2/MLStructFP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MLStructFP-0.3.1/setup.py` & `MLStructFP-0.3.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 # Load readme
 with open('README.rst') as f:
     long_description = f.read()
 
 # Load requirements
 requirements = [
+    'IPython == 8.12.2',
     'matplotlib == 3.5.3',
     'numpy == 1.18.5',
     'opencv-python == 4.5.1.48',
-    'Pillow == 9.4.0',
+    'Pillow == 9.5.0',
     'plotly == 5.11.0',
-    'requests == 2.28.1',
-    'six == 1.16.0'
+    'requests == 2.31.0',
+    'six == 1.16.0',
+    'tabulate == 0.9.0'
 ]
 
 # Setup library
 setup(
     author=MLStructFP.__author__,
     author_email=MLStructFP.__email__,
     classifiers=[
@@ -38,15 +40,15 @@
         'Topic :: Scientific/Engineering :: Visualization'
     ],
     description=MLStructFP.__description__,
     long_description=long_description,
     include_package_data=True,
     install_requires=requirements,
     extras_require={
-        'test': ['codecov', 'nose2']
+        'test': ['nose2[coverage_plugin]']
     },
     keywords=MLStructFP.__keywords__,
     name='MLStructFP',
     packages=find_packages(exclude=[
         '.idea',
         '.ipynb_checkpoints',
         'test'
```

### Comparing `MLStructFP-0.3.1/test/test_db.py` & `MLStructFP-0.3.2/test/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     def test_db_load(self) -> None:
         """
         Test db loader path and number of dataset items.
         """
         db = DbLoader(DB_PATH)
         self.assertEqual(os.path.dirname(DB_PATH), db._path)
+        db.tabulate()
 
         # Test floors
         self.assertEqual(len(db.floor), 7)
 
         # Test geometry of a given object
         f = db.floor[302]
         self.assertEqual(len(f.rect), 80)
```

