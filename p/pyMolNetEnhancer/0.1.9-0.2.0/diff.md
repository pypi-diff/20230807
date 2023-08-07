# Comparing `tmp/pyMolNetEnhancer-0.1.9.tar.gz` & `tmp/pyMolNetEnhancer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyMolNetEnhancer-0.1.9.tar", last modified: Thu Nov 28 12:41:47 2019, max compression
+gzip compressed data, was "dist/pyMolNetEnhancer-0.2.0.tar", last modified: Mon Aug  7 12:59:54 2023, max compression
```

## Comparing `pyMolNetEnhancer-0.1.9.tar` & `pyMolNetEnhancer-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 madeleineernst   (501) staff       (20)        0 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/
--rw-r--r--   0 madeleineernst   (501) staff       (20)    17313 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/PKG-INFO
--rw-r--r--   0 madeleineernst   (501) staff       (20)    15337 2019-11-06 10:00:34.000000 pyMolNetEnhancer-0.1.9/README.md
-drwxr-xr-x   0 madeleineernst   (501) staff       (20)        0 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer/
--rwxr-xr-x   0 madeleineernst   (501) staff       (20)      491 2019-11-28 12:18:04.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer/__init__.py
--rw-r--r--   0 madeleineernst   (501) staff       (20)    38030 2019-11-28 12:40:54.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer/molnetenhancer.py
-drwxr-xr-x   0 madeleineernst   (501) staff       (20)        0 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer.egg-info/
--rw-r--r--   0 madeleineernst   (501) staff       (20)    17313 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer.egg-info/PKG-INFO
--rw-r--r--   0 madeleineernst   (501) staff       (20)      242 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer.egg-info/SOURCES.txt
--rw-r--r--   0 madeleineernst   (501) staff       (20)        1 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer.egg-info/dependency_links.txt
--rw-r--r--   0 madeleineernst   (501) staff       (20)       17 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/pyMolNetEnhancer.egg-info/top_level.txt
--rw-r--r--   0 madeleineernst   (501) staff       (20)       38 2019-11-28 12:41:47.000000 pyMolNetEnhancer-0.1.9/setup.cfg
--rwxr-xr-x   0 madeleineernst   (501) staff       (20)      741 2019-11-28 12:41:05.000000 pyMolNetEnhancer-0.1.9/setup.py
+drwxr-xr-x   0 madeleineernst   (501) staff       (20)        0 2023-08-07 12:59:54.000000 pyMolNetEnhancer-0.2.0/
+-rw-r--r--   0 madeleineernst   (501) staff       (20)    17313 2023-08-07 12:59:54.000000 pyMolNetEnhancer-0.2.0/PKG-INFO
+-rw-r--r--   0 madeleineernst   (501) staff       (20)    15337 2023-08-07 12:58:32.000000 pyMolNetEnhancer-0.2.0/README.md
+drwxr-xr-x   0 madeleineernst   (501) staff       (20)        0 2023-08-07 12:59:54.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer/
+-rwxr-xr-x   0 madeleineernst   (501) staff       (20)      491 2023-08-07 12:58:32.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer/__init__.py
+-rw-r--r--   0 madeleineernst   (501) staff       (20)    38124 2023-08-07 12:58:32.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer/molnetenhancer.py
+drwxr-xr-x   0 madeleineernst   (501) staff       (20)        0 2023-08-07 12:59:54.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer.egg-info/
+-rw-r--r--   0 madeleineernst   (501) staff       (20)    17313 2023-08-07 12:59:53.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer.egg-info/PKG-INFO
+-rw-r--r--   0 madeleineernst   (501) staff       (20)      242 2023-08-07 12:59:53.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer.egg-info/SOURCES.txt
+-rw-r--r--   0 madeleineernst   (501) staff       (20)        1 2023-08-07 12:59:53.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer.egg-info/dependency_links.txt
+-rw-r--r--   0 madeleineernst   (501) staff       (20)       17 2023-08-07 12:59:53.000000 pyMolNetEnhancer-0.2.0/pyMolNetEnhancer.egg-info/top_level.txt
+-rw-r--r--   0 madeleineernst   (501) staff       (20)       38 2023-08-07 12:59:54.000000 pyMolNetEnhancer-0.2.0/setup.cfg
+-rwxr-xr-x   0 madeleineernst   (501) staff       (20)      741 2023-08-07 12:59:15.000000 pyMolNetEnhancer-0.2.0/setup.py
```

### Comparing `pyMolNetEnhancer-0.1.9/PKG-INFO` & `pyMolNetEnhancer-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMolNetEnhancer
-Version: 0.1.9
+Version: 0.2.0
 Summary: A python implementation of MolNetEnhancer
 Home-page: https://github.com/madeleineernst/pyMolNetEnhancer
 Author: Madeleine Ernst, Ming Wang, Ricardo Silva
 Author-email: mernst@ucsd.edu
 License: UNKNOWN
 Description: # pyMolNetEnhancer
