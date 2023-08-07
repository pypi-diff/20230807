# Comparing `tmp/emobject-0.7.2.tar.gz` & `tmp/emobject-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emobject-0.7.2.tar", last modified: Wed Aug  2 21:30:26 2023, max compression
+gzip compressed data, was "emobject-0.7.3.tar", last modified: Mon Aug  7 20:38:32 2023, max compression
```

## Comparing `emobject-0.7.2.tar` & `emobject-0.7.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.492400 emobject-0.7.2/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-08-02 21:30:16.000000 emobject-0.7.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 21:30:26.492400 emobject-0.7.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3915 2023-08-02 21:30:16.000000 emobject-0.7.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.489400 emobject-0.7.2/emobject/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39593 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/core.py
--rw-rw-rw-   0 root         (0) root         (0)    15643 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/database.py
--rw-rw-rw-   0 root         (0) root         (0)    32512 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emexperiment.py
--rw-rw-rw-   0 root         (0) root         (0)    14806 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emimage.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emlayer.py
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emobject.py
--rw-rw-rw-   0 root         (0) root         (0)     6759 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/empublicaccess.py
--rw-rw-rw-   0 root         (0) root         (0)     9493 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/emroitools.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.491400 emobject-0.7.2/emobject/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    24229 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/io.py
--rw-rw-rw-   0 root         (0) root         (0)    11201 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/utils/visualization.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-02 21:30:16.000000 emobject-0.7.2/emobject/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 21:30:26.490400 emobject-0.7.2/emobject.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4312 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      559 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      229 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-08-02 21:30:26.000000 emobject-0.7.2/emobject.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-02 21:30:26.492400 emobject-0.7.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-08-02 21:30:16.000000 emobject-0.7.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 20:38:32.555159 emobject-0.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-08-07 20:38:22.000000 emobject-0.7.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-08-07 20:38:32.555159 emobject-0.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3915 2023-08-07 20:38:22.000000 emobject-0.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 20:38:32.552159 emobject-0.7.3/emobject/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39593 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    15643 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/database.py
+-rw-rw-rw-   0 root         (0) root         (0)    32512 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/emexperiment.py
+-rw-rw-rw-   0 root         (0) root         (0)    14806 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/emimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     9750 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/emlayer.py
+-rw-rw-rw-   0 root         (0) root         (0)    50335 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/emobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     6759 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/empublicaccess.py
+-rw-rw-rw-   0 root         (0) root         (0)     9493 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/emroitools.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 20:38:32.555159 emobject-0.7.3/emobject/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/utils/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/utils/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    11201 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/utils/visualization.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-07 20:38:22.000000 emobject-0.7.3/emobject/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 20:38:32.553160 emobject-0.7.3/emobject.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-08-07 20:38:32.000000 emobject-0.7.3/emobject.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-08-07 20:38:32.000000 emobject-0.7.3/emobject.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 20:38:32.000000 emobject-0.7.3/emobject.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      229 2023-08-07 20:38:32.000000 emobject-0.7.3/emobject.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-07 20:38:32.000000 emobject-0.7.3/emobject.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-07 20:38:32.555159 emobject-0.7.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-08-07 20:38:22.000000 emobject-0.7.3/setup.py
```

### Comparing `emobject-0.7.2/LICENSE` & `emobject-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/PKG-INFO` & `emobject-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.2
+Version: 0.7.3
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.2/README.md` & `emobject-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/core.py` & `emobject-0.7.3/emobject/core.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/database.py` & `emobject-0.7.3/emobject/database.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/emexperiment.py` & `emobject-0.7.3/emobject/emexperiment.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/emimage.py` & `emobject-0.7.3/emobject/emimage.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/emlayer.py` & `emobject-0.7.3/emobject/emlayer.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/emobject.py` & `emobject-0.7.3/emobject/emobject.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,35 +728,46 @@
             layer:  the layer to slice within.
                 If None, uses the active layer.
         Returns:
             Subsetted EMObject view
         """
         self._validate()
 
+        if layer is None:
+            layer = self._activelayer
+        else:
+            assert layer in self.ax
+
         if obs_subset is None:
-            obs_subset = self._obs_ax
+            obs_subset = self._layerdict[layer]._obs_ax
         if var_subset is None:
-            var_subset = self._var_ax
+            var_subset = self._layerdict[layer]._var_ax
         if type(obs_subset) == list:
             obs_subset = np.array(obs_subset)
         if type(var_subset) == list:
             var_subset = np.array(var_subset)
-        if layer is None:
-            layer = self._activelayer
-        else:
-            assert layer in self.ax
 
         if seg_subset is not None:
             assert seg_subset in np.unique(self.seg)
-            obs_subset, _ = np.where(self._seg == seg_subset)
+            all_r = set()
+            if type(seg_subset) == int:
+                seg_subset = [seg_subset]
+            for si in seg_subset:
+                rr, cc = np.where(self._layerdict[layer]._seg == si)
+                all_r.update(rr)
+            obs_subset = np.array(list(all_r))
+            obs_subset = self._layerdict[layer]._obs_ax[obs_subset]
 
         if mask is not None:
+            if self._layerdict[layer]._seg is None:
+                _ = self.seg
             assert mask in self.mask.mask_names
             ix, = np.where(self.mask.mask_names == mask)
-            obs_subset, _ = np.where(self._seg[:, ix] != 0)
+            obs_subset, _ = np.where(self._layerdict[layer]._seg[:, ix] != 0)
+            obs_subset = self._layerdict[layer]._obs_ax[obs_subset]
 
         pos_dict = {}
         for coord_sys in self._layerdict[layer]._pos.keys():
             pos_dict[coord_sys] = self._layerdict[layer]._pos[coord_sys].loc[obs_subset, :]
 
         # a view will return an in-memory EMObject that has been subsetted
         return EMObject(
@@ -770,29 +781,26 @@
             is_view=True
         )
 
     def slice(self,
               obs_subset: Optional[Union[np.ndarray, list]] = None,
               seg_subset: Optional[Union[np.ndarray, list, int]] = None,
               anchor_layer: Optional[str] = None,
-              layers: Optional[Union[str, list, np.ndarray]] = None,
-              lossy_threshold: Optional[float] = None) -> EMObject:
+              layers: Optional[Union[str, list, np.ndarray]] = None) -> EMObject:
 
         """
         Slices through all emObject layers on the basis of observations, variables, or masks
         and returns a new EMObject with the subsetted data.
 
         Args:
             obs_subset: subset of observations to include.
                 Elements must belong to obs_ax
             seg_subset: subset of segments to include.
                 Elements must belong to sobs_ax
             layers: the layers to slice within. If None, uses all.
