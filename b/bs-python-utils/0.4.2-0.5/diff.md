# Comparing `tmp/bs_python_utils-0.4.2.tar.gz` & `tmp/bs_python_utils-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.4.2.tar", max compression
+gzip compressed data, was "bs_python_utils-0.5.tar", max compression
```

## Comparing `bs_python_utils-0.4.2.tar` & `bs_python_utils-0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-07-25 18:18:48.273804 bs_python_utils-0.4.2/LICENSE
--rw-r--r--   0        0        0     1909 2023-08-02 17:45:46.755089 bs_python_utils-0.4.2/README.md
--rw-r--r--   0        0        0     1799 2023-07-25 18:18:48.274334 bs_python_utils-0.4.2/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-07-25 18:18:48.274376 bs_python_utils-0.4.2/bs_python_utils/__init__.py
--rw-r--r--   0        0        0     9123 2023-08-02 17:29:19.470519 bs_python_utils-0.4.2/bs_python_utils/bivariate_quantiles.py
--rw-r--r--   0        0        0    28473 2023-07-25 18:18:48.274727 bs_python_utils-0.4.2/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-07-25 18:18:48.274839 bs_python_utils-0.4.2/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-07-25 18:18:48.274920 bs_python_utils-0.4.2/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-07-25 18:18:48.275009 bs_python_utils-0.4.2/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    15009 2023-07-25 18:18:48.275181 bs_python_utils-0.4.2/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-07-25 18:18:48.275258 bs_python_utils-0.4.2/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-07-25 18:18:48.275357 bs_python_utils-0.4.2/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     2201 2023-08-02 17:22:32.496441 bs_python_utils-0.4.2/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-07-25 18:18:48.275517 bs_python_utils-0.4.2/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    33587 2023-07-25 18:18:48.275734 bs_python_utils-0.4.2/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-07-25 18:18:48.275838 bs_python_utils-0.4.2/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    14053 2023-08-02 17:44:39.345131 bs_python_utils-0.4.2/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9471 2023-07-25 18:18:48.276116 bs_python_utils-0.4.2/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0    14016 2023-07-25 18:18:48.276224 bs_python_utils-0.4.2/bs_python_utils/chebyshev.py
--rw-r--r--   0        0        0     7801 2023-07-25 18:18:48.276337 bs_python_utils-0.4.2/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-07-25 18:18:48.276417 bs_python_utils-0.4.2/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-07-25 18:18:48.276493 bs_python_utils-0.4.2/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-07-25 18:18:48.276564 bs_python_utils-0.4.2/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-07-25 18:18:48.276629 bs_python_utils-0.4.2/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-07-25 18:18:48.276695 bs_python_utils-0.4.2/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-07-25 18:18:48.276775 bs_python_utils-0.4.2/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-07-25 18:18:48.276867 bs_python_utils-0.4.2/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-07-25 18:18:48.276931 bs_python_utils-0.4.2/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1890 2023-08-02 17:23:55.728156 bs_python_utils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 bs_python_utils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 18:18:48.273804 bs_python_utils-0.5/LICENSE
+-rw-r--r--   0        0        0     1991 2023-08-07 20:03:46.878133 bs_python_utils-0.5/README.md
+-rw-r--r--   0        0        0     1799 2023-07-25 18:18:48.274334 bs_python_utils-0.5/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-07-25 18:18:48.274376 bs_python_utils-0.5/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0     9123 2023-08-02 17:29:19.000000 bs_python_utils-0.5/bs_python_utils/bivariate_quantiles.py
+-rw-r--r--   0        0        0    28473 2023-07-25 18:18:48.274727 bs_python_utils-0.5/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-07-25 18:18:48.274839 bs_python_utils-0.5/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-07-25 18:18:48.274920 bs_python_utils-0.5/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-07-25 18:18:48.275009 bs_python_utils-0.5/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    15009 2023-07-25 18:18:48.275181 bs_python_utils-0.5/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-07-25 18:18:48.275258 bs_python_utils-0.5/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-07-25 18:18:48.275357 bs_python_utils-0.5/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     2201 2023-08-02 17:22:32.000000 bs_python_utils-0.5/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-07-25 18:18:48.275517 bs_python_utils-0.5/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    33587 2023-07-25 18:18:48.275734 bs_python_utils-0.5/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-07-25 18:18:48.275838 bs_python_utils-0.5/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    14053 2023-08-02 17:44:39.000000 bs_python_utils-0.5/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-07-25 18:18:48.276116 bs_python_utils-0.5/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0    15050 2023-08-07 20:02:40.667050 bs_python_utils-0.5/bs_python_utils/chebyshev.py
+-rw-r--r--   0        0        0     7801 2023-07-25 18:18:48.276337 bs_python_utils-0.5/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-07-25 18:18:48.276417 bs_python_utils-0.5/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-07-25 18:18:48.276493 bs_python_utils-0.5/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-07-25 18:18:48.276564 bs_python_utils-0.5/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-07-25 18:18:48.276629 bs_python_utils-0.5/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-07-25 18:18:48.276695 bs_python_utils-0.5/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-07-25 18:18:48.276775 bs_python_utils-0.5/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-07-25 18:18:48.276867 bs_python_utils-0.5/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-07-25 18:18:48.276931 bs_python_utils-0.5/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1888 2023-08-07 19:57:21.410538 bs_python_utils-0.5/pyproject.toml
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 bs_python_utils-0.5/PKG-INFO
```

### Comparing `bs_python_utils-0.4.2/LICENSE` & `bs_python_utils-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/README.md` & `bs_python_utils-0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
+#### 0.5 (August 7, 2023)
+Added 1-dimensional root finding in `chebyshev` module.
 #### 0.4.2 (August 2, 2023)
 Updated the docs.
 #### 0.4.1 (July 23, 2023)
 Only print if verbose in bivariate quantiles.
 #### 0.4 (July 22, 2023)
 Added bivariate quantiles and ranks à la optimal transportation.
 #### 0.3 (July 21, 2023)
