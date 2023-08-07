# Comparing `tmp/seismic2dreem-0.0.2.tar.gz` & `tmp/seismic2dreem-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic2dreem-0.0.2.tar", last modified: Mon Jul 31 17:04:57 2023, max compression
+gzip compressed data, was "seismic2dreem-0.0.3.tar", last modified: Mon Aug  7 14:13:31 2023, max compression
```

## Comparing `seismic2dreem-0.0.2.tar` & `seismic2dreem-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-31 17:04:57.131309 seismic2dreem-0.0.2/
--rw-r--r--   0 ymdt       (501) staff       (20)     1068 2023-07-28 19:47:55.000000 seismic2dreem-0.0.2/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-07-31 17:04:57.131171 seismic2dreem-0.0.2/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      997 2023-07-31 16:16:06.000000 seismic2dreem-0.0.2/README.md
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-31 17:04:57.129756 seismic2dreem-0.0.2/seismic2dreem/
--rw-r--r--   0 ymdt       (501) staff       (20)       21 2023-07-28 19:52:38.000000 seismic2dreem-0.0.2/seismic2dreem/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)      671 2023-07-31 16:13:08.000000 seismic2dreem-0.0.2/seismic2dreem/cli.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1998 2023-07-31 15:55:26.000000 seismic2dreem-0.0.2/seismic2dreem/dump.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2615 2023-07-31 16:14:29.000000 seismic2dreem-0.0.2/seismic2dreem/main.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2151 2023-07-28 21:22:43.000000 seismic2dreem-0.0.2/seismic2dreem/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     1421 2023-07-28 23:16:58.000000 seismic2dreem-0.0.2/seismic2dreem/translation.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-31 17:04:57.130954 seismic2dreem-0.0.2/seismic2dreem.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      392 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       56 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/entry_points.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       19 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       14 2023-07-31 17:04:57.000000 seismic2dreem-0.0.2/seismic2dreem.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-31 17:04:57.131348 seismic2dreem-0.0.2/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-31 17:04:47.000000 seismic2dreem-0.0.2/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-08-07 14:13:31.513685 seismic2dreem-0.0.3/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1068 2023-07-28 19:47:55.000000 seismic2dreem-0.0.3/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-08-07 14:13:31.513539 seismic2dreem-0.0.3/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      997 2023-07-31 16:16:06.000000 seismic2dreem-0.0.3/README.md
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-08-07 14:13:31.512285 seismic2dreem-0.0.3/seismic2dreem/
+-rw-r--r--   0 ymdt       (501) staff       (20)       21 2023-07-28 19:52:38.000000 seismic2dreem-0.0.3/seismic2dreem/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)      671 2023-07-31 16:13:08.000000 seismic2dreem-0.0.3/seismic2dreem/cli.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1998 2023-07-31 15:55:26.000000 seismic2dreem-0.0.3/seismic2dreem/dump.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2637 2023-08-07 14:04:21.000000 seismic2dreem-0.0.3/seismic2dreem/main.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2407 2023-08-07 13:59:03.000000 seismic2dreem-0.0.3/seismic2dreem/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     1656 2023-08-07 14:11:24.000000 seismic2dreem-0.0.3/seismic2dreem/translation.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-08-07 14:13:31.513347 seismic2dreem-0.0.3/seismic2dreem.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)      287 2023-08-07 14:13:31.000000 seismic2dreem-0.0.3/seismic2dreem.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      392 2023-08-07 14:13:31.000000 seismic2dreem-0.0.3/seismic2dreem.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-08-07 14:13:31.000000 seismic2dreem-0.0.3/seismic2dreem.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       56 2023-08-07 14:13:31.000000 seismic2dreem-0.0.3/seismic2dreem.egg-info/entry_points.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       19 2023-08-07 14:13:31.000000 seismic2dreem-0.0.3/seismic2dreem.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       14 2023-08-07 14:13:31.000000 seismic2dreem-0.0.3/seismic2dreem.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-08-07 14:13:31.513732 seismic2dreem-0.0.3/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-08-07 14:13:19.000000 seismic2dreem-0.0.3/setup.py
```

### Comparing `seismic2dreem-0.0.2/LICENSE` & `seismic2dreem-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.2/README.md` & `seismic2dreem-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.2/seismic2dreem/cli.py` & `seismic2dreem-0.0.3/seismic2dreem/cli.py`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.2/seismic2dreem/dump.py` & `seismic2dreem-0.0.3/seismic2dreem/dump.py`

 * *Files identical despite different names*

