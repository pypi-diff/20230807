# Comparing `tmp/ccs_fit-0.21.9.tar.gz` & `tmp/ccs_fit-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs_fit-0.21.9.tar", max compression
+gzip compressed data, was "ccs_fit-0.22.0.tar", max compression
```

## Comparing `ccs_fit-0.21.9.tar` & `ccs_fit-0.22.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-08-03 12:56:44.579397 ccs_fit-0.21.9/LICENSE
--rw-r--r--   0        0        0     7898 2023-08-03 12:56:44.579397 ccs_fit-0.21.9/README.md
--rw-r--r--   0        0        0     2483 2023-08-03 12:57:23.048105 ccs_fit-0.21.9/pyproject.toml
--rw-r--r--   0        0        0     1027 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/__init__.py
--rw-r--r--   0        0        0     9636 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/ase_calculator/buck.py
--rw-r--r--   0        0        0     8028 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
--rw-r--r--   0        0        0    10653 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
--rw-r--r--   0        0        0      488 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/__init__.py
--rw-r--r--   0        0        0      628 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/exceptions.py
--rw-r--r--   0        0        0     1476 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/io.py
--rw-r--r--   0        0        0      486 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/math/__init__.py
--rw-r--r--   0        0        0     1071 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/math/ewald.py
--rw-r--r--   0        0        0     2156 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/common/neighborlist.py
--rw-r--r--   0        0        0      488 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/data/__init__.py
--rw-r--r--   0        0        0      854 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/data/conversion.py
--rw-r--r--   0        0        0      805 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/debugging_tools/timing.py
--rw-r--r--   0        0        0      488 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/fitting/__init__.py
--rw-r--r--   0        0        0    13479 2023-08-03 12:56:45.563438 ccs_fit-0.21.9/src/ccs_fit/fitting/main copy.py
--rw-r--r--   0        0        0    14597 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/fitting/main.py
--rw-r--r--   0        0        0    23897 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/fitting/objective.py
--rw-r--r--   0        0        0    11717 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/fitting/spline_functions.py
--rw-r--r--   0        0        0    20046 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/ppmd_interface/ccs_ppmd.py
--rw-r--r--   0        0        0     6913 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/regression_tool/regression.py
--rw-r--r--   0        0        0      488 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/__init__.py
--rw-r--r--   0        0        0     7361 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db copy.py
--rw-r--r--   0        0        0     7229 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db.py
--rw-r--r--   0        0        0     8555 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_FF.py
--rw-r--r--   0        0        0     4155 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_sktable.py
--rw-r--r--   0        0        0     8623 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fetch.py
--rw-r--r--   0        0        0     2537 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fit.py
--rw-r--r--   0        0        0     6482 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_prune.py
--rw-r--r--   0        0        0     6754 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_validate.py
--rw-r--r--   0        0        0     1784 2023-08-03 12:56:45.567438 ccs_fit-0.21.9/src/ccs_fit/scripts/jsonTotable.py
--rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 ccs_fit-0.21.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-07 14:25:50.869181 ccs_fit-0.22.0/LICENSE
+-rw-r--r--   0        0        0     7898 2023-08-07 14:25:50.869181 ccs_fit-0.22.0/README.md
+-rw-r--r--   0        0        0     2483 2023-08-07 14:26:28.409136 ccs_fit-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0     1027 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/__init__.py
+-rw-r--r--   0        0        0     9636 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/ase_calculator/buck.py
+-rw-r--r--   0        0        0     8028 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
+-rw-r--r--   0        0        0    10653 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
+-rw-r--r--   0        0        0      488 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/common/__init__.py
+-rw-r--r--   0        0        0      628 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/common/exceptions.py
+-rw-r--r--   0        0        0     1476 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/common/io.py
+-rw-r--r--   0        0        0      486 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/common/math/__init__.py
+-rw-r--r--   0        0        0     1071 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/common/math/ewald.py
+-rw-r--r--   0        0        0     2156 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/common/neighborlist.py
+-rw-r--r--   0        0        0      488 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/data/__init__.py
+-rw-r--r--   0        0        0      854 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/data/conversion.py
+-rw-r--r--   0        0        0      805 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/debugging_tools/timing.py
+-rw-r--r--   0        0        0      488 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/fitting/__init__.py
+-rw-r--r--   0        0        0    13479 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/fitting/main copy.py
+-rw-r--r--   0        0        0    14597 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/fitting/main.py
+-rw-r--r--   0        0        0    24221 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/fitting/objective.py
+-rw-r--r--   0        0        0    11717 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/fitting/spline_functions.py
+-rw-r--r--   0        0        0    20046 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/ppmd_interface/ccs_ppmd.py
+-rw-r--r--   0        0        0     6913 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/regression_tool/regression.py
+-rw-r--r--   0        0        0      488 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/__init__.py
+-rw-r--r--   0        0        0     7361 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_build_db copy.py
+-rw-r--r--   0        0        0     7229 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_build_db.py
+-rw-r--r--   0        0        0     8555 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_export_FF.py
+-rw-r--r--   0        0        0     4155 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_export_sktable.py
+-rw-r--r--   0        0        0     8623 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_fetch.py
+-rw-r--r--   0        0        0     2537 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_fit.py
+-rw-r--r--   0        0        0     6482 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_prune.py
+-rw-r--r--   0        0        0     6754 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_validate.py
+-rw-r--r--   0        0        0     1784 2023-08-07 14:25:51.905181 ccs_fit-0.22.0/src/ccs_fit/scripts/jsonTotable.py
+-rw-r--r--   0        0        0     9123 1970-01-01 00:00:00.000000 ccs_fit-0.22.0/PKG-INFO
```

### Comparing `ccs_fit-0.21.9/LICENSE` & `ccs_fit-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/README.md` & `ccs_fit-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/pyproject.toml` & `ccs_fit-0.22.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ccs_fit"
-version = "0.21.9"
+version = "0.22.0"
 description = "Fitting tools for repulsive two body interactions using curvature constrained splines."
 authors = [
     "Akshay Krishna AK",
     "Jolla Kullgren <jolla.kullgren@kemi.uu.se>",
     "Eddie Wadbro <eddie.wadbro@umu.se>"
     ]
 maintainers = [
```

### Comparing `ccs_fit-0.21.9/src/ccs_fit/__init__.py` & `ccs_fit-0.22.0/src/ccs_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/ase_calculator/buck.py` & `ccs_fit-0.22.0/src/ccs_fit/ase_calculator/buck.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_G2B.py` & `ccs_fit-0.22.0/src/ccs_fit/ase_calculator/ccs_ase_G2B.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/ase_calculator/ccs_ase_calculator.py` & `ccs_fit-0.22.0/src/ccs_fit/ase_calculator/ccs_ase_calculator.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/common/exceptions.py` & `ccs_fit-0.22.0/src/ccs_fit/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/common/io.py` & `ccs_fit-0.22.0/src/ccs_fit/common/io.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/common/math/ewald.py` & `ccs_fit-0.22.0/src/ccs_fit/common/math/ewald.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/common/neighborlist.py` & `ccs_fit-0.22.0/src/ccs_fit/common/neighborlist.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/data/conversion.py` & `ccs_fit-0.22.0/src/ccs_fit/data/conversion.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/debugging_tools/timing.py` & `ccs_fit-0.22.0/src/ccs_fit/debugging_tools/timing.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/fitting/main copy.py` & `ccs_fit-0.22.0/src/ccs_fit/fitting/main copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/fitting/main.py` & `ccs_fit-0.22.0/src/ccs_fit/fitting/main.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/fitting/objective.py` & `ccs_fit-0.22.0/src/ccs_fit/fitting/objective.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,14 +176,24 @@
 
         # logger.info(
         #     "\n The best switch is : %s with mse: %s", *
         #     nswitch_list[opt_sol_index], mse
         # )
         best_switch_r = np.around([nswitch_list[opt_sol_index][elem]*self.l_twb[elem].res+self.l_twb[elem].Rmin for elem in range(self.np)], decimals=2)
         elem_pairs = [self.l_twb[elem].name for elem in range(self.np)]
+
+        best_switch_dict = {}
+        for i, elem_pair, in enumerate(elem_pairs):
+            best_switch_dict[elem_pair] =  best_switch_r[i]
+
+        results_dict = {"rmse": mse**0.5, "best_switches": best_switch_dict}
+        
+        with open("rmse.json", "w") as outfile:
+            json.dump(results_dict, outfile)
+
         print(
             f"    The best switch is {nswitch_list[opt_sol_index][:]} with rmse: {mse**0.5}, corresponding to distances of {best_switch_r} Å for element pairs {elem_pairs[:]}.")
 
         # [{' '.join(['{:2f}'.format(best_switch_r[elem]) for elem in range(self.np)])}]
 
         [g_opt, aa] = self.get_g(nswitch_list[opt_sol_index])
         bb = np.zeros(aa.shape[0])
```

### Comparing `ccs_fit-0.21.9/src/ccs_fit/fitting/spline_functions.py` & `ccs_fit-0.22.0/src/ccs_fit/fitting/spline_functions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/ppmd_interface/ccs_ppmd.py` & `ccs_fit-0.22.0/src/ccs_fit/ppmd_interface/ccs_ppmd.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/regression_tool/regression.py` & `ccs_fit-0.22.0/src/ccs_fit/regression_tool/regression.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db copy.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_build_db copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_build_db.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_build_db.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_FF.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_export_FF.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_export_sktable.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_export_sktable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fetch.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_fetch.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_fit.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_fit.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_prune.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_prune.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/ccs_validate.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/ccs_validate.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/src/ccs_fit/scripts/jsonTotable.py` & `ccs_fit-0.22.0/src/ccs_fit/scripts/jsonTotable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.9/PKG-INFO` & `ccs_fit-0.22.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-fit
-Version: 0.21.9
+Version: 0.22.0
 Summary: Fitting tools for repulsive two body interactions using curvature constrained splines.
 Home-page: https://github.com/Teoroo-CMC/CCS
 License: GPL-3
 Keywords: Curvature,Constrained,Splines,Two-Body,Interatomic,Repulsive,Fitting
 Author: Akshay Krishna AK
 Maintainer: Jolla Kullgren
 Maintainer-email: jolla.kullgren@kemi.uu.se
```

