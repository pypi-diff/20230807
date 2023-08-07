# Comparing `tmp/sumt-3.2.5.tar.gz` & `tmp/sumt-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumt-3.2.5.tar", last modified: Mon Jul 31 09:22:29 2023, max compression
+gzip compressed data, was "sumt-3.2.6.tar", last modified: Mon Aug  7 11:27:28 2023, max compression
```

## Comparing `sumt-3.2.5.tar` & `sumt-3.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 09:22:29.719376 sumt-3.2.5/
--rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.5/LICENSE
--rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-07-31 09:22:29.719806 sumt-3.2.5/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)    20838 2023-07-31 09:18:33.000000 sumt-3.2.5/README.md
--rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.5/pyproject.toml
--rw-r--r--   0 agpe       (502) staff       (20)      650 2023-07-31 09:22:29.720859 sumt-3.2.5/setup.cfg
-drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-07-31 09:22:29.718740 sumt-3.2.5/sumt.egg-info/
--rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/PKG-INFO
--rw-r--r--   0 agpe       (502) staff       (20)      220 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/SOURCES.txt
--rw-r--r--   0 agpe       (502) staff       (20)        1 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/dependency_links.txt
--rw-r--r--   0 agpe       (502) staff       (20)       35 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/entry_points.txt
--rw-r--r--   0 agpe       (502) staff       (20)       28 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/requires.txt
--rw-r--r--   0 agpe       (502) staff       (20)        5 2023-07-31 09:22:29.000000 sumt-3.2.5/sumt.egg-info/top_level.txt
--rwxr-xr-x   0 agpe       (502) staff       (20)    32428 2023-07-31 09:16:44.000000 sumt-3.2.5/sumt.py
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-08-07 11:27:28.829062 sumt-3.2.6/
+-rw-r--r--   0 agpe       (502) staff       (20)    35149 2022-02-20 16:31:26.000000 sumt-3.2.6/LICENSE
+-rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-08-07 11:27:28.829369 sumt-3.2.6/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)    20838 2023-08-07 11:26:56.000000 sumt-3.2.6/README.md
+-rw-r--r--   0 agpe       (502) staff       (20)      104 2021-11-24 21:14:07.000000 sumt-3.2.6/pyproject.toml
+-rw-r--r--   0 agpe       (502) staff       (20)      650 2023-08-07 11:27:28.830198 sumt-3.2.6/setup.cfg
+drwxr-xr-x   0 agpe       (502) staff       (20)        0 2023-08-07 11:27:28.828728 sumt-3.2.6/sumt.egg-info/
+-rw-r--r--   0 agpe       (502) staff       (20)    21313 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/PKG-INFO
+-rw-r--r--   0 agpe       (502) staff       (20)      220 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/SOURCES.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        1 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/dependency_links.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       35 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/entry_points.txt
+-rw-r--r--   0 agpe       (502) staff       (20)       28 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/requires.txt
+-rw-r--r--   0 agpe       (502) staff       (20)        5 2023-08-07 11:27:28.000000 sumt-3.2.6/sumt.egg-info/top_level.txt
+-rwxr-xr-x   0 agpe       (502) staff       (20)    32052 2023-08-07 11:07:59.000000 sumt-3.2.6/sumt.py
```

### Comparing `sumt-3.2.5/LICENSE` & `sumt-3.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sumt-3.2.5/PKG-INFO` & `sumt-3.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.5
+Version: 3.2.6
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.5-blue)
+![](https://img.shields.io/badge/version-3.2.6-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
```

### Comparing `sumt-3.2.5/README.md` & `sumt-3.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.5-blue)
+![](https://img.shields.io/badge/version-3.2.6-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
```

### Comparing `sumt-3.2.5/setup.cfg` & `sumt-3.2.6/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sumt
-version = 3.2.5
+version = 3.2.6
 author = Anders Gorm Pedersen
 author_email = agpe@dtu.dk
 description = Computes consensus trees and other phylogenetic tree summaries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/agormp/sumt
 classifiers =
```

### Comparing `sumt-3.2.5/sumt.egg-info/PKG-INFO` & `sumt-3.2.6/sumt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: sumt
-Version: 3.2.5
+Version: 3.2.6
 Summary: Computes consensus trees and other phylogenetic tree summaries
 Home-page: https://github.com/agormp/sumt
 Author: Anders Gorm Pedersen
 Author-email: agpe@dtu.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sumt
 
-![](https://img.shields.io/badge/version-3.2.5-blue)
+![](https://img.shields.io/badge/version-3.2.6-blue)
 [![PyPI downloads](https://static.pepy.tech/personalized-badge/sumt?period=total&units=none&left_color=black&right_color=blue&left_text=PyPI%20downloads&service=github)](https://pepy.tech/project/sumt)
 
 The command-line program `sumt` computes consensus trees and other tree-summary statistics for sets of phylogenetic trees. The input trees can be in one or more input files, and will typically be from a Bayesian MCMC analysis (BEAST or MrBayes for instance) or from a bootstrap procedure. 
 
 `sumt` can compute three different kinds of main tree summaries:
 
 * Majority rule consensus tree
```

### Comparing `sumt-3.2.5/sumt.py` & `sumt-3.2.6/sumt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ####################################################################################
 ####################################################################################
 
 import phylotreelib as treelib
-import argparse, os, sys, time, math, copy, psutil
+import argparse, os, sys, time, math, copy, psutil, statistics
 from itertools import (takewhile,repeat)
 from operator import itemgetter
 from pathlib import Path
 import gc
 
 gc.disable()        # Faster. Assume no cyclic references will ever be created
 
@@ -444,51 +444,34 @@
     #       population estimates of std, and is in accordance with what MrBayes does. One could
     #       argue that N should be used instead of N-1 (to get the Max Likelihood estimate of std).
 
     sum_std = 0
     N = float(len(treesummarylist))
 
     # Find combined set of bipartitions (excluding external branches)
+    # Only biparts that have freq >= minfreq are kept
     bipset = set()
     for treesummary in treesummarylist:
-        for bipart in treesummary.bipartsummary:
+        for bipart,branch in treesummary.bipartsummary.items():
             (bip1, bip2) = bipart
-            if (len(bip1)==1 or len(bip2)==1):
-                pass
-            else:
+            if len(bip1)>1 and len(bip2)>1 and branch.freq >= minfreq:
                 bipset.add(bipart)
 
-    # Discard rare bipartitions: Only biparts that have freq >= minfreq are kept
-    bipset_keep = set()
-    for bipart in bipset:
-        for treesummary in treesummarylist:
-            try:
-                if treesummary.bipartsummary[bipart].freq >= minfreq:
-                    bipset_keep.add(bipart)
-                    break
-            except:
-                pass
-    del(bipset)
-
     # For each internal bipart: compute std of freq of this bipart across all treesummaries
-    for bipart in bipset_keep:
-
-        freqsum = 0
-        sumsq = 0
+    for bipart in bipset:
+        freqlist = []
         for treesummary in treesummarylist:
-            # If current bipartition in treesummary, add freq etc. Otherwise add zero (=do nothing)
+            # If current bipartition not in current treesummary: set freq=0.0
             if bipart in treesummary.bipartsummary:
-                freqsum += treesummary.bipartsummary[bipart].freq
-                sumsq += (treesummary.bipartsummary[bipart].freq)**2
-
-        meansq = (freqsum/N)**2
-        std = math.sqrt((sumsq-N*meansq)/(N-1))
-        sum_std += std
+                freqlist.append(treesummary.bipartsummary[bipart].freq)
+            else:
+                freqlist.append(0.0)
+        sum_std += statistics.stdev(freqlist)
 
-    ave_std = sum_std / len(bipset_keep)
+    ave_std = sum_std / len(bipset)
     return ave_std
 
 ##########################################################################################
 ##########################################################################################
 
 def  merge_treesummaries(treesummarylist):
 
@@ -497,15 +480,14 @@
         treesummary.update(treesummary2)
         del treesummary2
     return treesummary
 
 ##########################################################################################
 ##########################################################################################
 
-
 def compute_and_print_biparts(treesummary, args):
 
     # Compute and retrieve results
     (leaflist, bipreslist) = bipart_report(treesummary, args)
 
     # Before printing results: check whether files already exist
     partsfilename = args.outbase.parent / (args.outbase.name + ".parts")
@@ -531,15 +513,15 @@
                     "SEM  = Standard error of the mean for branch length\n"
                     "ID   = Leaf name or internal branch label, for those bipartitions that are included in consensus tree\n\n")
     stringwidth = len(leaflist)
     partsfile.write("PART" + (stringwidth-1)*" " + "PROB      " + "BLEN       " + "VAR          " + "SEM          " + "ID\n")
 
     for (_, _, bipstring, freq, mean, var, sem, branchID) in bipreslist:
         if var == "NA":
-            partsfile.write(f"{bipstring}   {freq:<8.6f}  {mean:<9.4g}  ({var:<9.4g})  ({sem:<9.4g})  {branchID}\n")
+            partsfile.write(f"{bipstring}   {freq:<8.6f}  {mean:<9.4g}  ({var:<9})  ({sem:<9})  {branchID}\n")
         else:
             partsfile.write(f"{bipstring}   {freq:<8.6f}  {mean:<9.4g}  ({var:<9.4g})  ({sem:<9.4g})  {branchID}\n")
     partsfile.close()
     print(f"   Bipartition list written to {partsfilename}")
 
 ##########################################################################################
 ##########################################################################################
@@ -730,9 +712,10 @@
 
     return toporeport
 
 ##########################################################################################
 ##########################################################################################
 
 if __name__ == "__main__":
-    main()
-
+    # main()
+    import cProfile
+    cProfile.run('main()', 'tmp/profile.pstats')
```

