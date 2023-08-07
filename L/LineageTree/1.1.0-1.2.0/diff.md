# Comparing `tmp/LineageTree-1.1.0.tar.gz` & `tmp/LineageTree-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LineageTree-1.1.0.tar", last modified: Thu Apr 27 10:28:56 2023, max compression
+gzip compressed data, was "LineageTree-1.2.0.tar", last modified: Mon Aug  7 12:47:39 2023, max compression
```

## Comparing `LineageTree-1.1.0.tar` & `LineageTree-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.765994 LineageTree-1.1.0/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-08-16 08:53:03.000000 LineageTree-1.1.0/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)     2362 2023-04-27 10:28:56.765842 LineageTree-1.1.0/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1895 2022-08-16 08:53:03.000000 LineageTree-1.1.0/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      567 2023-04-27 10:28:38.000000 LineageTree-1.1.0/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)       38 2023-04-27 10:28:56.766036 LineageTree-1.1.0/setup.cfg
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1052 2023-04-27 10:28:38.000000 LineageTree-1.1.0/setup.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.762978 LineageTree-1.1.0/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.763749 LineageTree-1.1.0/src/LineageTree/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       59 2023-04-27 10:28:38.000000 LineageTree-1.1.0/src/LineageTree/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    75126 2023-04-27 10:26:30.000000 LineageTree-1.1.0/src/LineageTree/lineageTree.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.764379 LineageTree-1.1.0/src/LineageTree.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     2362 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      319 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       50 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       12 2023-04-27 10:28:56.000000 LineageTree-1.1.0/src/LineageTree.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-04-27 10:28:56.765570 LineageTree-1.1.0/test/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      264 2023-01-31 17:57:50.000000 LineageTree-1.1.0/test/test_lineageTree.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-08-07 12:47:39.100788 LineageTree-1.2.0/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-08-16 08:53:03.000000 LineageTree-1.2.0/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3103 2023-08-07 12:47:39.100849 LineageTree-1.2.0/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1895 2022-08-16 08:53:03.000000 LineageTree-1.2.0/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      523 2023-08-07 09:48:02.000000 LineageTree-1.2.0/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1470 2023-08-07 12:47:39.101163 LineageTree-1.2.0/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-08-07 12:47:39.098120 LineageTree-1.2.0/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-08-07 12:47:39.098963 LineageTree-1.2.0/src/LineageTree/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       59 2023-08-07 09:48:02.000000 LineageTree-1.2.0/src/LineageTree/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    76208 2023-08-02 15:54:03.000000 LineageTree-1.2.0/src/LineageTree/lineageTree.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-08-07 12:47:39.100459 LineageTree-1.2.0/src/LineageTree.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     3103 2023-08-07 12:47:39.000000 LineageTree-1.2.0/src/LineageTree.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      362 2023-08-07 12:47:39.000000 LineageTree-1.2.0/src/LineageTree.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-08-07 12:47:39.000000 LineageTree-1.2.0/src/LineageTree.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       70 2023-08-07 12:47:39.000000 LineageTree-1.2.0/src/LineageTree.egg-info/entry_points.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       66 2023-08-07 12:47:39.000000 LineageTree-1.2.0/src/LineageTree.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       12 2023-08-07 12:47:39.000000 LineageTree-1.2.0/src/LineageTree.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-08-07 12:47:39.100572 LineageTree-1.2.0/test/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      264 2023-01-31 17:57:50.000000 LineageTree-1.2.0/test/test_lineageTree.py
```

### Comparing `LineageTree-1.1.0/LICENSE` & `LineageTree-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LineageTree-1.1.0/PKG-INFO` & `LineageTree-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: LineageTree
-Version: 1.1.0
-Summary: Lineage tree structure for TGMM algorithm
-Home-page: https://github.com/leoguignard/TGMMlibraries
-Author: Leo Guignard
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: svg
-License-File: LICENSE
-
 # LineageTree
 
 This library allows to import and work with cell (but not limited to cells) lineage trees.
 With LineageTree you can read from:
   - TGMM algorithm outputs described in [Fernando et al. 2014](https://www.nature.com/articles/nmeth.3036)
   - TrackMate files described in [Tinevez et al. 2017](https://doi.org/10.1016/j.ymeth.2016.09.016)
   - MaMuT files described in [Wolff et al. 2018](https://doi.org/10.7554/eLife.34410)
```

### Comparing `LineageTree-1.1.0/pyproject.toml` & `LineageTree-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,21 @@
 line-length = 79
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
 ]
 "src/LineageTree/__init__.py" = [
     '__version__ = "{version}"',
-]
-"setup.py" = [
-    'version="{version}"',
 ]
```

### Comparing `LineageTree-1.1.0/src/LineageTree/lineageTree.py` & `LineageTree-1.2.0/src/LineageTree/lineageTree.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from scipy.spatial import Delaunay
 from itertools import combinations
 from numbers import Number
 import struct
 from scipy.spatial.distance import cdist
 import pickle as pkl
 
+
 class lineageTree(object):
     def get_next_id(self):
         """Computes the next authorized id.
 
         Returns:
             int: next authorized id
         """
@@ -273,15 +274,19 @@
         node_size=None,
         stroke_width=None,
         factor=1.0,
         node_color=None,
         stroke_color=None,
         positions=None,
         node_color_map=None,
+        normalize=True,
     ):
+
+        ##### remove background? default True background value? default 1
+
         """Writes the lineage tree to an SVG file.
         Node and edges coloring and size can be provided.
 
         Args:
             file_name: str, filesystem filename valid for `open()`
             roots: [int, ...], list of node ids to be drawn. If `None` all the nodes will be drawn. Default `None`
             draw_nodes: bool, wether to print the nodes or not, default `True`
@@ -296,15 +301,15 @@
                        the the size will be mapped according to the property
             stroke_width: func, a function that maps a node id to a `float` value that will determine the
                           width of the daughter edge.  The default function return the constant value `vertical_space_factor/2.1`
             factor: float, scaling factor for nodes positions, default 1
             node_color: func | str, a function that maps a node id to a triplet between 0 and 255.
                         The triplet will determine the color of the node. If a string is given instead and it is a property
                         of the tree, the the color will be mapped according to the property
-            node_color_map: str, the name of the colormap to use to color the nodes
+            node_color_map: str | func, the name of the colormap to use to color the nodes, or a colormap function
             stroke_color: func, a function that maps a node id to a triplet between 0 and 255.
                           The triplet will determine the color of the stroke of the inward edge.
             positions: {int: [float, float], ...}, dictionary that maps a node id to a 2D position.
                        Default `None`. If provided it will be used to position the nodes.
         """
         import svgwrite
 
@@ -313,14 +318,15 @@
             max_ = np.percentile(v, 99)
             values = range * ((v - min_) / (max_ - min_)) + shift
             values_dict_nodes = dict(zip(nodes, values))
             return lambda x: values_dict_nodes[x] * mult
 
         if roots is None:
             roots = list(set(self.successor).difference(self.predecessor))
+            roots = [cell for cell in roots if self.image_label[cell] != 1]
 
         if node_size is None:
             node_size = lambda x: vert_space_factor / 2.1
         elif isinstance(node_size, str) and node_size in self.__dict__:
             values = np.array([self[node_size][c] for c in self.nodes])
             node_size = normalize_values(
                 values, self.nodes, 0.5, 0.5, vert_space_factor / 2.1
@@ -451,36 +457,62 @@
                             (factor * x1, factor * y1),
                             node_size(c),
                             fill=svgwrite.rgb(*(node_color(c))),
                         )
                     )
         dwg.save()
 