-            lossy_threshold: when slicing from a higher resolution layer to a lower,
-                there is a loss of spatial resolution. T
         """
         self._validate()
 
         if layers is None:
             raise EMObjectException("Must specify layers to slice.")
         elif type(layers) == str:
             layers = [layers]
@@ -910,14 +918,24 @@
             np.ndarray: the observations in target layer for a given segment ID
         '''
         segment_to_cell_map = {}
 
         assert mask_name in self.mask.mask_names
         assert target_layer in self.layers
 
+        # Check that a segmentation mask exists for the target layer
+        if self._layerdict[target_layer].segmentation is None:
+            if 'segmentation_mask' in self.mask.mask_names:
+                warning(f"Automatically assigning mask `segmentation_mask` to {target_layer}.\
+                        To assign a different mask, use `E.set_layer_segmentation()`.")
+            else:
+                raise EMObjectException(f"No segmentation mask exists for {target_layer}.\
+                                        Please specify a segmentation mask for {target_layer}\
+                                        with `E.set_layer_segmentation().`")
+
         if isinstance(segment_id, int):
             segment_id = [segment_id]
 
         # Get the pixels that belong to the segment
         segment_mask = sparse.coo_matrix(self.mask.mloc(mask_name))
 
         for si in segment_id:
```

### Comparing `emobject-0.7.2/emobject/empublicaccess.py` & `emobject-0.7.3/emobject/empublicaccess.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/emroitools.py` & `emobject-0.7.3/emobject/emroitools.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/utils/graph.py` & `emobject-0.7.3/emobject/utils/graph.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/utils/helpers.py` & `emobject-0.7.3/emobject/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/utils/io.py` & `emobject-0.7.3/emobject/utils/io.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject/utils/visualization.py` & `emobject-0.7.3/emobject/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/emobject.egg-info/PKG-INFO` & `emobject-0.7.3/emobject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emobject
-Version: 0.7.2
+Version: 0.7.3
 Summary: data abstraction and libraries for spatial omics
 Home-page: https://gitlab.com/enable-medicine/rnd-subgroup/emobject/
 Author: Ethan A. G. Baker
 Author-email: ethan.baker@enablemedicine.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7, <4
```

### Comparing `emobject-0.7.2/emobject.egg-info/SOURCES.txt` & `emobject-0.7.3/emobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emobject-0.7.2/setup.py` & `emobject-0.7.3/setup.py`

 * *Files identical despite different names*

