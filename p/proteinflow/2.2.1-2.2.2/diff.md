# Comparing `tmp/proteinflow-2.2.1.tar.gz` & `tmp/proteinflow-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-2.2.1.tar", last modified: Thu Aug  3 16:32:24 2023, max compression
+gzip compressed data, was "proteinflow-2.2.2.tar", last modified: Mon Aug  7 17:31:52 2023, max compression
```

## Comparing `proteinflow-2.2.1.tar` & `proteinflow-2.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 16:32:10.000000 proteinflow-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-03 16:32:24.854595 proteinflow-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-03 16:32:10.000000 proteinflow-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 16:32:10.000000 proteinflow-2.2.1/dev/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 16:32:10.000000 proteinflow-2.2.1/dev/update_init_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow/data/
--rw-r--r--   0 runner    (1001) docker     (123)    74235 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43477 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/data/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow/download/
--rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/download/boto.py
--rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/ligand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/processing/
--rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/proteinflow/split/
--rw-r--r--   0 runner    (1001) docker     (123)    50805 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/split/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/split/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-08-03 16:32:10.000000 proteinflow-2.2.1/proteinflow/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.850595 proteinflow-2.2.1/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-03 16:32:24.000000 proteinflow-2.2.1/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-03 16:32:10.000000 proteinflow-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-03 16:32:24.854595 proteinflow-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:32:24.854595 proteinflow-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_ligands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-03 16:32:10.000000 proteinflow-2.2.1/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-07 17:31:41.000000 proteinflow-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-07 17:31:52.477350 proteinflow-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-08-07 17:31:41.000000 proteinflow-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.473350 proteinflow-2.2.2/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-07 17:31:41.000000 proteinflow-2.2.2/dev/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-07 17:31:41.000000 proteinflow-2.2.2/dev/update_init_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.473350 proteinflow-2.2.2/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.473350 proteinflow-2.2.2/proteinflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    74235 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44386 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/data/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/proteinflow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    24607 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/download/boto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36587 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/ligand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/proteinflow/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/proteinflow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    19390 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/proteinflow/split/
+-rw-r--r--   0 runner    (1001) docker     (123)    50805 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/split/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-08-07 17:31:41.000000 proteinflow-2.2.2/proteinflow/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.473350 proteinflow-2.2.2/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-08-07 17:31:52.000000 proteinflow-2.2.2/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-08-07 17:31:52.000000 proteinflow-2.2.2/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-07 17:31:52.000000 proteinflow-2.2.2/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-07 17:31:52.000000 proteinflow-2.2.2/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-07 17:31:52.000000 proteinflow-2.2.2/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-07 17:31:52.000000 proteinflow-2.2.2/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-07 17:31:41.000000 proteinflow-2.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-07 17:31:52.477350 proteinflow-2.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-07 17:31:52.477350 proteinflow-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-07 17:31:41.000000 proteinflow-2.2.2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-07 17:31:41.000000 proteinflow-2.2.2/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-07 17:31:41.000000 proteinflow-2.2.2/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-07 17:31:41.000000 proteinflow-2.2.2/tests/test_ligands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-07 17:31:41.000000 proteinflow-2.2.2/tests/test_sabdab.py
```

### Comparing `proteinflow-2.2.1/LICENSE` & `proteinflow-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/PKG-INFO` & `proteinflow-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.2.1
+Version: 2.2.2
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.2.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.2.2 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.2.1/README.md` & `proteinflow-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/dev/bump_version.py` & `proteinflow-2.2.2/dev/bump_version.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/dev/update_init_docs.py` & `proteinflow-2.2.2/dev/update_init_docs.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/__init__.py` & `proteinflow-2.2.2/proteinflow/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/cli.py` & `proteinflow-2.2.2/proteinflow/cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/constants.py` & `proteinflow-2.2.2/proteinflow/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     "VAL": "V",
     "GLU": "E",
     "TYR": "Y",
     "MET": "M",
 }
 
 REVERSE_D3TO1 = {v: k for k, v in D3TO1.items()}