-    def to_treex(self, sampling=1):
-        """Convert the lineage tree into a treex file."""
+    def to_treex(self, sampling=1, start=0, finish=10000, many=True):
+        """
+        Convert the lineage tree into a treex file.
+
+        start/finish refer to first index in the new array times_to_consider
+
+        """
         from treex.tree import Tree
+        from warnings import warn
 
+        start //= sampling
+        finish //= sampling
+        if finish - start <= 0:
+            warn("Will return None, because start = finish")
+            return None
         id_to_tree = {id: Tree() for id in self.nodes}
-        times_to_consider = [t for t, n in self.time_nodes.items() if 0<len(n)]
-        times_to_consider = times_to_consider[::sampling]
+        times_to_consider = [
+            t for t, n in self.time_nodes.items() if 0 < len(n)
+        ]
+        times_to_consider = times_to_consider[start:finish:sampling]
+        start_time = times_to_consider[0]
         for t in times_to_consider:
             for id_mother in self.time_nodes[t]:
                 ids_daughters = self.successor.get(id_mother, [])
                 new_ids_daughters = ids_daughters.copy()
-                for _ in range(sampling-1):
+                for _ in range(sampling - 1):
                     tmp = []
                     for d in new_ids_daughters:
                         tmp.extend(self.successor.get(d, [d]))
                     new_ids_daughters = tmp