### Comparing `seismic2dreem-0.0.2/seismic2dreem/main.py` & `seismic2dreem-0.0.3/seismic2dreem/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,18 +40,18 @@
                     try:
                         out[construct][section] = seismic_csv_to_dreem_json(seismic_path.get_csv_path(sample, construct, section))
                     except FileNotFoundError:
                         if verbose:
                             print(f"WARNING: no csv found for {sample}/{construct}/{section}")
                     except ValueError as e:
                         if verbose:
-                            print(f"WARNING: {e} for {sample}/{construct}/{section}")
+                            print(f"WARNING value error: {e} for {sample}/{construct}/{section}")
                     except Exception as e:
                         if verbose:
-                            print(f"WARNING: {e} for {sample}/{construct}/{section}")
+                            print(f"WARNING: exception {e} for {sample}/{construct}/{section}")
                 
             # clean up empty constructs
             for construct in seismic_path.list_constructs(sample):
                 if len(out[construct]) == 1:
                     if len(out[construct][list(out[construct].keys())[0]]) == 0:
                         del out[construct]
```

### Comparing `seismic2dreem-0.0.2/seismic2dreem/path.py` & `seismic2dreem-0.0.3/seismic2dreem/path.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 from os.path import join, isfile, isdir, dirname
 
 
 class SeismicPath:
     
     def __init__(self, root:str) -> None:
         assert isdir(root), f"seismic_folder_path is not a directory: {root}"
-        self.root = join(root, "out",'table')
+        self.root = self.find_table(root)
         assert isdir(self.root), f"seismic_folder_path does not contain a 'out/table' directory: {root}"
+        
+    def find_table(self, root):
+        paths = os.walk(root)
+        for path in paths:
+            path = path[0]
+            if path.split('/')[-1] == 'table':
+                return path
+        raise FileNotFoundError("No table directory found")
     
     def list_csvs(self):
         for sample in self.list_samples():
             for construct in self.list_constructs(sample):
                 for section in self.list_sections(sample, construct):
                     yield self.get_csv(sample, construct, section)
```

### Comparing `seismic2dreem-0.0.2/seismic2dreem/translation.py` & `seismic2dreem-0.0.3/seismic2dreem/translation.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 import gzip
 import shutil
 import os
 
 translation_arrays = {
     "Called": 'cov',
+    "Covered" : 'cov',
+    "Informed": 'info',
     "Subbed": 'sub_N',
     "Subbed-A": 'sub_A',
     "Subbed-C": 'sub_C',
     "Subbed-G": 'sub_G',
     "Subbed-T": 'sub_T',
     "Deleted": 'del',
     "Inserted": 'ins',
@@ -20,18 +22,20 @@
     # load csv
     i = pd.read_csv(csv_path)
     sequence = ''.join(i['Base'].tolist())
     
     # convert to json
     d = {}
     for k, v in translation_arrays.items():
-        d[v] = np.array(i[k], dtype=np.int64).tolist()
+        if k in i.columns:
+            d[v] = np.array(i[k], dtype=np.int64).tolist()
     d['min_cov'] = min(d['cov'])
-    d['info'] = (i['Mutated'] + i['Matched']).tolist()
-    d['sub_rate'] = (np.array(d['sub_N']) / np.array(d['info'])).tolist()
+    if 'info' not in d.keys():
+        d['info'] = (i['Mutated'] + i['Matched']).tolist()
+    d['sub_rate'] = np.divide(np.array(d['sub_N']).astype(float), np.array(d['info']).astype(float), out=np.zeros_like(np.array(d['sub_N']).astype(float)), where= np.array(d['info'])!=0).tolist()
     
     # add sub_hist from relate-per-read.csv.gz
     d['sub_hist'] = read_num_of_mutations(csv_path.replace('relate-per-pos.csv', 'relate-per-read.csv.gz'))
     
     return {'sequence': sequence, 'pop_avg': d}
 
 def read_num_of_mutations(csv_gz_path:str):
```

### Comparing `seismic2dreem-0.0.2/setup.py` & `seismic2dreem-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="seismic2dreem",
-    version='0.0.2',
+    version='0.0.3',
     description="Converts seismic data to dreem format",
     author="Yves Martin des Taillades for the Rouskin Lab",
     author_email="yves@martin.yt",
     url="https://github.com/rouskinlab/seismic2dreem",
     packages=find_packages(),
     install_requires=['pandas','numpy','click'],
     python_requires=">=3.9",
```

