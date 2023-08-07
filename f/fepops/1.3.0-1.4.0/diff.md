# Comparing `tmp/fepops-1.3.0.tar.gz` & `tmp/fepops-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fepops-1.3.0.tar", last modified: Wed May  3 13:57:10 2023, max compression
+gzip compressed data, was "fepops-1.4.0.tar", last modified: Sun Aug  6 22:32:30 2023, max compression
```

## Comparing `fepops-1.3.0.tar` & `fepops-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.208404 fepops-1.3.0/
--rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.3.0/LICENSE.md
--rw-rw-r--   0 justin    (1002) justin    (1002)     4500 2023-05-03 13:57:10.208404 fepops-1.3.0/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)     4079 2023-05-03 13:53:36.000000 fepops-1.3.0/README.md
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.192404 fepops-1.3.0/fepops/
--rw-rw-r--   0 justin    (1002) justin    (1002)       26 2023-03-28 16:17:49.000000 fepops-1.3.0/fepops/__init__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)     3717 2023-04-08 17:08:41.000000 fepops-1.3.0/fepops/__main__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)    23245 2023-05-02 17:37:04.000000 fepops-1.3.0/fepops/fepops.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.192404 fepops-1.3.0/fepops.egg-info/
--rw-rw-r--   0 justin    (1002) justin    (1002)     4500 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)      269 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      136 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/requires.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      118 2023-04-01 11:25:23.000000 fepops-1.3.0/pyproject.toml
--rw-rw-r--   0 justin    (1002) justin    (1002)      696 2023-05-03 13:57:10.208404 fepops-1.3.0/setup.cfg
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.192404 fepops-1.3.0/test/
--rw-rw-r--   0 justin    (1002) justin    (1002)      956 2023-04-01 11:25:23.000000 fepops-1.3.0/test/tests.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-08-06 22:32:30.588129 fepops-1.4.0/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.4.0/LICENSE.md
+-rw-rw-r--   0 justin    (1002) justin    (1002)      319 2023-08-06 22:32:30.588129 fepops-1.4.0/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4079 2023-05-03 13:53:36.000000 fepops-1.4.0/README.md
+-rw-rw-r--   0 justin    (1002) justin    (1002)      977 2023-08-06 22:28:07.000000 fepops-1.4.0/pyproject.toml
+-rw-rw-r--   0 justin    (1002) justin    (1002)       38 2023-08-06 22:32:30.588129 fepops-1.4.0/setup.cfg
+-rw-rw-r--   0 justin    (1002) justin    (1002)       38 2023-08-06 20:41:37.000000 fepops-1.4.0/setup.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-08-06 22:32:30.584129 fepops-1.4.0/src/
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-08-06 22:32:30.584129 fepops-1.4.0/src/fepops/
+-rw-rw-r--   0 justin    (1002) justin    (1002)       31 2023-08-06 22:28:07.000000 fepops-1.4.0/src/fepops/__init__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     3499 2023-08-06 22:28:07.000000 fepops-1.4.0/src/fepops/__main__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)    16988 2023-08-06 22:28:07.000000 fepops-1.4.0/src/fepops/benchmark.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4855 2023-08-06 22:28:07.000000 fepops-1.4.0/src/fepops/dude_preprocessor.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)    33769 2023-08-06 22:28:07.000000 fepops-1.4.0/src/fepops/fepops.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-08-06 22:32:30.584129 fepops-1.4.0/src/fepops/fepops_persistent/
+-rwxrwxr-x   0 justin    (1002) justin    (1002)      143 2023-08-06 20:41:37.000000 fepops-1.4.0/src/fepops/fepops_persistent/__init__.py
+-rwxrwxr-x   0 justin    (1002) justin    (1002)    13921 2023-08-06 22:28:07.000000 fepops-1.4.0/src/fepops/fepops_persistent/fepops_persistent_abc.py
+-rwxrwxr-x   0 justin    (1002) justin    (1002)     3567 2023-08-06 20:41:37.000000 fepops-1.4.0/src/fepops/fepops_persistent/fepopsdb_json.py
+-rwxrwxr-x   0 justin    (1002) justin    (1002)     5365 2023-08-06 20:41:37.000000 fepops-1.4.0/src/fepops/fepops_persistent/fepopsdb_sqlite.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)      527 2023-08-06 20:41:37.000000 fepops-1.4.0/src/fepops/fepops_persistent/utils.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-08-06 22:32:30.584129 fepops-1.4.0/src/fepops.egg-info/
+-rw-rw-r--   0 justin    (1002) justin    (1002)      319 2023-08-06 22:32:30.000000 fepops-1.4.0/src/fepops.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)      581 2023-08-06 22:32:30.000000 fepops-1.4.0/src/fepops.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-08-06 22:32:30.000000 fepops-1.4.0/src/fepops.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)       61 2023-08-06 22:32:30.000000 fepops-1.4.0/src/fepops.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-08-06 22:32:30.000000 fepops-1.4.0/src/fepops.egg-info/top_level.txt
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-08-06 22:32:30.588129 fepops-1.4.0/test/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     2182 2023-08-06 22:28:07.000000 fepops-1.4.0/test/tests.py
```

### Comparing `fepops-1.3.0/LICENSE.md` & `fepops-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fepops-1.3.0/PKG-INFO` & `fepops-1.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fepops
-Version: 1.3.0
-Summary: Python implementation of the FEPOPS molecular descriptors
-Home-page: https://github.com/JustinYKC/FEPOPS
-Author: Yan-Kai Chen
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # FEPOPS(feature point pharmacophores)
 Python implementation of the FEPOPS molecular similarity method and descriptor generator. The FEPOPS descriptors is a 3D method of molecular representation by four centroids with five pharmacophoric features (i.e. atomic logP, atomic partial charges, hydrogen bond acceptors, hydrogen bond donors, and 6 distances between the four centroids). This implementation was recreated following the original paper: [https://pubs.acs.org/doi/10.1021/jm049654z](https://pubs.acs.org/doi/10.1021/jm049654z)
 
 ### Steps for implementation:
 1. Preprocessing: Molecules were filtered by the number of atoms (< 4), the number of rings (> 9), and the number of rotatable bonds (< 40). A salt/ions filter was then applied. Filtering carried out using `mol_filter.py`.
 2. Tautomer enumeration: Tautomers for each molecule were enumerated and saved as mol objects (codes in `fepops.py`).
 3. Sample conformers through rotation of flexible bonds: Each tautomer underwent conformer generation, changing the angles of all rotatable bonds. Up to 1024 conformers are sampled from the pool of conformers if more than 5 rotatable bonds are found in a molecule (codes in `fepops.py`).
@@ -75,8 +62,8 @@
                 continue
             elif "SMILES Parse Error" in err:
                 print (f"# {id} SMILES_parse_error\n")
                 continue
 
         fepops_features = f.get_fepops(smiles)
         print (f"{fepops_features}\n")
-```
+```
```

