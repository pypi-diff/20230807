# Comparing `tmp/xnemogcm-0.4.1.tar.gz` & `tmp/xnemogcm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnemogcm-0.4.1.tar", max compression
+gzip compressed data, was "xnemogcm-0.4.2.tar", max compression
```

## Comparing `xnemogcm-0.4.1.tar` & `xnemogcm-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-03-30 10:11:17.138321 xnemogcm-0.4.1/LICENSE
--rw-r--r--   0        0        0     3656 2023-03-30 10:11:17.138321 xnemogcm-0.4.1/README.md
--rw-r--r--   0        0        0      982 2023-03-30 10:11:17.142321 xnemogcm-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      242 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/__init__.py
--rw-r--r--   0        0        0     1300 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/arakawa_points.py
--rw-r--r--   0        0        0     6391 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/domcfg.py
--rw-r--r--   0        0        0     4454 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/merge.py
--rw-r--r--   0        0        0     4520 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/metrics.py
--rw-r--r--   0        0        0     1112 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/namelist.py
--rw-r--r--   0        0        0     8042 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/nemo.py
--rw-r--r--   0        0        0      468 2023-03-30 10:11:17.146321 xnemogcm-0.4.1/xnemogcm/test/conftest.py
--rw-r--r--   0        0        0     1195 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_dask.py
--rw-r--r--   0        0        0     3540 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_domcfg.py
--rw-r--r--   0        0        0     1856 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_merge.py
--rw-r--r--   0        0        0     2316 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_metrics.py
--rw-r--r--   0        0        0     1198 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_namelist.py
--rw-r--r--   0        0        0     4474 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_nemo.py
--rw-r--r--   0        0        0      373 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_surface.py
--rw-r--r--   0        0        0      461 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/test/test_version.py
--rw-r--r--   0        0        0     3361 2023-03-30 10:11:17.162321 xnemogcm-0.4.1/xnemogcm/tools.py
--rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 xnemogcm-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-07 10:10:50.714835 xnemogcm-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4097 2023-08-07 10:10:50.714835 xnemogcm-0.4.2/README.md
+-rw-r--r--   0        0        0      982 2023-08-07 10:10:50.718835 xnemogcm-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      242 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/__init__.py
+-rw-r--r--   0        0        0     1300 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/arakawa_points.py
+-rw-r--r--   0        0        0     7473 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/domcfg.py
+-rw-r--r--   0        0        0     4454 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/merge.py
+-rw-r--r--   0        0        0     4520 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/metrics.py
+-rw-r--r--   0        0        0     1112 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/namelist.py
+-rw-r--r--   0        0        0     8852 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/nemo.py
+-rw-r--r--   0        0        0      468 2023-08-07 10:10:50.722835 xnemogcm-0.4.2/xnemogcm/test/conftest.py
+-rw-r--r--   0        0        0     1195 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_dask.py
+-rw-r--r--   0        0        0     4148 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_domcfg.py
+-rw-r--r--   0        0        0     1856 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_merge.py
+-rw-r--r--   0        0        0     2316 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_metrics.py
+-rw-r--r--   0        0        0     1198 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_namelist.py
+-rw-r--r--   0        0        0     5317 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_nemo.py
+-rw-r--r--   0        0        0      764 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_surface.py
+-rw-r--r--   0        0        0      461 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/test/test_version.py
+-rw-r--r--   0        0        0     3361 2023-08-07 10:10:50.734835 xnemogcm-0.4.2/xnemogcm/tools.py
+-rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 xnemogcm-0.4.2/PKG-INFO
```

### Comparing `xnemogcm-0.4.1/LICENSE` & `xnemogcm-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/README.md` & `xnemogcm-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # xnemogcm
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5724577.svg)](https://doi.org/10.5281/zenodo.5724577)
+![ci](https://github.com/rcaneill/xnemogcm/actions/workflows/ci.yml/badge.svg)
+![pypi](https://badge.fury.io/py/xnemogcm.svg)
+![anaconda badge](https://anaconda.org/conda-forge/xnemogcm/badges/version.svg)
 
 Interface to open NEMO ocean global circulation model output dataset and create a xgcm grid.
 NEMO 3.6, 4.0, and 4.2.0 are tested and supported. Any version between 3.6 and 4.2.0 should work,
 but in case of trouble, [please open an issue](https://github.com/rcaneill/xnemogcm/issues).
 
 
 ## Usage
@@ -68,14 +71,19 @@
 Sources for the notebooks are located in `src_example`. This is where to add / modify the
 examples. A github action is set to automatically build the notebook according to
 the latest version of the code, and publish them to `example` when commiting to master branch.
 
 
 ## What's new
 
+### v0.4.2 (2023-08-07)
+* Allow additional dimension names occurring when variables on inner grid are diagnosed, e.g. `x_grid_U_inner` or `x_grid_U`.
+* Add coordinates into the DataArrays
+* Add some standard names and units in domcfg
+
 ### v0.4.1 (2023-03-29)
 * Allow to open files if time bounds are missing
 * Minor bug correction for nemo 3.6 
 * Add nemo 3.6 and 4.2.0 test data
 * Update code to support nemo 3.6 and 4.2.0
 
 ### v0.4.0 (2022-12-08)
```

### Comparing `xnemogcm-0.4.1/pyproject.toml` & `xnemogcm-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xnemogcm"
-version = "0.4.1"
+version = "0.4.2"
 description = "Interface to open NEMO global circulation model output dataset and create a xgcm grid."
 license = "MIT"
 homepage = "https://github.com/rcaneill/xnemogcm"
 authors = ["Romain Caneill <romain.caneill@gu.se>"]
 readme = "README.md"
 exclude = ["xnemogcm/test/data"]
```

### Comparing `xnemogcm-0.4.1/xnemogcm/arakawa_points.py` & `xnemogcm-0.4.2/xnemogcm/arakawa_points.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/domcfg.py` & `xnemogcm-0.4.2/xnemogcm/domcfg.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,42 @@
 import numpy as np
 import xarray as xr
 
 from . import arakawa_points as akp
 from .tools import get_domcfg_points, _dir_or_files_to_files
 
 
+def _add_cf(domcfg):
+    """
+    Add cf standard_name and units when possible
+    """
+    for i in domcfg.variables:
+        if "glam" in i:
+            domcfg[i].attrs.update(
+                {"standard_name": "longitude", "units": "degrees_east"}
+            )
+        if "gphi" in i:
+            domcfg[i].attrs.update(
+                {"standard_name": "latitude", "units": "degrees_north"}
+            )
+        if "gdep" in i:
+            domcfg[i].attrs.update(
+                {"standard_name": "depth", "units": "m", "positive": "down"}
+            )
+        if "e1" in i or "e2" in i:
+            domcfg[i].attrs.update({"units": "m"})
+        if "e3" in i:
+            domcfg[i].attrs.update({"standard_name": "cell_thickness", "units": "m"})
+        if i in ["ff", "ff_f", "ff_t"]:
+            domcfg[i].attrs.update(
+                {"standard_name": "coriolis_parameter", "units": "s-1"}
+            )
+    return domcfg
+
+
 def domcfg_preprocess(ds):
     """
     Preprocess domcfg / meshmask files when needed to be recombined (= 1 file per processor)
     """
     # nemo 3.6
     if "z" in ds or "z" in ds.dims or "z" in ds.coords:
         ds = ds.swap_dims({"z": "nav_lev"})
@@ -193,8 +221,12 @@
     for coord in coordinates:
         domcfg = domcfg.drop_dims(coord, errors="ignore").drop_vars(
             coord, errors="ignore"
         )
     # adding variables as coordinates
     if add_coordinates:
         domcfg = _add_coordinates(domcfg)
+    # Remove nav_lon and nav_lat
+    domcfg = domcfg.drop_vars(["nav_lon", "nav_lat"], errors="ignore")
+    # Add cf
+    domcfg = _add_cf(domcfg)
     return domcfg
```

### Comparing `xnemogcm-0.4.1/xnemogcm/merge.py` & `xnemogcm-0.4.2/xnemogcm/merge.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/metrics.py` & `xnemogcm-0.4.2/xnemogcm/metrics.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/namelist.py` & `xnemogcm-0.4.2/xnemogcm/namelist.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/nemo.py` & `xnemogcm-0.4.2/xnemogcm/nemo.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,17 +77,26 @@
     point = akp.Point(point_type)
     # get the name of the depth variable e.g. deptht, depthu, etc
     try:
         z_nme = [i for i in ds.dims.keys() if "depth" in i][0]
     except IndexError:
         # This means that there is no depth dependence of the data (surface data)
         z_nme = None
-    x_nme = "x"
-    y_nme = "y"
-    to_rename.update({x_nme: point.x, y_nme: point.y})
+
+    # get the name of the dimension along i e.g. x, x_grid_U, x_grid_U_inner etc
+    x_nme = [i for i in ds.dims.keys() if "x_grid" in i or i == "x"]
+    # get the name of the dimension along j e.g. y, y_grid_U, y_grid_U_inner etc
+    y_nme = [i for i in ds.dims.keys() if "y_grid" in i or i == "y"]
+
+    for x in x_nme:
+        to_rename.update({x: point.x})
+
+    for y in y_nme:
+        to_rename.update({y: point.y})
+
     points = [point.x, point.y]
     if z_nme:
         to_rename.update({z_nme: point.z})
         points += [point.z]
 
     ds = ds.drop_vars(
         ["nav_lat", "nav_lon"],
@@ -101,14 +110,27 @@
     else:
         to_rename.update({"time_counter": "t"})
     ds = ds.rename(to_rename)
     if time_b:
         ds["t"].attrs["bounds"] = "t_bounds"
     # setting z_c/z_f/x_c/etc to be the same as in domcfg
     ds = ds.assign_coords({i: domcfg[i] for i in points})
+    # Assign the proper coordinates
+    # 1st case: horizontal
+    if z_nme:
+        p = set(points[:2])
+    else:
+        p = set(points)
+    coords = [i for i in domcfg.coords if set(domcfg.coords[i].dims) == p]
+    ds = ds.assign_coords({i: domcfg[i] for i in coords})
+    # 2nd case vertical
+    if z_nme:
+        p = set(points)
+        coords = [i for i in domcfg.coords if set(domcfg.coords[i].dims) == p]
+        ds = ds.assign_coords({i: domcfg[i] for i in coords})
     return ds
 
 
 def _check_position(ds, position, parallel=False):
     if position is not None:
         return position
     else:
```

### Comparing `xnemogcm-0.4.1/xnemogcm/test/test_dask.py` & `xnemogcm-0.4.2/xnemogcm/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/test/test_domcfg.py` & `xnemogcm-0.4.2/xnemogcm/test/test_domcfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,7 +96,28 @@
 
 
 def test_compare_domcfg_mesh_mask(data_path):
     """Test that the data of mesh_mask are the same as in domain_cfg_out"""
     domcfg_1 = open_domain_cfg(datadir=(data_path / "mesh_mask_1_file"))
     domcfg_multi = open_domain_cfg(datadir=(data_path / "mesh_mask_multi_files"))
     assert (domcfg_1 == domcfg_multi).all()
+
+
+def test_coordinates_horizontal(data_path):
+    """Test that coordinates are added to nemo files"""
+    domcfg = open_domain_cfg(
+        datadir=data_path / "mesh_mask_1_file",
+    )
+    assert "glamt" in domcfg.e1t.coords
+    if "ff_f" in domcfg:
+        assert "glamf" in domcfg.ff_f.coords
+    else:
+        # NEMO 3.6
+        assert "glamf" in domcfg.ff.coords
+
+
+def test_attributes(data_path):
+    """Test that coordinates are added to nemo files"""
+    domcfg = open_domain_cfg(
+        datadir=data_path / "mesh_mask_1_file",
+    )
+    assert domcfg.glamt.attrs.get("standard_name") == "longitude"
```

### Comparing `xnemogcm-0.4.1/xnemogcm/test/test_merge.py` & `xnemogcm-0.4.2/xnemogcm/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/test/test_metrics.py` & `xnemogcm-0.4.2/xnemogcm/test/test_metrics.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/test/test_namelist.py` & `xnemogcm-0.4.2/xnemogcm/test/test_namelist.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/xnemogcm/test/test_nemo.py` & `xnemogcm-0.4.2/xnemogcm/test/test_nemo.py`

 * *Files 14% similar despite different names*

```diff
@@ -142,7 +142,36 @@
         datadir=data_path / "mesh_mask_1_file",
     )
     ds_raw = xr.open_dataset(data_path / "nemo/GYRE_1y_00010101_00011230_grid_T.nc")
     ds_raw.encoding["source"] = "GYRE_1y_00010101_00011230_grid_T.nc"
     ds = nemo_preprocess(ds_raw, domcfg)
     assert "x_c" in ds
     assert "t" in ds
+
+
+def test_coordinates_horizontal(data_path):
+    """Test that coordinates are added to nemo files"""
+    domcfg = open_domain_cfg(
+        datadir=data_path / "mesh_mask_1_file",
+    )
+    nemo_ds = open_nemo(
+        datadir=data_path / "nemo",
+        domcfg=domcfg,
+    )
+    assert "glamt" in nemo_ds.toce.coords
+    assert "glamu" in nemo_ds.uoce.coords
+
+
+def test_coordinates_vertical(data_path, request):
+    """Test that coordinates are added to nemo files"""
+    if request.node.callspec.id == "3.6":
+        pytest.xfail(
+            "Failing for nemo <= 3.6 as gdept_0 and gdepw_0 are not in mesh mask"
+        )
+    domcfg = open_domain_cfg(
+        datadir=data_path / "mesh_mask_1_file",
+    )
+    nemo_ds = open_nemo(
+        datadir=data_path / "nemo",
+        domcfg=domcfg,
+    )
+    assert "gdept_0" in nemo_ds.toce.coords
```

### Comparing `xnemogcm-0.4.1/xnemogcm/tools.py` & `xnemogcm-0.4.2/xnemogcm/tools.py`

 * *Files identical despite different names*

### Comparing `xnemogcm-0.4.1/PKG-INFO` & `xnemogcm-0.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnemogcm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Interface to open NEMO global circulation model output dataset and create a xgcm grid.
 Home-page: https://github.com/rcaneill/xnemogcm
 License: MIT
 Author: Romain Caneill
 Author-email: romain.caneill@gu.se
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,17 @@
 Requires-Dist: xarray (>=0.21.1)
 Requires-Dist: xgcm (>=0.6.0) ; extra == "metrics"
 Description-Content-Type: text/markdown
 
 # xnemogcm
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5724577.svg)](https://doi.org/10.5281/zenodo.5724577)
+![ci](https://github.com/rcaneill/xnemogcm/actions/workflows/ci.yml/badge.svg)
+![pypi](https://badge.fury.io/py/xnemogcm.svg)
+![anaconda badge](https://anaconda.org/conda-forge/xnemogcm/badges/version.svg)
 
 Interface to open NEMO ocean global circulation model output dataset and create a xgcm grid.
 NEMO 3.6, 4.0, and 4.2.0 are tested and supported. Any version between 3.6 and 4.2.0 should work,
 but in case of trouble, [please open an issue](https://github.com/rcaneill/xnemogcm/issues).
 
 
 ## Usage
@@ -92,14 +95,19 @@
 Sources for the notebooks are located in `src_example`. This is where to add / modify the
 examples. A github action is set to automatically build the notebook according to
 the latest version of the code, and publish them to `example` when commiting to master branch.
 
 
 ## What's new
 
+### v0.4.2 (2023-08-07)
+* Allow additional dimension names occurring when variables on inner grid are diagnosed, e.g. `x_grid_U_inner` or `x_grid_U`.
+* Add coordinates into the DataArrays
+* Add some standard names and units in domcfg
+
 ### v0.4.1 (2023-03-29)
 * Allow to open files if time bounds are missing
 * Minor bug correction for nemo 3.6 
 * Add nemo 3.6 and 4.2.0 test data
 * Update code to support nemo 3.6 and 4.2.0
 
 ### v0.4.0 (2022-12-08)
```