```

### Comparing `bs_python_utils-0.4.2/bs_python_utils/Timer.py` & `bs_python_utils-0.5/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bivariate_quantiles.py` & `bs_python_utils-0.5/bs_python_utils/bivariate_quantiles.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_altair.py` & `bs_python_utils-0.5/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_logging.py` & `bs_python_utils-0.5/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.5/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_mem.py` & `bs_python_utils-0.5/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_opt.py` & `bs_python_utils-0.5/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.5/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.5/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.5/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bsnputils.py` & `bs_python_utils-0.5/bs_python_utils/bsnputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bssputils.py` & `bs_python_utils-0.5/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bsstats.py` & `bs_python_utils-0.5/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/bsutils.py` & `bs_python_utils-0.5/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/chebyshev.py` & `bs_python_utils-0.5/bs_python_utils/chebyshev.py`

 * *Files 9% similar despite different names*

```diff
@@ -165,14 +165,43 @@
         degree = cast(int, degree)
         fun = cast(ArrayFunctionOfArray, fun)
         c = cheb_get_coefficients_1d(fun, interval, degree)
     y_vals = ncheb.chebval(move_to1m1(x_vals, interval), c)
     return y_vals, c
 
 
+def cheb_find_root(
+    f: ArrayFunctionOfArray, degree: int, interval: Interval | None = None
+) -> np.ndarray | tuple[np.ndarray, np.ndarray | float | None]:
+    """find the roots of $f(x)=0$ in $[0,1]$; also return the one(s) within the interval, if given
+
+    Args:
+        f: the function
+        degree: the degree of the Chebyshev expansion
+        interval: the interval where we want the root
+
+    Returns:
+        the roots in $[0,1]$;  and the one(s) in `interval`, if specified
+    """
+    interval01 = Interval(0.0, 1.0)
+    coeffs_f = cheb_get_coefficients_1d(f, interval01, degree)
+    roots = cast(np.ndarray, move_from1m1(ncheb.chebroots(coeffs_f), interval01))
+
+    if interval:
+        roots_in_interval = roots[(roots >= interval.x0) & (roots <= interval.x1)]
+        if len(roots_in_interval) == 0:
+            return roots, None
+        elif len(roots_in_interval) == 1:
+            return roots, roots_in_interval[0]
+        else:
+            return roots, roots_in_interval
+    else:
+        return roots
+
+
 def cheb_integrate_from_coeffs_1d(c: np.ndarray, interval: Interval) -> float:
     """integrate a function on an interval using the coefficients of its Chebyshev expansion
 
     Args:
         c: the Chebyshev coefficients for `fun`
         interval: the Interval
 
@@ -393,15 +422,15 @@
     Args:
         vals_at_nodes: the values of the function on the grid of 2d nodes
         weights: the Chebyshev weights in 2d
 
     Returns:
         the value of the integral
 
-    Notes:
+    Warning:
         this is much less precise than `cheb_integrate_from_coeffs_2d`
     """
     Mv = check_vector(vals_at_nodes)
     Mw = check_vector(weights)
     if Mv != Mw:
         bs_error_abort(
             f"weights and vals_at_nodes must have the same length, not {Mw} and {Mv}"
@@ -417,15 +446,15 @@
     Args:
         vals_at_nodes4d: the values of the function on the square of the grid of 2d nodes, an $(M^2, M^2)$ matrix
         weights2d: the Chebyshev weights on the rectangular grid, an $M^2$-vector
 
     Returns:
         the value of the integral
 
-    Notes:
+    Warning:
         it would be better to have a `cheb_integrate_from_coeffs_4d`
     """
     Mv2 = check_square(vals_at_nodes4d)
     Mw2 = check_vector(weights2d)
     if Mv2 != Mw2:
         bs_error_abort(
             "weights2d and vals_at_nodes4d should have the same number of rows, not"
```

### Comparing `bs_python_utils-0.4.2/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.5/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/example_opt.py` & `bs_python_utils-0.5/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/examples_altair.py` & `bs_python_utils-0.5/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.5/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/examples_mem.py` & `bs_python_utils-0.5/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.5/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.5/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.5/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.5/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.4.2/pyproject.toml` & `bs_python_utils-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.4.2"
+version = "0.5"
 description = "my Python utilities"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.4.2/PKG-INFO` & `bs_python_utils-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.4.2
+Version: 0.5
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -33,14 +33,16 @@
 
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
+#### 0.5 (August 7, 2023)
+Added 1-dimensional root finding in `chebyshev` module.
 #### 0.4.2 (August 2, 2023)
 Updated the docs.
 #### 0.4.1 (July 23, 2023)
 Only print if verbose in bivariate quantiles.
 #### 0.4 (July 22, 2023)
 Added bivariate quantiles and ranks à la optimal transportation.
 #### 0.3 (July 21, 2023)
```

