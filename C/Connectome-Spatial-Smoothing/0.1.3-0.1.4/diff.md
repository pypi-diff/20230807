# Comparing `tmp/Connectome_Spatial_Smoothing-0.1.3.tar.gz` & `tmp/Connectome_Spatial_Smoothing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Connectome_Spatial_Smoothing-0.1.3.tar", last modified: Thu May 26 15:34:20 2022, max compression
+gzip compressed data, was "Connectome_Spatial_Smoothing-0.1.4.tar", last modified: Mon Aug  7 10:31:11 2023, max compression
```

## Comparing `Connectome_Spatial_Smoothing-0.1.3.tar` & `Connectome_Spatial_Smoothing-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.586206 Connectome_Spatial_Smoothing-0.1.3/
--rw-rw-r--   0 sina      (1000) sina      (1000)     1072 2021-08-14 09:16:33.000000 Connectome_Spatial_Smoothing-0.1.3/LICENSE
--rw-rw-r--   0 sina      (1000) sina      (1000)      127 2022-05-26 14:25:14.000000 Connectome_Spatial_Smoothing-0.1.3/MANIFEST.in
--rw-rw-r--   0 sina      (1000) sina      (1000)     2613 2022-05-26 15:34:20.586206 Connectome_Spatial_Smoothing-0.1.3/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)     2034 2022-02-05 07:54:42.000000 Connectome_Spatial_Smoothing-0.1.3/README.md
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.582206 Connectome_Spatial_Smoothing-0.1.3/code/
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.582206 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/
--rw-rw-r--   0 sina      (1000) sina      (1000)    30415 2022-05-26 15:20:08.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/CSS.py
--rwxrwxrwx   0 sina      (1000) sina      (1000)        0 2020-02-04 08:25:01.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/__init__.py
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.582206 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.582206 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.582206 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/atlas/
--rwxrwxrwx   0 sina      (1000) sina      (1000)   621936 2019-12-18 02:18:51.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/atlas/Glasser360.32k_fs_LR.dlabel.nii
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.586206 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/cifti/
--rwxrwxrwx   0 sina      (1000) sina      (1000)   995912 2018-11-12 22:40:58.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/cifti/ones.dscalar.nii
-drwxrwxr-x   0 sina      (1000) sina      (1000)        0 2022-05-26 15:34:20.582206 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/
--rw-rw-r--   0 sina      (1000) sina      (1000)     2613 2022-05-26 15:34:20.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/PKG-INFO
--rw-rw-r--   0 sina      (1000) sina      (1000)      583 2022-05-26 15:34:20.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/SOURCES.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)        1 2022-05-26 15:34:20.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/dependency_links.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)       34 2022-05-26 15:34:20.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/requires.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)       29 2022-05-26 15:34:20.000000 Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/top_level.txt
--rw-rw-r--   0 sina      (1000) sina      (1000)      104 2021-11-28 03:09:41.000000 Connectome_Spatial_Smoothing-0.1.3/pyproject.toml
--rw-rw-r--   0 sina      (1000) sina      (1000)       38 2022-05-26 15:34:20.586206 Connectome_Spatial_Smoothing-0.1.3/setup.cfg
--rw-rw-r--   0 sina      (1000) sina      (1000)     1012 2022-05-26 15:33:42.000000 Connectome_Spatial_Smoothing-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.021989 Connectome_Spatial_Smoothing-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/
+-rw-r--r--   0 runner    (1001) docker     (123)    31856 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/CSS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/atlas/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   621936 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/atlas/Glasser360.32k_fs_LR.dlabel.nii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/cifti/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   995912 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/cifti/ones.dscalar.nii
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 10:31:11.017989 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-07 10:31:10.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-07 10:31:10.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 10:31:10.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-07 10:31:10.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-07 10:31:10.000000 Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-07 10:31:11.021989 Connectome_Spatial_Smoothing-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-07 10:31:00.000000 Connectome_Spatial_Smoothing-0.1.4/setup.py
```

### Comparing `Connectome_Spatial_Smoothing-0.1.3/LICENSE` & `Connectome_Spatial_Smoothing-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Connectome_Spatial_Smoothing-0.1.3/PKG-INFO` & `Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Connectome_Spatial_Smoothing
-Version: 0.1.3
+Name: Connectome-Spatial-Smoothing
+Version: 0.1.4
 Summary: Connectome Spatial Smoothing
 Home-page: https://github.com/sina-mansour/connectome-spatial-smoothing
 Author: Sina Mansour L.
 Author-email: sina.mansour.lakouraj@gmail.com
 Project-URL: Bug Tracker, https://github.com/sina-mansour/connectome-spatial-smoothing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,10 +52,24 @@
 
 Then, you could simply use the package in your own code after importing:
 
 `from Connectome_Spatial_Smoothing import CSS as css`
 
 ---
 