-                for daugther in new_ids_daughters: ## For each daughter in the list of daughters
-                    id_to_tree[id_mother].add_subtree(id_to_tree[daugther]) ## Add the Treex daughter as a subtree of the Treex mother   
-        
-        roots = [id_to_tree[id] for id in set(self.successor).difference(self.predecessor)] 
-
-        return roots
+                for (
+                    daugther
+                ) in (
+                    new_ids_daughters
+                ):  ## For each daughter in the list of daughters
+                    id_to_tree[id_mother].add_subtree(
+                        id_to_tree[daugther]
+                    )  ## Add the Treex daughter as a subtree of the Treex mother
+        roots = [id_to_tree[id] for id in set(self.time_nodes[start_time])]
+        for root, ids in zip(roots, set(self.time_nodes[start_time])):
+            root.add_attribute_to_id("ID", ids)
+        if not many:
+            reroot = Tree()
+            for root in roots:
+                reroot.add_subtree(root)
+            return reroot
+        else:
+            return roots
 
     def to_tlp(
         self,
         fname,
         t_min=-1,
         t_max=np.inf,
         nodes_to_use=None,
@@ -564,17 +596,15 @@
                     edges_to_use += [
                         e
                         for e in self.edges
                         if t_min < self.time[e[0]] < t_max
                     ]
                 if spatial:
                     edges_to_use += [
-                        e
-                        for e in s_edges
-                        if t_min < self.time[e[0]] < t_max
+                        e for e in s_edges if t_min < self.time[e[0]] < t_max
                     ]
             else:
                 nodes_to_use = list(self.nodes)
                 edges_to_use = []
                 if temporal:
                     edges_to_use += list(self.edges)
                 if spatial:
@@ -756,263 +786,210 @@
         """Read an `xml` or `pkl` file produced by the ASTEC algorithm.
 
         Args:
             file_path (str): path to an output generated by ASTEC
             eigen (bool): whether or not to read the eigen values, default False
         """
         self._astec_keydictionary = {
-            "lineage": {
-                "output_key": "cell_lineage",
-                "input_keys": [
-                    "lineage_tree",
-                    "lin_tree",
-                    "Lineage tree",
-                    "cell_lineage",
-                ],
-            },
-            "h_min": {
-                "output_key": "cell_h_min",
-                "input_keys": ["cell_h_min", "h_mins_information"],
-            },
-            "volume": {
-                "output_key": "cell_volume",
-                "input_keys": [
-                    "cell_volume",
-                    "volumes_information",
-                    "volumes information",
-                    "vol",
-                ],
-            },
-            "surface": {
-                "output_key": "cell_surface",
-                "input_keys": ["cell_surface", "cell surface"],
-            },
-            "compactness": {
-                "output_key": "cell_compactness",
-                "input_keys": [
-                    "cell_compactness",
-                    "Cell Compactness",
-                    "compacity",
-                    "cell_sphericity",
-                ],
-            },
-            "sigma": {
-                "output_key": "cell_sigma",
-                "input_keys": ["cell_sigma", "sigmas_information", "sigmas"],
-            },
-            "label_in_time": {
-                "output_key": "cell_labels_in_time",
-                "input_keys": [
-                    "cell_labels_in_time",
-                    "Cells labels in time",
-                    "time_labels",
-                ],
-            },
-            "barycenter": {
-                "output_key": "cell_barycenter",
-                "input_keys": [
-                    "cell_barycenter",
-                    "Barycenters",
-                    "barycenters",
-                ],
-            },
-            "fate": {
-                "output_key": "cell_fate",
-                "input_keys": ["cell_fate", "Fate"],
-            },
-            "fate2": {
-                "output_key": "cell_fate_2",
-                "input_keys": ["cell_fate_2", "Fate2"],
-            },
-            "fate3": {
-                "output_key": "cell_fate_3",
-                "input_keys": ["cell_fate_3", "Fate3"],
-            },
-            "fate4": {
-                "output_key": "cell_fate_4",
-                "input_keys": ["cell_fate_4", "Fate4"],
-            },
-            "all-cells": {
-                "output_key": "all_cells",
-                "input_keys": [
-                    "all_cells",
-                    "All Cells",
-                    "All_Cells",
-                    "all cells",
-                    "tot_cells",
-                ],
-            },
-            "principal-value": {
-                "output_key": "cell_principal_values",
-                "input_keys": ["cell_principal_values", "Principal values"],
-            },
-            "name": {
-                "output_key": "cell_name",
-                "input_keys": ["cell_name", "Names", "names", "cell_names"],
-            },
-            "contact": {
-                "output_key": "cell_contact_surface",
-                "input_keys": [
-                    "cell_contact_surface",
-                    "cell_cell_contact_information",
-                ],
-            },
-            "history": {
-                "output_key": "cell_history",
-                "input_keys": [
-                    "cell_history",
-                    "Cells history",
-                    "cell_life",
-                    "life",
-                ],
-            },
-            "principal-vector": {
-                "output_key": "cell_principal_vectors",
-                "input_keys": ["cell_principal_vectors", "Principal vectors"],
-            },
-            "name-score": {
-                "output_key": "cell_naming_score",
-                "input_keys": ["cell_naming_score", "Scores", "scores"],
-            },
-            "problems": {
-                "output_key": "problematic_cells",
-                "input_keys": ["problematic_cells"],
-            },
-            "unknown": {
-                "output_key": "unknown_key",
-                "input_keys": ["unknown_key"],
-            },
+            "cell_lineage": [
+                "lineage_tree",
+                "lin_tree",
+                "Lineage tree",
+                "cell_lineage",
+            ],
+            "cell_h_min": ["cell_h_min", "h_mins_information"],
+            "cell_volume": [
+                "cell_volume",
+                "volumes_information",
+                "volumes information",
+                "vol",
+            ],
+            "cell_surface": ["cell_surface", "cell surface"],
+            "cell_compactness": [
+                "cell_compactness",
+                "Cell Compactness",
+                "compacity",
+                "cell_sphericity",
+            ],
+            "cell_sigma": ["cell_sigma", "sigmas_information", "sigmas"],
+            "cell_labels_in_time": [
+                "cell_labels_in_time",
+                "Cells labels in time",
+                "time_labels",
+            ],
+            "cell_barycenter": [
+                "cell_barycenter",
+                "Barycenters",
+                "barycenters",
+            ],
+            "cell_fate": ["cell_fate", "Fate"],
+            "cell_fate_2": ["cell_fate_2", "Fate2"],
+            "cell_fate_3": ["cell_fate_3", "Fate3"],
+            "cell_fate_4": ["cell_fate_4", "Fate4"],
+            "all_cells": [
+                "all_cells",
+                "All Cells",
+                "All_Cells",
+                "all cells",
+                "tot_cells",
+            ],
+            "cell_principal_values": [
+                "cell_principal_values",
+                "Principal values",
+            ],
+            "cell_name": ["cell_name", "Names", "names", "cell_names"],
+            "cell_contact_surface": [
+                "cell_contact_surface",
+                "cell_cell_contact_information",
+            ],
+            "cell_history": [
+                "cell_history",
+                "Cells history",
+                "cell_life",
+                "life",
+            ],
+            "cell_principal_vectors": [
+                "cell_principal_vectors",
+                "Principal vectors",
+            ],
+            "cell_naming_score": ["cell_naming_score", "Scores", "scores"],
+            "problematic_cells": ["problematic_cells"],
+            "unknown_key": ["unknown_key"],
         }
+
         if os.path.splitext(file_path)[-1] == ".xml":
             tmp_data = self._read_from_ASTEC_xml(file_path)
         else:
             tmp_data = self._read_from_ASTEC_pkl(file_path, eigen)
 
+        # make sure these are all named liked they are in tmp_data (or change dictionary above)
         self.name = {}
         self.volume = {}
         self.lT2pkl = {}
         self.pkl2lT = {}
         self.contact = {}
         self.prob_cells = set()
-        if "cell_lineage" in tmp_data:
-            lt = tmp_data["cell_lineage"]
-        elif "lin_tree" in tmp_data:
-            lt = tmp_data["lin_tree"]
-        else:
-            lt = tmp_data["Lineage tree"]
-        if "cell_name" in tmp_data:
-            names = tmp_data["cell_name"]
-        elif "Names" in tmp_data:
-            names = tmp_data["Names"]
-        else:
-            names = {}
-        if "cell_fate" in tmp_data:
-            self.fates = {}
-            fates = tmp_data["cell_fate"]
-            do_fates = True
-        else:
-            do_fates = False
-        if "cell_volume" in tmp_data:
-            do_volumes = True
-            volumes = tmp_data["cell_volume"]
-        elif "volume_information" in tmp_data:
-            do_volumes = True
-            volumes = tmp_data["volume_information"]
-        else:
-            do_volumes = False
+        self.image_label = {}
+
+        lt = tmp_data["cell_lineage"]
+
+        # if "cell_name" in tmp_data:
+        #     names = tmp_data["cell_name"]
+        # else:
+        #     names = {}
+
         if "cell_contact_surface" in tmp_data:
             do_surf = True
             surfaces = tmp_data["cell_contact_surface"]
         else:
             do_surf = False
-        if "problematic_cells" in tmp_data:
-            prob_cells = set(tmp_data["problematic_cells"])
-        else:
-            prob_cells = set()
-        if eigen:
-            self.eigen_vectors = {}
-            self.eigen_values = {}
-            eig_val = tmp_data["cell_principal_values"]
-            eig_vec = tmp_data["cell_principal_vectors"]
+
+        # if "problematic_cells" in tmp_data:
+        #     prob_cells = set(tmp_data["problematic_cells"])
+        # else:
+        #     prob_cells = set()
+        # if eigen:
+        #     self.eigen_vectors = {}
+        #     self.eigen_values = {}
+        #     eig_val = tmp_data["cell_principal_values"]
+        #     eig_vec = tmp_data["cell_principal_vectors"]
 
         inv = {vi: [c] for c, v in lt.items() for vi in v}
         nodes = set(lt).union(inv)
-        if "cell_barycenter" in tmp_data:
-            pos = tmp_data["cell_barycenter"]
-        elif "Barycenters" in tmp_data:
-            pos = tmp_data["Barycenters"]
-        else:
-            pos = dict(
-                list(
-                    zip(
-                        nodes,
-                        [
-                            [0.0, 0.0, 0.0],
-                        ]
-                        * len(nodes),
-                    )
-                )
-            )
+        # if "cell_barycenter" in tmp_data:
+        #     pos = tmp_data["cell_barycenter"]
+        # else:
+        #     pos = dict(list(zip(nodes,[[0.0, 0.0, 0.0]]* len(nodes))))
 
         unique_id = 0
-        id_corres = {}
-        self.image_label = {}
+        # id_corres = {}
+
         for n in nodes:
-            if n in prob_cells:
-                self.prob_cells.add(unique_id)
+            # if n in prob_cells:
+            #     self.prob_cells.add(unique_id)
             # if n in pos and n in names:
             t = n // 10**4
             self.image_label[unique_id] = n % 10**4
             self.lT2pkl[unique_id] = n
             self.pkl2lT[n] = unique_id
-            self.name[unique_id] = names.get(n, "")
-            position = np.array(pos.get(n, [0, 0, 0]), dtype=float)
+            # self.name[unique_id] = names.get(n, "")
+            # position = np.array(pos.get(n, [0, 0, 0]), dtype=float)
             self.time_nodes.setdefault(t, set()).add(unique_id)
             self.nodes.add(unique_id)
-            self.pos[unique_id] = position
+            # self.pos[unique_id] = position
             self.time[unique_id] = t
-            id_corres[n] = unique_id
-            if do_volumes:
-                self.volume[unique_id] = volumes.get(n, 0.0)
-            if eigen:
-                self.eigen_vectors[unique_id] = eig_vec.get(n)
-                self.eigen_values[unique_id] = eig_val.get(n)
-            if do_fates:
-                self.fates[unique_id] = fates.get(n, "")
+            # id_corres[n] = unique_id
+            if "cell_volume" in tmp_data:
+                self.volume[unique_id] = tmp_data["cell_volume"].get(n, 0.0)
+            # if eigen:
+            #     self.eigen_vectors[unique_id] = eig_vec.get(n)
+            #     self.eigen_values[unique_id] = eig_val.get(n)
+            if "cell_fate" in tmp_data:
+                self.fates = {}
+                self.fates[unique_id] = tmp_data["cell_fate"].get(n, "")
 
             unique_id += 1
         # self.contact = {self.pkl2lT[c]: v for c, v in surfaces.iteritems() if c in self.pkl2lT}
         if do_surf:
             for c in nodes:
                 if c in surfaces and c in self.pkl2lT:
                     self.contact[self.pkl2lT[c]] = {
                         self.pkl2lT.get(n, -1): s
                         for n, s in surfaces[c].items()
                         if n % 10**4 == 1 or n in self.pkl2lT
                     }
 
-        for n, new_id in id_corres.items():
+        for n, new_id in self.pkl2lT.items():
             # new_id = id_corres[n]
             if n in inv:
-                self.predecessor[new_id] = [id_corres[ni] for ni in inv[n]]
+                self.predecessor[new_id] = [self.pkl2lT[ni] for ni in inv[n]]
             if n in lt:
                 self.successor[new_id] = [
-                    id_corres[ni] for ni in lt[n] if ni in id_corres
+                    self.pkl2lT[ni] for ni in lt[n] if ni in self.pkl2lT
                 ]
                 self.edges.update(
                     [(new_id, ni) for ni in self.successor[new_id]]
                 )
                 for ni in self.successor[new_id]:
                     # self.edges += [(new_id, ni)]
                     self.time_edges.setdefault(t - 1, set()).add((new_id, ni))
 
         self.t_b = min(self.time_nodes)
         self.t_e = max(self.time_nodes)
         self.max_id = unique_id
 
+        # do this in the end of the process, skip lineage tree and whatever is stored already
+        for prop_name, prop_values in tmp_data.items():
+            if hasattr(self, prop_name):
+                continue
+            else:
+                if isinstance(prop_values, dict):
+                    dictionary = {
+                        self.pkl2lT[k]: v for k, v in prop_values.items()
+                    }
+                    # is it a regular dictionary or a dictionary with dictionaries inside?
+                    for key, value in dictionary.items():
+                        if isinstance(value, dict):
+                            # rename all ids from old to new
+                            dictionary[key] = {
+                                self.pkl2lT[k]: v for k, v in value
+                            }
+                    self.__dict__[prop_name] = dictionary
+                # is any of this necessary? Or does it mean it anyways does not contain information about the id and a simple else: is enough?
+                elif (
+                    prop_values.isinstance(set)
+                    or prop_values.isinstance(list)
+                    or prop_values.isinstance(np.array)
+                ):
+                    self.__dict__[prop_name] = prop_values
+
+            # what else could it be?
+
+        # add a list of all available properties
+
     def _read_from_ASTEC_xml(self, file_path):
         def _set_dictionary_value(root):
             if len(root) == 0:
                 if root.text is None:
                     return None
                 else:
                     return eval(root.text)
@@ -1026,38 +1003,40 @@
             return dictionary
 
         tree = ET.parse(file_path)
         root = tree.getroot()
         dictionary = {}
 
         for k, v in self._astec_keydictionary.items():
-            if root.tag == v["output_key"]:
+            if root.tag == k:
                 dictionary[str(root.tag)] = _set_dictionary_value(root)
                 break
         else:
             for child in root:
                 value = _set_dictionary_value(child)
                 if value is not None:
                     dictionary[str(child.tag)] = value
         return dictionary
 
     def _read_from_ASTEC_pkl(self, file_path, eigen=False):
-        
+
         with open(file_path, "rb") as f:
             tmp_data = pkl.load(f, encoding="latin1")
             f.close()
         new_ref = {}
         for k, v in self._astec_keydictionary.items():
-            for key in v["input_keys"]:
-                new_ref[key] = v["output_key"]
+            for key in v:
+                new_ref[key] = k
         new_dict = {}
 
         for k, v in tmp_data.items():
             if k in new_ref:
                 new_dict[new_ref[k]] = v
+            else:
+                new_dict[k] = v
         return new_dict
 
     def read_from_txt_for_celegans(self, file):
         implicit_l_t = {
             "AB": "P0",
             "P1": "P0",
             "EMS": "P1",
@@ -1285,14 +1264,49 @@
                 else:
                     if t in self.ind_cells:
                         self.ind_cells[t] += 1
                     else:
                         self.ind_cells[t] = 1
         self.max_id = unique_id - 1
 
+    def read_from_mastodon(self, path, name):
+        from mastodon_reader import MastodonReader
+
+        mr = MastodonReader(path)
+        spots, links = mr.read_tables()
+        mr.read_tags(spots, links)
+
+        self.node_name = {}
+
+        for c in spots.iloc:
+            unique_id = c.name
+            x, y, z = c.x, c.y, c.z
+            t = c.t
+            if name is not None:
+                n = c[name]
+            else:
+                n = ""
+            self.time_nodes.setdefault(t, set()).add(unique_id)
+            self.nodes.add(unique_id)
+            self.time[unique_id] = t
+            self.node_name[unique_id] = n
+            self.pos[unique_id] = np.array([x, y, z])
+
+        for e in links.iloc:
+            source = e.source_idx
+            target = e.target_idx
+            self.predecessor.setdefault(target, []).append(source)
+            self.successor.setdefault(source, []).append(target)
+            self.edges.add((source, target))
+            self.time_edges.setdefault(self.time[source], set()).add(
+                (source, target)
+            )
+        self.t_b = min(self.time_nodes.keys())
+        self.t_e = max(self.time_nodes.keys())
+
     def read_from_mamut_xml(self, path):
         """Read a lineage tree from a MaMuT xml.
 
         Args:
             path (str): path to the MaMut xml
         """
         tree = ET.parse(path)
@@ -1340,17 +1354,20 @@
         self.edges = set()
         self.roots = []
         tracks = {}
         self.successor = {}
         self.predecessor = {}
         self.track_name = {}
         for track in AllTracks:
-            t_id, l = int(track.attrib["TRACK_ID"]), float(
-                track.attrib["TRACK_DURATION"]
-            )
+            if "TRACK_DURATION" in track.attrib:
+                t_id, l = int(track.attrib["TRACK_ID"]), float(
+                    track.attrib["TRACK_DURATION"]
+                )
+            else:
+                t_id = int(track.attrib["TRACK_ID"])
             t_name = track.attrib["name"]
             tracks[t_id] = []
             for edge in track:
                 s, t = int(edge.attrib["SPOT_SOURCE_ID"]), int(
                     edge.attrib["SPOT_TARGET_ID"]
                 )
                 if s in self.nodes and t in self.nodes:
@@ -1567,23 +1584,23 @@
         self.edges = set(edges)
         self.t_b = min(time_nodes.keys())
         self.t_e = max(time_nodes.keys())
         self.is_root = is_root
         self.max_id = max(self.nodes)
 
     def write(self, fname):
-        if os.path.splitext(fname)[-1] != '.lT':
-            os.path.extsep.join(fname, 'lT')
-        with open(fname, 'bw') as f:
+        if os.path.splitext(fname)[-1] != ".lT":
+            fname = os.path.extsep.join((fname, "lT"))
+        with open(fname, "bw") as f:
             pkl.dump(self, f)
             f.close()
 
     @classmethod
     def load(clf, fname):
-        with open(fname, 'br') as f:
+        with open(fname, "br") as f:
             lT = pkl.load(f)
             f.close()
         return lT
 
     def get_idx3d(self, t):
         """Get a 3d kdtree for the dataset at time *t* .
         The  kdtree is stored in *self.kdtrees[t]*
@@ -1891,14 +1908,15 @@
         file_type="",
         delim=",",
         eigen=False,
         shape=None,
         raw_size=None,
         reorder=False,
         xml_attributes=[],
+        name=None,
     ):
         """Main library to build tree graph representation of lineage tree data
         It can read TGMM, ASTEC, SVF, MaMuT and TrackMate outputs.
 
         Args:
             file_format (strr): either - path format to TGMM xmls
                                        - path to the MaMuT xml
@@ -1929,21 +1947,23 @@
         file_type = file_type.lower()
         if file_type == "tgmm":
             self.read_tgmm_xml(file_format, tb, te, z_mult)
             self.t_b = tb
             self.t_e = te
         elif file_type == "mamut" or file_type == "trackmate":
             self.read_from_mamut_xml(file_format)
+        elif file_type == "mastodon":
+            self.read_from_mastodon(file_format, name)
         elif file_type == "celegans":
             self.read_from_txt_for_celegans(file_format)
         elif file_type == "celegans_cao":
             self.read_from_txt_for_celegans_CAO(
                 file_format, reorder=reorder, shape=shape, raw_size=raw_size
             )
         elif file_type == "astec":
             self.read_from_ASTEC(file_format, eigen)
         elif file_type == "csv":
             self.read_from_csv(file_format, z_mult, link=1, delim=delim)
-        elif file_format is not None and '.lT' in file_format:
-            self.read(file_format)
+        elif file_format is not None and ".lT" in file_format:
+            self.load(file_format)
         elif file_format is not None:
             self.read_from_binary(file_format)
```

### Comparing `LineageTree-1.1.0/src/LineageTree.egg-info/PKG-INFO` & `LineageTree-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 Metadata-Version: 2.1
 Name: LineageTree
-Version: 1.1.0
-Summary: Lineage tree structure for TGMM algorithm
-Home-page: https://github.com/leoguignard/TGMMlibraries
-Author: Leo Guignard
-Classifier: Development Status :: 5 - Production/Stable
+Version: 1.2.0
+Summary: Lineage tree structure
+Home-page: https://github.com/leoguignard/LineageTree
+Author: Léo Guignard
+Author-email: leo.guignard@univ-amu.fr
+License: MIT
+Project-URL: Bug Tracker, https://github.com/leoguignard/LineageTree/issues
+Project-URL: Documentation, https://github.com/leoguignard/LineageTree#README.md
+Project-URL: Source Code, https://github.com/leoguignard/LineageTree
+Project-URL: User Support, https://github.com/leoguignard/LineageTree/issues
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: svg
 License-File: LICENSE
 
 # LineageTree
 
 This library allows to import and work with cell (but not limited to cells) lineage trees.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