+REVERSE_D3TO1["-"] = "GLY"
 REVERSE_D3TO1["X"] = "GLY"
 
 ALPHABET = "-ACDEFGHIKLMNPQRSTVWY"
 
 FEATURES_DICT = defaultdict(lambda: defaultdict(lambda: 0))
 FEATURES_DICT["hydropathy"].update(
     {
```

### Comparing `proteinflow-2.2.1/proteinflow/data/__init__.py` & `proteinflow-2.2.2/proteinflow/data/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/data/torch.py` & `proteinflow-2.2.2/proteinflow/data/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,15 @@
         classes_dict_path=None,
         cut_edges=False,
         mask_residues=True,
         lower_limit=15,
         upper_limit=100,
         mask_frac=None,
         mask_whole_chains=False,
+        mask_sequential=False,
         force_binding_sites_frac=0.15,
         mask_all_cdrs=False,
         load_ligands=False,
         pyg_graph=False,
         patch_around_mask=False,
         initial_patch_size=128,
         antigen_patch_size=128,
@@ -346,14 +347,17 @@
             the lower limit of the number of residues to mask
         upper_limit : int, default 100
             the upper limit of the number of residues to mask
         mask_frac : float, optional
             if given, the number of residues to mask is `mask_frac` times the length of the chain
         mask_whole_chains : bool, default False
             if `True`, the whole chain is masked
+        mask_sequential : bool, default False
+            if `True`, the masked residues will be neighbors in the sequence; otherwise a geometric
+            mask is applied based on the coordinates
         force_binding_sites_frac : float, default 0.15
             if `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
             from a polymer is sampled, the center of the masked region will be forced to be in a binding site (in PDB datasets)
         mask_all_cdrs : bool, default False
             if `True`, all CDRs will be masked (in SAbDab datasets)
         load_ligands : bool, default False
             if `True`, the ligands will be loaded as well
@@ -385,14 +389,15 @@
         self.force_binding_sites_frac = force_binding_sites_frac
         self.mask_all_cdrs = mask_all_cdrs
         self.load_ligands = load_ligands
         self.pyg_graph = pyg_graph
         self.patch_around_mask = patch_around_mask
         self.initial_patch_size = initial_patch_size
         self.antigen_patch_size = antigen_patch_size
+        self.mask_sequential = mask_sequential
         self.feature_types = []
         if node_features_type is not None:
             self.feature_types = node_features_type.split("+")
         self.entry_type = entry_type
         self.shuffle_clusters = shuffle_clusters
         self.feature_functions = {
             "sidechain_orientation": self._sidechain,
@@ -536,14 +541,17 @@
         """Get the mask for the residues that need to be predicted.
 
         Depending on the parameters the residues are selected as follows:
         - if `mask_whole_chains` is `True`, the whole chain is masked
         - if `mask_frac` is given, the number of residues to mask is `mask_frac` times the length of the chain,
         - otherwise, the number of residues to mask is sampled uniformly from the range [`lower_limit`, `upper_limit`].
 
+        If `mask_sequential` is `True`, the residues are masked based on the order in the sequence, otherwise a
+        spherical mask is applied based on the coordinates.
+
         If `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
         from a polymer is sampled, the center of the masked region will be forced to be in a binding site.
 
         Parameters
         ----------
         data : dict
             an entry generated by `ProteinDataset`
@@ -620,21 +628,26 @@
                     k = int(len(neighbor_indices) * self.mask_frac)
                 else:
                     up = min(
                         self.upper_limit, int(len(neighbor_indices) * 0.5)
                     )  # do not mask more than half of the sequence
                     low = min(up - 1, self.lower_limit)
                     k = random.choice(range(low, up))
-                dist = torch.norm(
-                    chain[neighbor_indices, 2, :] - res_coords.unsqueeze(0), dim=-1
-                )
-                closest_indices = neighbor_indices[
-                    torch.topk(dist, k, largest=False)[1]
-                ]
-                chain_M[closest_indices + chain_start] = 1
+                if self.mask_sequential:
+                    start = max(0, res_i - k // 2)
+                    end = min(len(chain), res_i + k // 2)
+                    chain_M[chain_start + start : chain_start + end] = 1
+                else:
+                    dist = torch.norm(
+                        chain[neighbor_indices, 2, :] - res_coords.unsqueeze(0), dim=-1
+                    )
+                    closest_indices = neighbor_indices[
+                        torch.topk(dist, k, largest=False)[1]
+                    ]
+                    chain_M[closest_indices + chain_start] = 1
         return chain_M
 
     def _dihedral(self, data_entry, chains):
         """Return dihedral angles."""
         return data_entry.dihedral_angles(chains)
 
     def _sidechain(self, data_entry, chains):
@@ -872,16 +885,20 @@
                 mask[chain_mask] = True
         return mask
 
     def _patch(self, data):
         """Cut the data around the anchor residues."""
         # adapted from diffab
         pos_alpha = data["X"][:, 2]
-        anchor_ind = self.get_anchor_ind(data["masked_res"], data["mask"])
-        anchor_points = torch.stack([pos_alpha[ind] for ind in anchor_ind], dim=0)
+        if self.mask_whole_chains:
+            mask_ = (data["mask"] * data["masked_res"]).bool()
+            anchor_points = pos_alpha[mask_].mean(0).unsqueeze(0)
+        else:
+            anchor_ind = self.get_anchor_ind(data["masked_res"], data["mask"])
+            anchor_points = torch.stack([pos_alpha[ind] for ind in anchor_ind], dim=0)
         dist_anchor = torch.cdist(pos_alpha, anchor_points, p=2).min(dim=1)[0]  # (L, )
         dist_anchor[~data["mask"].bool()] = float("+inf")
         initial_patch_idx = torch.topk(
             dist_anchor,
             k=min(self.initial_patch_size, dist_anchor.size(0)),
             largest=False,
             sorted=True,
```

### Comparing `proteinflow-2.2.1/proteinflow/data/utils.py` & `proteinflow-2.2.2/proteinflow/data/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/download/__init__.py` & `proteinflow-2.2.2/proteinflow/download/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/download/boto.py` & `proteinflow-2.2.2/proteinflow/download/boto.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/ligand.py` & `proteinflow-2.2.2/proteinflow/ligand.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/logging/__init__.py` & `proteinflow-2.2.2/proteinflow/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/metrics/__init__.py` & `proteinflow-2.2.2/proteinflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/processing/__init__.py` & `proteinflow-2.2.2/proteinflow/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/split/__init__.py` & `proteinflow-2.2.2/proteinflow/split/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/split/utils.py` & `proteinflow-2.2.2/proteinflow/split/utils.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow/visualize.py` & `proteinflow-2.2.2/proteinflow/visualize.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/proteinflow.egg-info/PKG-INFO` & `proteinflow-2.2.2/proteinflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 2.2.1
+Version: 2.2.2
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 2.2.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.2.2 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-2.2.1/proteinflow.egg-info/SOURCES.txt` & `proteinflow-2.2.2/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/pyproject.toml` & `proteinflow-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `proteinflow-2.2.1/tests/test_download.py` & `proteinflow-2.2.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/tests/test_entry.py` & `proteinflow-2.2.2/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/tests/test_generate.py` & `proteinflow-2.2.2/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/tests/test_ligands.py` & `proteinflow-2.2.2/tests/test_ligands.py`

 * *Files identical despite different names*

### Comparing `proteinflow-2.2.1/tests/test_sabdab.py` & `proteinflow-2.2.2/tests/test_sabdab.py`

 * *Files identical despite different names*