```

### Comparing `pyMolNetEnhancer-0.1.9/README.md` & `pyMolNetEnhancer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyMolNetEnhancer-0.1.9/pyMolNetEnhancer/molnetenhancer.py` & `pyMolNetEnhancer-0.2.0/pyMolNetEnhancer/molnetenhancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from collections import OrderedDict
 import csv  
 import functools
 from functools import reduce
 from joblib import Parallel, delayed
 import json
 import multiprocessing
-from networkx import *
+import networkx as nx
 import operator
 import pandas as pd
 from pandas.api.types import is_numeric_dtype
 import requests
 import requests_cache
 
 pd.options.mode.chained_assignment = None 
@@ -43,15 +43,15 @@
     :param overlap: Minimal overlap score for a Mass2Motif to be included
     :type overlap: float
     :param top: Specifies how many most shared motifs per molecular family (network component index) should be shown
     :type top: int
     :return: A dictionary of two dataframes containing network nodes and edges with motifs mapped
     :rtype: dict
 
-    """	
+    """ 
     motifs = motifs[motifs.probability > prob]
     motifs = motifs[motifs.overlap > overlap]
     
     if 'MEH' not in edges.columns and 'OtherScore' not in edges.columns:
         edges['MEH'] = 0.0 
         edges['OtherScore'] = 0.0
     
@@ -93,23 +93,23 @@
     cols = edges.columns
     lst = []
 
     for index, row in edges.iterrows():
         if row['shared_motifs'] != 'None':
             for idx,val in enumerate(row['shared_motifs']):
                 if 'EdgeAnnotation' not in edges.columns:
-                	lst.append([row['CLUSTERID1'],row['shared_motifs'][idx],row['CLUSTERID2'], 
+                    lst.append([row['CLUSTERID1'],row['shared_motifs'][idx],row['CLUSTERID2'], 
                         row['DeltaMZ'], row['MEH'], row['Cosine'], row['OtherScore'],row['ComponentIndex'],row['shared_motifs'], row['TopSharedMotifs']])
                 else:
-                	lst.append([row['CLUSTERID1'],row['shared_motifs'][idx],row['CLUSTERID2'], 
+                    lst.append([row['CLUSTERID1'],row['shared_motifs'][idx],row['CLUSTERID2'], 
                         row['DeltaMZ'], row['MEH'], row['Cosine'], row['OtherScore'],row['ComponentIndex'],row['EdgeAnnotation'],row['shared_motifs'], row['TopSharedMotifs']])
 
 
     motifedges = pd.DataFrame(lst, columns=cols)
-    edges = edges.append(motifedges)
+    edges = pd.concat([edges,motifedges])
     
     return {'nodes':comb,'edges':edges}
 
 def make_inchidic(smilesdic):
     """Convert a dictionary of SMILES to a dictionary of InChIKeys
 
     :param smilesdic: A dictionary of SMILES
@@ -150,16 +150,16 @@
     """
     # combine SMILES for same feature into one string of features
     for index, item in enumerate(matches):
         if 'Scan' in matches[index].columns:
             matches[index] = matches[index].groupby('Scan', as_index=False).agg(lambda x: ','.join(set(x.dropna()))) 
             matches[index] = matches[index].rename(columns = {'Scan':'cluster.index'})
         if '#Scan#' in matches[index].columns:
-        	matches[index] = matches[index].groupby('#Scan#', as_index=False).agg(lambda x: ','.join(set(x.dropna())))
-        	matches[index] = matches[index].rename(columns = {'#Scan#':'cluster.index'})
+            matches[index] = matches[index].groupby('#Scan#', as_index=False).agg(lambda x: ','.join(set(x.dropna())))
+            matches[index] = matches[index].rename(columns = {'#Scan#':'cluster.index'})
             
     comb = reduce(lambda left,right: pd.merge(left,right,on='cluster.index', how = "outer"), matches)
     if 'FusionSMILES' in comb.columns:
         comb = comb.drop(['FusionSMILES', 'ConsensusSMILES'], axis=1)
     
     # concatenate all SMILES
     comb['AllSmiles'] = comb.filter(regex='^.*(Smiles|SMILES).*$').apply(lambda x: ','.join([y for y in x.tolist() if str(y) != 'nan']), axis=1)
@@ -198,17 +198,17 @@
     # combine SMILES for same feature into one string features
     #for index, item in enumerate(matches):
         #if 'Scan' in matches[index].columns:
            # matches[index] = matches[index].groupby('Scan', as_index=False).agg(lambda x: ','.join(set(x.dropna()))) 
            # matches[index] = matches[index].rename(columns = {'Scan':'cluster.index'})
             
     for index, item in enumerate(matches):
-    	if 'Scan' in matches[index].columns:
-        	matches[index] = matches[index].groupby('Scan', as_index=False).agg(lambda x: ';'.join(map(str,x)) if is_numeric_dtype(x) else ';'.join(set(x.dropna()))) 
-        	matches[index] = matches[index].rename(columns = {'Scan':'cluster.index'})
+        if 'Scan' in matches[index].columns:
+            matches[index] = matches[index].groupby('Scan', as_index=False).agg(lambda x: ';'.join(map(str,x)) if is_numeric_dtype(x) else ';'.join(set(x.dropna()))) 
+            matches[index] = matches[index].rename(columns = {'Scan':'cluster.index'})
             
     comb = reduce(lambda left,right: pd.merge(left,right,on='cluster.index', how = "outer"), matches)
     if 'FusionSMILES' in comb.columns:
         comb = comb.drop(['FusionSMILES', 'ConsensusSMILES'], axis=1)
     
     # concatenate all SMILES
     comb['All_INCHIS'] = comb.filter(regex='^.*(INCHI).*$').apply(lambda x: ';'.join([y for y in x.tolist() if str(y) != 'nan']), axis=1)
@@ -873,33 +873,33 @@
             sp[-2] += suffix
             write_path = '.'.join(sp)
         else:
             write_path += suffix
     return write_path
 
 def run_shell_command(script_to_run):
-	os.system(script_to_run)
-	return "DONE"
+    os.system(script_to_run)
+    return "DONE"
 
 # Wraps running in parallel a set of shell scripts
 def run_parallel_shellcommands(input_shell_commands, parallelism_level):
-	return run_parallel_job(run_shell_command, input_shell_commands, parallelism_level)
+    return run_parallel_job(run_shell_command, input_shell_commands, parallelism_level)
 
 # Wraps the parallel job running, simplifying code
 def run_parallel_job(input_function, input_parameters_list, parallelism_level):
-	if parallelism_level == 1:
-		output_results_list = []
-		for input_param in input_parameters_list:
-			result_object = input_function(input_param)
-			output_results_list.append(result_object)
-		return output_results_list
-	else:
-		results = Parallel(n_jobs = parallelism_level)(delayed(input_function)(input_object) for input_object in input_parameters_list)
-		return results
-		
+    if parallelism_level == 1:
+        output_results_list = []
+        for input_param in input_parameters_list:
+            result_object = input_function(input_param)
+            output_results_list.append(result_object)
+        return output_results_list
+    else:
+        results = Parallel(n_jobs = parallelism_level)(delayed(input_function)(input_object) for input_object in input_parameters_list)
+        return results
+        
 def get_classifications(inchifile):
 
     with open(inchifile) as csvfile:
         all_inchi_keys = []
     
         reader = csv.DictReader(csvfile)
         row_count = 0
```

### Comparing `pyMolNetEnhancer-0.1.9/pyMolNetEnhancer.egg-info/PKG-INFO` & `pyMolNetEnhancer-0.2.0/pyMolNetEnhancer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMolNetEnhancer
-Version: 0.1.9
+Version: 0.2.0
 Summary: A python implementation of MolNetEnhancer
 Home-page: https://github.com/madeleineernst/pyMolNetEnhancer
 Author: Madeleine Ernst, Ming Wang, Ricardo Silva
 Author-email: mernst@ucsd.edu
 License: UNKNOWN
 Description: # pyMolNetEnhancer
```

### Comparing `pyMolNetEnhancer-0.1.9/setup.py` & `pyMolNetEnhancer-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyMolNetEnhancer",
-    version="0.1.9",
+    version="0.2.0",
     author="Madeleine Ernst, Ming Wang, Ricardo Silva",
     author_email="mernst@ucsd.edu",
     description="A python implementation of MolNetEnhancer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/madeleineernst/pyMolNetEnhancer",
     packages=setuptools.find_packages(),
```