+## Usage notes
+
+### Verbosity:
+
+By default CSS scripts print out a bunch of logs that may or may not be of interest to you. If you like to disable the logs, simply add the following script:
+
+`css._verbose = False`
+
+---
+
 We have provided a short jupyter notebook showcasing all the functionalities described above. You may use the following link to open [this notebook](https://github.com/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb) in an interactive google colab session:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb)
+
+Note: there has been a new release with added functionality that is explained in the following interactive notebook:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example-v.0.1.3.ipynb)
```

### Comparing `Connectome_Spatial_Smoothing-0.1.3/README.md` & `Connectome_Spatial_Smoothing-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -37,10 +37,24 @@
 
 Then, you could simply use the package in your own code after importing:
 
 `from Connectome_Spatial_Smoothing import CSS as css`
 
 ---
 
+## Usage notes
+
+### Verbosity:
+
+By default CSS scripts print out a bunch of logs that may or may not be of interest to you. If you like to disable the logs, simply add the following script:
+
+`css._verbose = False`
+
+---
+
 We have provided a short jupyter notebook showcasing all the functionalities described above. You may use the following link to open [this notebook](https://github.com/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb) in an interactive google colab session:
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb)
+
+Note: there has been a new release with added functionality that is explained in the following interactive notebook:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example-v.0.1.3.ipynb)
```

### Comparing `Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/CSS.py` & `Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/CSS.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import gdist
 import multiprocessing as mp
 
 
 _main_dir = os.path.abspath(os.path.dirname(__file__))
 _sample_cifti_dscalar = os.path.join(_main_dir, 'data/templates/cifti/ones.dscalar.nii')
 _glasser_cifti = os.path.join(_main_dir, 'data/templates/atlas/Glasser360.32k_fs_LR.dlabel.nii')
+_verbose=True
 
 
 def _join_path(*args):
     return os.path.join(*args)
 
 
 def _write_sparse(sp_obj, file_path):
@@ -49,20 +50,21 @@
     if mode == 'raw':
         return time.time()
     if mode == 'abs':
         return time.asctime(time.localtime(time.time()))
 
 
 def _print_log(message, mode='info'):
-    if mode == 'info':
-        print ('{}: \033[0;32m[INFO]\033[0m {}'.format(_time_str(), message))
-    if mode == 'err':
-        print ('{}: \033[0;31m[ERROR]\033[0m {}'.format(_time_str(), message))
-        quit()
-    sys.stdout.flush()
+    if _verbose:
+        if mode == 'info':
+            print ('{}: \033[0;32m[INFO]\033[0m {}'.format(_time_str(), message))
+        if mode == 'err':
+            print ('{}: \033[0;31m[ERROR]\033[0m {}'.format(_time_str(), message))
+            quit()
+        sys.stdout.flush()
 
 
 def _handle_process_with_que(que, func, args, kwds):
     que.put(func(*args, **kwds))
 
 
 def _get_sample_cifti_dscalar():
