# Comparing `tmp/boxhed_prep-2.45.tar.gz` & `tmp/boxhed_prep-2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxhed_prep-2.45.tar", last modified: Sat Jan 14 01:58:09 2023, max compression
+gzip compressed data, was "boxhed_prep-2.46.tar", last modified: Mon Aug  7 19:26:36 2023, max compression
```

## Comparing `boxhed_prep-2.45.tar` & `boxhed_prep-2.46.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-01-14 01:58:09.115537 boxhed_prep-2.45/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       31 2023-01-14 00:31:55.000000 boxhed_prep-2.45/MANIFEST.in
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      134 2023-01-14 01:58:09.115537 boxhed_prep-2.45/PKG-INFO
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-01-14 01:58:09.115537 boxhed_prep-2.45/boxhed_prep/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      527 2023-01-14 00:31:55.000000 boxhed_prep-2.45/boxhed_prep/CMakeLists.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    29296 2023-01-14 00:33:57.000000 boxhed_prep-2.45/boxhed_prep/boxhed_prep.cpp
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)     2732 2023-01-14 00:31:55.000000 boxhed_prep-2.45/boxhed_prep/boxhed_prep.h
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)    16956 2023-01-14 00:31:55.000000 boxhed_prep-2.45/boxhed_prep/boxhed_prep.py
-drwxrwxr-x   0 a.pakbin (127003716) a.pakbin (127003716)        0 2023-01-14 01:58:09.115537 boxhed_prep-2.45/boxhed_prep.egg-info/
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      134 2023-01-14 01:58:09.000000 boxhed_prep-2.45/boxhed_prep.egg-info/PKG-INFO
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      346 2023-01-14 01:58:09.000000 boxhed_prep-2.45/boxhed_prep.egg-info/SOURCES.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-01-14 01:58:09.000000 boxhed_prep-2.45/boxhed_prep.egg-info/dependency_links.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)        1 2023-01-14 01:58:09.000000 boxhed_prep-2.45/boxhed_prep.egg-info/not-zip-safe
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       19 2023-01-14 01:58:09.000000 boxhed_prep-2.45/boxhed_prep.egg-info/requires.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       12 2023-01-14 01:58:09.000000 boxhed_prep-2.45/boxhed_prep.egg-info/top_level.txt
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)       38 2023-01-14 01:58:09.115537 boxhed_prep-2.45/setup.cfg
--rw-rw-r--   0 a.pakbin (127003716) a.pakbin (127003716)      396 2023-01-14 01:57:20.000000 boxhed_prep-2.45/setup.py
+drwxr-xr-x   0 a.pakbin (45888) xrdp       (130)        0 2023-08-07 19:26:36.145477 boxhed_prep-2.46/
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)       31 2023-07-21 21:06:25.000000 boxhed_prep-2.46/MANIFEST.in
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)      134 2023-08-07 19:26:36.149477 boxhed_prep-2.46/PKG-INFO
+drwxr-xr-x   0 a.pakbin (45888) xrdp       (130)        0 2023-08-07 19:26:36.145477 boxhed_prep-2.46/boxhed_prep/
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)      527 2023-07-21 21:06:25.000000 boxhed_prep-2.46/boxhed_prep/CMakeLists.txt
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)    28966 2023-08-02 00:33:33.000000 boxhed_prep-2.46/boxhed_prep/boxhed_prep.cpp
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)     2732 2023-07-21 21:06:25.000000 boxhed_prep-2.46/boxhed_prep/boxhed_prep.h
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)    16940 2023-08-02 00:30:51.000000 boxhed_prep-2.46/boxhed_prep/boxhed_prep.py
+drwxr-xr-x   0 a.pakbin (45888) xrdp       (130)        0 2023-08-07 19:26:36.145477 boxhed_prep-2.46/boxhed_prep.egg-info/
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)      134 2023-08-07 19:26:36.000000 boxhed_prep-2.46/boxhed_prep.egg-info/PKG-INFO
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)      346 2023-08-07 19:26:36.000000 boxhed_prep-2.46/boxhed_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)        1 2023-08-07 19:26:36.000000 boxhed_prep-2.46/boxhed_prep.egg-info/dependency_links.txt
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)        1 2023-08-07 19:26:06.000000 boxhed_prep-2.46/boxhed_prep.egg-info/not-zip-safe
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)       19 2023-08-07 19:26:36.000000 boxhed_prep-2.46/boxhed_prep.egg-info/requires.txt
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)       12 2023-08-07 19:26:36.000000 boxhed_prep-2.46/boxhed_prep.egg-info/top_level.txt
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)       38 2023-08-07 19:26:36.149477 boxhed_prep-2.46/setup.cfg
+-rw-r--r--   0 a.pakbin (45888) xrdp       (130)      396 2023-08-07 19:23:35.000000 boxhed_prep-2.46/setup.py
```

### Comparing `boxhed_prep-2.45/boxhed_prep/CMakeLists.txt` & `boxhed_prep-2.46/boxhed_prep/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `boxhed_prep-2.45/boxhed_prep/boxhed_prep.cpp` & `boxhed_prep-2.46/boxhed_prep/boxhed_prep.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -470,51 +470,42 @@
 inline void _compute_quant(const T* data, size_t nrows, size_t ncols, const bool* is_cat, size_t t_start_idx, size_t t_end_idx, size_t id_idx, size_t delta_idx, T* quant, size_t* quant_size, size_t num_quantiles){
  
     #pragma omp parallel for schedule(dynamic)
     for (size_t col_idx = 0; col_idx<ncols; ++col_idx){
         if (is_cat[col_idx] || col_idx == t_end_idx || col_idx == id_idx || col_idx == delta_idx){
             continue;
         }
-        size_t vals_size = (col_idx==t_start_idx) ? 2*nrows : nrows;
+        size_t vals_size = (col_idx==t_start_idx) ? 2*nrows+1 : nrows;
         //vals_size       += 1;
 
         /*
         T vals [vals_size];
         */
         T *vals = new T[vals_size];
 
         _copy_col2arr(data, nrows, ncols, col_idx, vals);
         if (col_idx == t_start_idx){
             _copy_col2arr(data, nrows, ncols, t_end_idx, vals + nrows);
+            vals[2*nrows] = 0;
         }
 
         //vals[vals_size-1] = (col_idx==t_start_idx) ? 0 : _nan_min(vals, vals_size-1)-1;
 
         size_t num_non_nan;
         _rmv_nans(vals, vals_size, &num_non_nan);
         std::stable_sort(vals, vals + num_non_nan);
 
         size_t num_unique;
         _rmv_dupl_srtd<T>(vals, num_non_nan, &num_unique);
 
-        size_t num_quants = std::min(num_unique, num_quantiles-1);
-        quant_size [col_idx] = num_quants;
-
-        size_t offset;
-        if (((col_idx==t_start_idx)) && (vals[0]==0)){
-            offset                       = 0;
-        } else {
-            quant[col_idx*num_quantiles] = (col_idx==t_start_idx) ? 0 : _nan_min(vals, vals_size-1)-1;
-            offset                       = 1;
-            quant_size [col_idx]        += 1;
-        }
-        
+        size_t num_quants = std::min(num_unique, num_quantiles);
+        quant_size [col_idx] = num_quants;  
 
         for (size_t i=0; i<num_quants; ++i){
-            quant[col_idx*num_quantiles+i+offset] = vals[static_cast<int>(num_unique*i/num_quants)];
+            quant[col_idx*num_quantiles+i] = vals[static_cast<int>(num_unique*i/num_quants)];
         }
         delete [] vals;
                 
     }
 
 }
```

### Comparing `boxhed_prep-2.45/boxhed_prep/boxhed_prep.h` & `boxhed_prep-2.46/boxhed_prep/boxhed_prep.h`

 * *Files identical despite different names*

### Comparing `boxhed_prep-2.45/boxhed_prep/boxhed_prep.py` & `boxhed_prep-2.46/boxhed_prep/boxhed_prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
                 
             \textbf{delta}: equals one if an event occurred at the end of the epoch; zero otherwise.
         :rtype: pd.Series, pd.DataFrame, pd.Series, pd.Series
         """
 
         #XXX: using np.float64---c_double
         self.nthread            = nthread
-        self.num_quantiles      = num_quantiles+1#min(num_quantiles, 256)
+        self.num_quantiles      = min(num_quantiles, 256)
         self.weighted           = weighted
         _is_cat                 = self._contig_bool(np.zeros((1, data.shape[1])))
         for cat_col in is_cat:
             _is_cat[0, cat_col] = True
         self.is_cat             = _is_cat
         nrows                   = data.shape[0]
         self.ncols              = data.shape[1]
```