@@ -202,15 +204,15 @@
         surface_labels = surface_labels[:cortical_vertices_count]
 
     labels = [x for x in list(set(surface_labels)) if x != 'Unlabeled']
     labels.sort()
 
     label_dict = {x: i for (i, x) in enumerate(labels)}
 
-    parcellation_matrix = np.zeros((len(labels), cortical_vertices_count))
+    parcellation_matrix = np.zeros((len(labels), len(surface_labels)))
 
     for (i, x) in enumerate(surface_labels):
         parcellation_matrix[label_dict[x], i] = 1
 
     return labels, sparse.csr_matrix(parcellation_matrix)
 
 
@@ -597,34 +599,42 @@
 
 
 def _get_half_incidence_matrices_from_endpoint_distances(start_dists,
                                                          start_indices,
                                                          end_dists,
                                                          end_indices,
                                                          node_count,
-                                                         threshold):
+                                                         threshold,
+                                                         weights=None):
     """
     Returns two half incidence matrices in a sparse format (CSR) after
     filtering the streamlines that are far (>2mm) from their closest vertex.
     """
+
+    if weights is None:
+        weights = np.ones(len(start_dists))
+    elif (type(weights) == str):
+        # load text file contents (this could be sift weights files generated by mrtrix)
+        weights = np.genfromtxt(weights)
+
     # mask points that are further than the threshold from all surface coordinates
     outlier_mask = (start_dists > threshold) | (end_dists > threshold)
     _print_log('outliers located: #{} outliers ({}%, with threshold {}mm)'.format(
         sum(outlier_mask),
         (100 * sum(outlier_mask)) / len(outlier_mask),
         threshold,
     ))
 
     # create a sparse incidence matrix
     _print_log('creating sparse incidence matrix')
     start_dict = {}
     end_dict = {}
     indices = (i for i in range(len(outlier_mask)) if not outlier_mask[i])
     for l, i in enumerate(indices):
-        start_dict[(start_indices[i], l)] = start_dict.get((start_indices[i], l), 0) + 1
+        start_dict[(start_indices[i], l)] = start_dict.get((start_indices[i], l), 0) + weights[i]
         end_dict[(end_indices[i], l)] = end_dict.get((end_indices[i], l), 0) + 1
 
     start_inc_mat = sparse.dok_matrix(
         (
             node_count,
             (len(outlier_mask) - outlier_mask.sum())
         ),
@@ -646,29 +656,35 @@
         end_inc_mat[key] = end_dict[key]
 
     _print_log('sparse matrix generated')
 
     return (start_inc_mat.tocsr(), end_inc_mat.tocsr())
 
 
-def _get_adjacency_from_half_incidence_matrices(U, V):
+def _get_adjacency_from_half_incidence_matrices(U, V, stat='sum'):
     """
     return a sparse adjacency matrix A from the two halfs of incidence matrix U & V.
     """
     A = U.dot(V.T)
+    if stat == 'mean':
+        # compute average instead of sum
+        A_div = (U != 0).astype(int).dot(((V != 0).astype(int)).T)
+        A.data = A.data / A_div.data
     return A + A.T
 
 
 def map_high_resolution_structural_connectivity(track_file,
                                                 left_surface_file,
                                                 right_surface_file,
                                                 warp_file=None,
                                                 threshold=2,
                                                 subcortex=False,
-                                                cifti_file=_sample_cifti_dscalar,):
+                                                cifti_file=_sample_cifti_dscalar,
+                                                weights=None,
+                                                stat='sum'):
     """
     Map the high-resolution structural connectivity matrix from tractography outputs.
 
     Args:
 
         track_file: The tractography file to map connectivity from (tck format)
 
@@ -685,30 +701,41 @@
         subcortex: [optional, default: False] A flag to indicate whether subcortical and cerebellar
                    voxels should also be included in the high-resolution connectivity map.
 
         cifti_file: [optional, default: HCP-YA template] Path to a cifti file, this template is used
                     to determine the high-resolution structure to exclude the medial wall and potentially
                     integrate subcortical volume.
 
+        weights: [optional] A numpy vector with the length of number of streamlines, or a file path
+                 pointing to a per-streamline weights file (such as the files generated by mrtrix's
+                 tcksift2). If this file is provided, then the weights are used to adjust the 
+                 contribution of every streamline to the connectivity matrix.
+        stat: [optional, default='sum'] Either 'sum', or 'mean'. If sum, the values will be added up
+              over all streamlines. Otherwise an average is computed over all streamline weights.
+              combination of stat='mean' with a list of per-streamline lengths could be used to compute
+              a mean distance connectivity matrix.
+
     Returns:
 
         connectome: The high-resolution structural connectome in a sparse csr format.
     """
     return _get_adjacency_from_half_incidence_matrices(
         *_get_half_incidence_matrices_from_endpoint_distances(
             *_get_endpoint_distances_from_tractography(
                 track_file,
                 left_surface_file,
                 right_surface_file,
                 cifti_file,
                 warp_file,
                 subcortex=subcortex,
             ),
-            threshold=threshold
-        )
+            threshold=threshold,
+            weights=weights
+        ),
+        stat=stat
     )
 
 
 def downsample_high_resolution_structural_connectivity_to_atlas(high_resolution_connectome,
                                                                 parcellation):
     """
     Downsample the high-resolution structural connectivity matrix to the resolution of a brain atlas.
```

### Comparing `Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/atlas/Glasser360.32k_fs_LR.dlabel.nii` & `Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/atlas/Glasser360.32k_fs_LR.dlabel.nii`

 * *Files identical despite different names*

### Comparing `Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing/data/templates/cifti/ones.dscalar.nii` & `Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing/data/templates/cifti/ones.dscalar.nii`

 * *Files identical despite different names*

### Comparing `Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/PKG-INFO` & `Connectome_Spatial_Smoothing-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Connectome-Spatial-Smoothing
-Version: 0.1.3
+Name: Connectome_Spatial_Smoothing
+Version: 0.1.4
 Summary: Connectome Spatial Smoothing
 Home-page: https://github.com/sina-mansour/connectome-spatial-smoothing
 Author: Sina Mansour L.
 Author-email: sina.mansour.lakouraj@gmail.com
 Project-URL: Bug Tracker, https://github.com/sina-mansour/connectome-spatial-smoothing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -52,10 +52,24 @@
 
 Then, you could simply use the package in your own code after importing:
 
 `from Connectome_Spatial_Smoothing import CSS as css`
 
 ---
 
+## Usage notes
+
+### Verbosity:
+
+By default CSS scripts print out a bunch of logs that may or may not be of interest to you. If you like to disable the logs, simply add the following script:
+
+`css._verbose = False`
+
+---
+
 We have provided a short jupyter notebook showcasing all the functionalities described above. You may use the following link to open [this notebook](https://github.com/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb) in an interactive google colab session:
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example.ipynb)
+
+Note: there has been a new release with added functionality that is explained in the following interactive notebook:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sina-mansour/connectome-based-smoothing/blob/main/notebooks/example-v.0.1.3.ipynb)
```

### Comparing `Connectome_Spatial_Smoothing-0.1.3/code/Connectome_Spatial_Smoothing.egg-info/SOURCES.txt` & `Connectome_Spatial_Smoothing-0.1.4/code/Connectome_Spatial_Smoothing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Connectome_Spatial_Smoothing-0.1.3/setup.py` & `Connectome_Spatial_Smoothing-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 requirements = ["numpy", "scipy", "sklearn", "nibabel", "gdist"]
 
 setuptools.setup(
     name="Connectome_Spatial_Smoothing",
-    version="0.1.3",
+    version="0.1.4",
     author="Sina Mansour L.",
     author_email="sina.mansour.lakouraj@gmail.com",
     description="Connectome Spatial Smoothing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sina-mansour/connectome-spatial-smoothing",
     project_urls={
```

