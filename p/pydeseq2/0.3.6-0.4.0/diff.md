# Comparing `tmp/pydeseq2-0.3.6.tar.gz` & `tmp/pydeseq2-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/bmuzellec/Documents/Projects/FL_genomics/PyDESeq2/dist/.tmp-iij11kvm/pydeseq2-0.3.6.tar", last modified: Tue Aug  1 09:20:19 2023, max compression
+gzip compressed data, was "pydeseq2-0.4.0.tar", last modified: Mon Aug  7 13:20:10 2023, max compression
```

## Comparing `pydeseq2-0.3.6.tar` & `pydeseq2-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.3.6/LICENSE
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6563 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6230 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/README.md
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2/
--rw-r--r--   0 bmuzellec   (501) staff       (20)       53 2022-12-28 09:54:14.000000 pydeseq2-0.3.6/pydeseq2/__init__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2023-08-01 09:16:03.000000 pydeseq2-0.3.6/pydeseq2/__version__.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    41325 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/pydeseq2/dds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    25791 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/pydeseq2/ds.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     8480 2023-03-24 14:45:04.000000 pydeseq2-0.3.6/pydeseq2/grid_search.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1587 2023-06-01 08:36:08.000000 pydeseq2-0.3.6/pydeseq2/preprocessing.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    41248 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/pydeseq2/utils.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     6563 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/PKG-INFO
--rw-r--r--   0 bmuzellec   (501) staff       (20)      436 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/SOURCES.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/dependency_links.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      190 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/requires.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/pydeseq2.egg-info/top_level.txt
--rw-r--r--   0 bmuzellec   (501) staff       (20)      408 2023-04-05 09:20:58.000000 pydeseq2-0.3.6/pyproject.toml
--rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/setup.cfg
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1362 2023-05-02 08:07:48.000000 pydeseq2-0.3.6/setup.py
-drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-01 09:20:19.000000 pydeseq2-0.3.6/tests/
--rw-r--r--   0 bmuzellec   (501) staff       (20)     5654 2023-02-16 10:34:42.000000 pydeseq2-0.3.6/tests/test_docstring.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    12647 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/tests/test_edge_cases.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)    15705 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/tests/test_pydeseq2.py
--rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2023-08-01 09:13:46.000000 pydeseq2-0.3.6/tests/test_utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-07 13:20:10.086987 pydeseq2-0.4.0/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1062 2022-12-03 17:11:22.000000 pydeseq2-0.4.0/LICENSE
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6583 2023-08-07 13:20:10.086486 pydeseq2-0.4.0/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6250 2023-08-07 13:06:39.000000 pydeseq2-0.4.0/README.md
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-07 13:20:10.079614 pydeseq2-0.4.0/pydeseq2/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       53 2022-12-28 09:54:14.000000 pydeseq2-0.4.0/pydeseq2/__init__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       22 2023-08-07 13:10:25.000000 pydeseq2-0.4.0/pydeseq2/__version__.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    42910 2023-08-07 13:06:39.000000 pydeseq2-0.4.0/pydeseq2/dds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    27538 2023-08-07 13:06:39.000000 pydeseq2-0.4.0/pydeseq2/ds.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     8480 2023-03-24 14:45:04.000000 pydeseq2-0.4.0/pydeseq2/grid_search.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1587 2023-06-01 08:36:08.000000 pydeseq2-0.4.0/pydeseq2/preprocessing.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    43565 2023-08-07 13:06:39.000000 pydeseq2-0.4.0/pydeseq2/utils.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-07 13:20:10.082017 pydeseq2-0.4.0/pydeseq2.egg-info/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     6583 2023-08-07 13:20:10.000000 pydeseq2-0.4.0/pydeseq2.egg-info/PKG-INFO
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      436 2023-08-07 13:20:10.000000 pydeseq2-0.4.0/pydeseq2.egg-info/SOURCES.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        1 2023-08-07 13:20:10.000000 pydeseq2-0.4.0/pydeseq2.egg-info/dependency_links.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      190 2023-08-07 13:20:10.000000 pydeseq2-0.4.0/pydeseq2.egg-info/requires.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)        9 2023-08-07 13:20:10.000000 pydeseq2-0.4.0/pydeseq2.egg-info/top_level.txt
+-rw-r--r--   0 bmuzellec   (501) staff       (20)      408 2023-04-05 09:20:58.000000 pydeseq2-0.4.0/pyproject.toml
+-rw-r--r--   0 bmuzellec   (501) staff       (20)       38 2023-08-07 13:20:10.087134 pydeseq2-0.4.0/setup.cfg
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1362 2023-05-02 08:07:48.000000 pydeseq2-0.4.0/setup.py
+drwxr-xr-x   0 bmuzellec   (501) staff       (20)        0 2023-08-07 13:20:10.085152 pydeseq2-0.4.0/tests/
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     5654 2023-02-16 10:34:42.000000 pydeseq2-0.4.0/tests/test_docstring.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    13760 2023-08-07 13:06:39.000000 pydeseq2-0.4.0/tests/test_edge_cases.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)    18943 2023-08-07 13:06:39.000000 pydeseq2-0.4.0/tests/test_pydeseq2.py
+-rw-r--r--   0 bmuzellec   (501) staff       (20)     1951 2023-08-01 09:13:46.000000 pydeseq2-0.4.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pydeseq2-0.3.6/LICENSE` & `pydeseq2-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.6/PKG-INFO` & `pydeseq2-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.3.6
+Version: 0.4.0
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -21,16 +21,17 @@
 PyDESeq2 is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
 method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
 It aims to facilitate DEA experiments for python users.
 
 As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
 scratch, you may experience some differences in terms of retrieved values or available features.
 
-Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
-and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
+Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor and 
+multi-factor analysis (with categorical or continuous factors) using Wald tests.
+We plan to implement more in the future.
 In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Table of Contents
 - [PyDESeq2](#pydeseq2)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
     - [Requirements](#requirements)
@@ -137,16 +138,17 @@
 
 - [x] Integration to the [scverse](https://scverse.org/) ecosystem:
   * [x] Refactoring to use the [AnnData](https://anndata.readthedocs.io/) data structure
   * [x] Submitting a PR to be listed as an [scverse ecosystem](https://github.com/scverse/ecosystem-packages/) package
 - [x] Variance-stabilizing transformation
 - [ ] Improving multi-factor analysis:
   * [x] Allowing n-level factors
+  * [x] Support for continuous covariates
   * [ ] Implementing interaction terms
-  * [ ] Support for continuous covariates
+
 
 ## Citing this work
 
 ```
 @article{muzellec2022pydeseq2,
   title={PyDESeq2: a python package for bulk RNA-seq differential expression analysis},
   author={Muzellec, Boris and Telenczuk, Maria and Cabeli, Vincent and Andreux, Mathieu},
```

### Comparing `pydeseq2-0.3.6/README.md` & `pydeseq2-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 PyDESeq2 is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
 method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
 It aims to facilitate DEA experiments for python users.
 
 As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
 scratch, you may experience some differences in terms of retrieved values or available features.
 
-Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
-and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
+Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor and 
+multi-factor analysis (with categorical or continuous factors) using Wald tests.
+We plan to implement more in the future.
 In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Table of Contents
 - [PyDESeq2](#pydeseq2)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
     - [Requirements](#requirements)
@@ -125,16 +126,17 @@
 
 - [x] Integration to the [scverse](https://scverse.org/) ecosystem:
   * [x] Refactoring to use the [AnnData](https://anndata.readthedocs.io/) data structure
   * [x] Submitting a PR to be listed as an [scverse ecosystem](https://github.com/scverse/ecosystem-packages/) package
 - [x] Variance-stabilizing transformation
 - [ ] Improving multi-factor analysis:
   * [x] Allowing n-level factors
+  * [x] Support for continuous covariates
   * [ ] Implementing interaction terms
-  * [ ] Support for continuous covariates
+
 
 ## Citing this work
 
 ```
 @article{muzellec2022pydeseq2,
   title={PyDESeq2: a python package for bulk RNA-seq differential expression analysis},
   author={Muzellec, Boris and Telenczuk, Maria and Cabeli, Vincent and Andreux, Mathieu},
```

### Comparing `pydeseq2-0.3.6/pydeseq2/dds.py` & `pydeseq2-0.4.0/pydeseq2/dds.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from pydeseq2.utils import fit_moments_dispersions
 from pydeseq2.utils import fit_rough_dispersions
 from pydeseq2.utils import get_num_processes
 from pydeseq2.utils import irls_solver
 from pydeseq2.utils import make_scatter
 from pydeseq2.utils import mean_absolute_deviation
 from pydeseq2.utils import nb_nll
+from pydeseq2.utils import replace_underscores
 from pydeseq2.utils import robust_method_of_moments_disp
 from pydeseq2.utils import test_valid_counts
 from pydeseq2.utils import trimmed_mean
 
 # Ignore DomainWarning raised by statsmodels when fitting a Gamma GLM with identity link.
 warnings.simplefilter("ignore", DomainWarning)
 # Ignore AnnData's FutureWarning about implicit data conversion.
@@ -64,15 +65,19 @@
 
     metadata : pandas.DataFrame
         DataFrame containing sample metadata.
         Must be indexed by sample barcodes.
 
     design_factors : str or list
         Name of the columns of metadata to be used as design variables.
-        Only categorial factors are supported. (default: ``'condition'``).
+        (default: ``'condition'``).
+
+    continuous_factors : list or None
+        An optional list of continuous (as opposed to categorical) factors. Any factor
+        not in ``continuous_factors`` will be considered categorical (default: ``None``).
 
     ref_level : list or None
         An optional list of two strings of the form ``["factor", "test_level"]``
         specifying the factor of interest and the reference (control) level against which
         we're testing, e.g. ``["condition", "A"]``. (default: ``None``).
 
     min_mu : float
@@ -166,14 +171,15 @@
     def __init__(
         self,
         *,
         adata: Optional[ad.AnnData] = None,
         counts: Optional[pd.DataFrame] = None,
         metadata: Optional[pd.DataFrame] = None,
         design_factors: Union[str, List[str]] = "condition",
+        continuous_factors: Optional[List[str]] = None,
         ref_level: Optional[List[str]] = None,
         min_mu: float = 0.5,
         min_disp: float = 1e-8,
         max_disp: float = 10.0,
         refit_cooks: bool = True,
         min_replicates: int = 7,
         beta_tol: float = 1e-8,
@@ -205,23 +211,57 @@
                 "Either adata or both counts and metadata arguments must be provided."
             )
 
         # Convert design_factors to list if a single string was provided.
         self.design_factors = (
             [design_factors] if isinstance(design_factors, str) else design_factors
         )
+        self.continuous_factors = continuous_factors
+
         if self.obs[self.design_factors].isna().any().any():
             raise ValueError("NaNs are not allowed in the design factors.")
         self.obs[self.design_factors] = self.obs[self.design_factors].astype(str)
 
+        # Check that design factors don't contain underscores. If so, convert them to
+        # hyphens.
+        if np.any(["_" in factor for factor in self.design_factors]):
+            warnings.warn(
+                """Same factor names in the design contain underscores ('_'). They will
+                be converted to hyphens ('-').""",
+                UserWarning,
+                stacklevel=2,
+            )
+
+            new_factors = replace_underscores(self.design_factors)
+
+            self.obs.rename(
+                columns={
+                    old_factor: new_factor
+                    for (old_factor, new_factor) in zip(self.design_factors, new_factors)
+                },
+                inplace=True,
+            )
+
+            self.design_factors = new_factors
+
+            # Also check continuous factors
+            if self.continuous_factors is not None:
+                self.continuous_factors = replace_underscores(self.continuous_factors)
+
+        # If ref_level has underscores, covert them to hyphens
+        # Don't raise a warning: it will be raised by build_design_matrix()
+        if ref_level is not None:
+            ref_level = replace_underscores(ref_level)
+
         # Build the design matrix
         # Stored in the obsm attribute of the dataset
         self.obsm["design_matrix"] = build_design_matrix(
             metadata=self.obs,
             design_factors=self.design_factors,
+            continuous_factors=self.continuous_factors,
             ref_level=ref_level,
             expanded=False,
             intercept=True,
         )
 
         # Check that the design matrix has full rank
         self._check_full_rank_design()
```

### Comparing `pydeseq2-0.3.6/pydeseq2/ds.py` & `pydeseq2-0.4.0/pydeseq2/ds.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,18 @@
         DeseqDataSet for which dispersion and LFCs were already estimated.
 
     contrast : list or None
         A list of three strings, in the following format:
         ``['variable_of_interest', 'tested_level', 'ref_level']``.
         Names must correspond to the metadata data passed to the DeseqDataSet.
         E.g., ``['condition', 'B', 'A']`` will measure the LFC of 'condition B' compared
-        to 'condition A'. If None, the last variable from the design matrix is chosen
+        to 'condition A'.
+        For continuous variables, the last two strings should be left empty, e.g.
+        ``['measurement', '', ''].
+        If None, the last variable from the design matrix is chosen
         as the variable of interest, and the reference level is picked alphabetically.
         (default: ``None``).
 
     alpha : float
         P-value and adjusted p-value significance threshold (usually 0.05).
         (default: ``0.05``).
 
@@ -202,19 +205,22 @@
         self.results_df["baseMean"] = self.base_mean
         self.results_df["log2FoldChange"] = self.LFC @ self.contrast_vector / np.log(2)
         self.results_df["lfcSE"] = self.SE / np.log(2)
         self.results_df["stat"] = self.statistics
         self.results_df["pvalue"] = self.p_values
         self.results_df["padj"] = self.padj
 
-        if not self.quiet:
+        if self.contrast[1] == self.contrast[2] == "":
+            # The factor is continuous
+            print(f"Log2 fold change & Wald test p-value: " f"{self.contrast[0]}")
+        else:
+            # The factor is categorical
             print(
                 f"Log2 fold change & Wald test p-value: "
-                f"{self.contrast[0]} {self.contrast[1]} vs {self.contrast[2]}",
-                file=sys.stderr,
+                f"{self.contrast[0]} {self.contrast[1]} vs {self.contrast[2]}"
             )
         display(self.results_df)
 
     def run_wald_test(self) -> None:
         """Perform a Wald test.
 
         Get gene-wise p-values for gene over/under-expression.`
@@ -294,15 +300,22 @@
             The LFC coefficient to shrink. If set to ``None``, the method will try to
             shrink the coefficient corresponding to the ``contrast`` attribute.
             If the desired coefficient is not available, it may be set from the
             :class:`pydeseq2.dds.DeseqDataSet` argument ``ref_level``.
             (default: ``None``).
         """
 
-        contrast_level = f"{self.contrast[0]}_{self.contrast[1]}_vs_{self.contrast[2]}"
+        if self.contrast[1] == self.contrast[2] == "":
+            # The factor being tested is continuous
+            contrast_level = self.contrast[0]
+        else:
+            # The factor being tested is categorical
+            contrast_level = (
+                f"{self.contrast[0]}_{self.contrast[1]}_vs_{self.contrast[2]}"
+            )
 
         if coeff is not None:
             if coeff not in self.LFC.columns:
                 split_coeff = coeff.split("_")
                 if len(split_coeff) == 4:
                     raise KeyError(
                         f"The coeff argument '{coeff}' should be one the LFC columns. "
@@ -396,25 +409,29 @@
         # Set a flag to indicate that LFCs were shrunk
         self.shrunk_LFCs = True
 
         # Replace in results dataframe, if it exists
         if hasattr(self, "results_df"):
             self.results_df["log2FoldChange"] = self.LFC.iloc[:, coeff_idx] / np.log(2)
             self.results_df["lfcSE"] = self.SE / np.log(2)
-
-            # Get the corrresponding factor, tested and reference levels of the shrunk
+            # Get the corresponding factor, tested and reference levels of the shrunk
             # coefficient
             split_coeff = coeff.split("_")
-            # coeffs are of the form "factor_A_vs_B", hence "factor" is split_coeff[0],
-            # "A" is split_coeff[1] and "B" split_coeff[3]
-            if not self.quiet:
+            # Categorical coeffs are of the form "factor_A_vs_B", and continuous coeffs
+            # of the form "factor".
+            if len(split_coeff) == 1:
+                # The factor is continuous
+                print(f"Shrunk log2 fold change & Wald test p-value: " f"{coeff}")
+            else:
+                # The factor is categorical
+                # Categorical coeffs are of the form "factor_A_vs_B", hence "factor"
+                # is split_coeff[0], "A" is split_coeff[1] and "B" split_coeff[3]
                 print(
-                    f"Shrunk Log2 fold change & Wald test p-value: "
-                    f"{split_coeff[0]} {split_coeff[1]} vs {split_coeff[3]}",
-                    file=sys.stderr,
+                    f"Shrunk log2 fold change & Wald test p-value: "
+                    f"{split_coeff[0]} {split_coeff[1]} vs {split_coeff[3]}"
                 )
 
             display(self.results_df)
 
     def plot_MA(self, log: bool = True, save_path: Optional[str] = None, **kwargs):
         """
         Create an log ratio (M)-average (A) plot using matplotlib.
@@ -609,15 +626,18 @@
         Check the validity of the contrast (if provided). If not, build a default
         contrast, corresponding to the last column of the design matrix.
 
         A contrast should be a list of three strings, in the following format:
         ``['variable_of_interest', 'tested_level', 'reference_level']``.
         Names must correspond to the metadata data passed to the DeseqDataSet.
         E.g., ``['condition', 'B', 'A']`` will measure the LFC of 'condition B'
-        compared to 'condition A'. If None, the last variable from the design matrix
+        compared to 'condition A'.
+        For continuous variables, the last two strings will be left empty, e.g.
+        ``['measurement', '', ''].
+        If None, the last variable from the design matrix
         is chosen as the variable of interest, and the reference level is picked
         alphabetically.
 
         Parameters
         ----------
         contrast : list or None
             A list of three strings, in the following format:
@@ -629,45 +649,61 @@
             if len(contrast) != 3:
                 raise ValueError("The contrast should contain three strings.")
             if contrast[0] not in self.dds.design_factors:
                 raise KeyError(
                     f"The contrast variable ('{contrast[0]}') should be one "
                     f"of the design factors."
                 )
-            if contrast[1] not in self.dds.obs[contrast[0]].values:
-                raise KeyError(
-                    f"The tested level ('{contrast[1]}') should correspond to one of the"
-                    f" levels of '{contrast[0]}'"
-                )
-            if contrast[2] not in self.dds.obs[contrast[0]].values:
-                raise KeyError(
-                    f"The reference level ('{contrast[2]}') should correspond to one of"
-                    f" the levels of '{contrast[0]}'"
-                )
+            if not (contrast[1] == contrast[2] == ""):
+                # The contrast factor is categorical, so we should check that the tested
+                # and reference levels are valid.
+                if contrast[1] not in self.dds.obs[contrast[0]].values:
+                    raise KeyError(
+                        f"The tested level ('{contrast[1]}') should correspond to "
+                        f"one of the levels of '{contrast[0]}'"
+                    )
+                if contrast[2] not in self.dds.obs[contrast[0]].values:
+                    raise KeyError(
+                        f"The reference level ('{contrast[2]}') should correspond to "
+                        f"one of the levels of '{contrast[0]}'"
+                    )
             self.contrast = contrast
         else:  # Build contrast if None
             factor = self.dds.design_factors[-1]
-            factor_col = next(
-                col
-                for col in self.dds.obsm["design_matrix"].columns
-                if col.startswith(factor)
-            )
-            split_col = factor_col.split("_")
-            self.contrast = [split_col[0], split_col[1], split_col[-1]]
+            # Check whether this factor is categorical or continuous.
+            if (
+                self.dds.continuous_factors is not None
+                and factor in self.dds.continuous_factors
+            ):
+                # The factor is continuous
+                self.contrast = [factor, "", ""]
+            else:
+                # The factor is categorical
+                factor_col = next(
+                    col
+                    for col in self.dds.obsm["design_matrix"].columns
+                    if col.startswith(factor)
+                )
+                split_col = factor_col.split("_")
+                self.contrast = [split_col[0], split_col[1], split_col[-1]]
 
     def _build_contrast_vector(self) -> None:
         """
         Build a vector corresponding to the desired contrast.
 
         Allows to test any pair of levels without refitting LFCs.
         """
         factor = self.contrast[0]
         alternative = self.contrast[1]
         ref = self.contrast[2]
-        contrast_level = f"{factor}_{alternative}_vs_{ref}"
+        if ref == alternative == "":
+            # "factor" is a continuous variable
+            contrast_level = factor
+        else:
+            contrast_level = f"{factor}_{alternative}_vs_{ref}"
 
         self.contrast_vector = np.zeros(self.LFC.shape[-1])
         if contrast_level in self.design_matrix.columns:
             self.contrast_idx = self.LFC.columns.get_loc(contrast_level)
             self.contrast_vector[self.contrast_idx] = 1
         elif f"{factor}_{ref}_vs_{alternative}" in self.design_matrix.columns:
             # Reference and alternative are inverted
@@ -676,14 +712,14 @@
             )
             self.contrast_vector[self.contrast_idx] = -1
         else:
             # Need to change reference
             # Get any column corresponding to the desired factor and extract old ref
             old_ref = next(
                 col for col in self.LFC.columns if col.startswith(factor)
-            ).split("_")[-1]
+            ).split("_vs_")[-1]
             new_alternative_idx = self.LFC.columns.get_loc(
                 f"{factor}_{alternative}_vs_{old_ref}"
             )
             new_ref_idx = self.LFC.columns.get_loc(f"{factor}_{ref}_vs_{old_ref}")
             self.contrast_vector[new_alternative_idx] = 1
             self.contrast_vector[new_ref_idx] = -1
```

### Comparing `pydeseq2-0.3.6/pydeseq2/grid_search.py` & `pydeseq2-0.4.0/pydeseq2/grid_search.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.6/pydeseq2/preprocessing.py` & `pydeseq2-0.4.0/pydeseq2/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.6/pydeseq2/utils.py` & `pydeseq2-0.4.0/pydeseq2/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import multiprocessing
+import warnings
 from math import floor
 from pathlib import Path
 from typing import List
 from typing import Literal
 from typing import Optional
 from typing import Tuple
 from typing import Union
@@ -137,40 +138,44 @@
         raise ValueError("The count matrix should only contain non-negative values.")
 
 
 def build_design_matrix(
     metadata: pd.DataFrame,
     design_factors: Union[str, List[str]] = "condition",
     ref_level: Optional[List[str]] = None,
+    continuous_factors: Optional[List[str]] = None,
     expanded: bool = False,
     intercept: bool = True,
 ) -> pd.DataFrame:
     """Build design_matrix matrix for DEA.
 
-    Only single factor, 2-level designs are currently supported.
     Unless specified, the reference factor is chosen alphabetically.
-    NOTE: For now, each factor should have exactly two levels.
 
     Parameters
     ----------
     metadata : pandas.DataFrame
         DataFrame containing metadata information.
         Must be indexed by sample barcodes.
 
     design_factors : str or list
         Name of the columns of metadata to be used as design_matrix variables.
         (default: ``"condition"``).
 
-    ref_level : list or None
+    ref_level : dict or None
         An optional list of two strings of the form ``["factor", "ref_level"]``
         specifying the factor of interest and the desired reference level, e.g.
         ``["condition", "A"]``. (default: ``None``).
 
+    continuous_factors : list or None
+        An optional list of continuous (as opposed to categorical) factors. Any factor
+        not in ``continuous_factors`` will be considered categorical (default: ``None``).
+
     expanded : bool
-        If true, use one column per category. Else, use a single column.
+        If true, use one column per category. Else, use n-1 columns, for each n-level
+        categorical factor.
         (default: ``False``).
 
     intercept : bool
         If true, add an intercept (a column containing only ones). (default: ``True``).
 
     Returns
     -------
@@ -188,63 +193,121 @@
         # Check that each factor has at least 2 levels
         if len(np.unique(metadata[factor])) < 2:
             raise ValueError(
                 f"Factors should take at least two values, but {factor} "
                 f"takes the single value '{np.unique(metadata[factor])}'."
             )
 
-    design_matrix = pd.get_dummies(metadata[design_factors], drop_first=not expanded)
+    # Check that level factors in the design don't contain underscores. If so, convert
+    # them to hyphens
+    warning_issued = False
+    for factor in design_factors:
+        if np.any(["_" in value for value in metadata[factor]]):
+            if not warning_issued:
+                warnings.warn(
+                    """Some factor levels in the design contain underscores ('_').
+                    They will be converted to hyphens ('-').""",
+                    UserWarning,
+                    stacklevel=2,
+                )
+                warning_issued = True
+            metadata[factor] = metadata[factor].apply(lambda x: x.replace("_", "-"))
 
-    if ref_level is not None:
-        if len(ref_level) != 2:
-            raise KeyError("The reference level should contain 2 strings.")
-        if ref_level[1] not in metadata[ref_level[0]].values:
-            raise KeyError(
-                f"The metadata data should contain a '{ref_level[0]}' column"
-                f" with a '{ref_level[1]}' level."
-            )
+    if continuous_factors is not None:
+        categorical_factors = [
+            factor for factor in design_factors if factor not in continuous_factors
+        ]
+    else:
+        categorical_factors = design_factors
 
-        # Check that the reference level is not in the matrix (if unexpanded design)
-        ref_level_name = "_".join(ref_level)
-        if (not expanded) and ref_level_name in design_matrix.columns:
-            # Remove the reference level and add one
-            factor_cols = [
-                col for col in design_matrix.columns if col.startswith(ref_level[0])
-            ]
-            missing_level = next(
-                level
-                for level in np.unique(metadata[ref_level[0]])
-                if f"{ref_level[0]}_{level}" not in design_matrix.columns
-            )
-            design_matrix[f"{ref_level[0]}_{missing_level}"] = 1 - design_matrix[
-                factor_cols
-            ].sum(1)
-            design_matrix.drop(ref_level_name, axis="columns", inplace=True)
-
-    if not expanded:
-        # Add reference level as column name suffix
-        for factor in design_factors:
-            if ref_level is None or factor != ref_level[0]:
-                # The reference is the unique level that is no longer there
-                ref = next(
+    # Check that there is at least one categorical factor
+    if len(categorical_factors) > 0:
+        design_matrix = pd.get_dummies(
+            metadata[categorical_factors], drop_first=not expanded
+        )
+
+        if ref_level is not None:
+            if len(ref_level) != 2:
+                raise KeyError("The reference level should contain 2 strings.")
+            if ref_level[1] not in metadata[ref_level[0]].values:
+                raise KeyError(
+                    f"The metadata data should contain a '{ref_level[0]}' column"
+                    f" with a '{ref_level[1]}' level."
+                )
+
+            # Check that the reference level is not in the matrix (if unexpanded design)
+            ref_level_name = "_".join(ref_level)
+            if (not expanded) and ref_level_name in design_matrix.columns:
+                # Remove the reference level and add one
+                factor_cols = [
+                    col for col in design_matrix.columns if col.startswith(ref_level[0])
+                ]
+                missing_level = next(
                     level
-                    for level in np.unique(metadata[factor])
-                    if f"{factor}_{level}" not in design_matrix.columns
+                    for level in np.unique(metadata[ref_level[0]])
+                    if f"{ref_level[0]}_{level}" not in design_matrix.columns
                 )
-            else:
-                # The reference level is given as an argument
-                ref = ref_level[1]
-            design_matrix.columns = [
-                f"{col}_vs_{ref}" if col.startswith(factor) else col
-                for col in design_matrix.columns
-            ]
+                design_matrix[f"{ref_level[0]}_{missing_level}"] = 1 - design_matrix[
+                    factor_cols
+                ].sum(1)
+                design_matrix.drop(ref_level_name, axis="columns", inplace=True)
+
+        if not expanded:
+            # Add reference level as column name suffix
+            for factor in design_factors:
+                if ref_level is None or factor != ref_level[0]:
+                    # The reference is the unique level that is no longer there
+                    ref = next(
+                        level
+                        for level in np.unique(metadata[factor])
+                        if f"{factor}_{level}" not in design_matrix.columns
+                    )
+                else:
+                    # The reference level is given as an argument
+                    ref = ref_level[1]
+                design_matrix.columns = [
+                    f"{col}_vs_{ref}" if col.startswith(factor) else col
+                    for col in design_matrix.columns
+                ]
+    else:
+        # There is no categorical factor in the design
+        design_matrix = pd.DataFrame(index=metadata.index)
 
     if intercept:
         design_matrix.insert(0, "intercept", 1)
-    return design_matrix.astype("int")
+
+    # Convert categorical factors one-hot encodings to int
+    design_matrix = design_matrix.astype("int")
+
+    # Add continuous factors
+    if continuous_factors is not None:
+        for factor in continuous_factors:
+            # This factor should be numeric
+            design_matrix[factor] = pd.to_numeric(metadata[factor])
+    return design_matrix
+
+
+def replace_underscores(factors: List[str]):
+    """Replace all underscores from strings in a list by hyphens.
+
+    To be used on design factors to avoid bugs due to the reliance on `str.split("_")` in
+    parts of the code.
+
+    Parameters
+    ----------
+    factors : list
+        A list of strings which may contain underscores.
+
+    Returns
+    -------
+    list
+        A list of strings in which underscores were replaced by hyphens.
+    """
+
+    return [factor.replace("_", "-") for factor in factors]
 
 
 def dispersion_trend(
     normed_mean: Union[float, np.ndarray],
     coeffs: Union["pd.Series[float]", np.ndarray],
 ) -> Union[float, np.ndarray]:
     r"""Return dispersion trend from normalized counts.
```

### Comparing `pydeseq2-0.3.6/pydeseq2.egg-info/PKG-INFO` & `pydeseq2-0.4.0/pydeseq2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydeseq2
-Version: 0.3.6
+Version: 0.4.0
 Summary: A python implementation of DESeq2.
 Author: Boris Muzellec, Maria Telenczuk, Vincent Cabelli and Mathieu Andreux
 Author-email: boris.muzellec@owkin.com
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -21,16 +21,17 @@
 PyDESeq2 is a python implementation of the [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) 
 method [1] for differential expression analysis (DEA) with bulk RNA-seq data, originally in R.
 It aims to facilitate DEA experiments for python users.
 
 As PyDESeq2 is a re-implementation of [DESeq2](https://bioconductor.org/packages/release/bioc/html/DESeq2.html) from 
 scratch, you may experience some differences in terms of retrieved values or available features.
 
-Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor 
-and n-level multi-factor analysis (with categorical factors), but we plan to implement more in the future.
+Currently, available features broadly correspond to the default settings of DESeq2 (v1.34.0) for single-factor and 
+multi-factor analysis (with categorical or continuous factors) using Wald tests.
+We plan to implement more in the future.
 In case there is a feature you would particularly like to be implemented, feel free to open an issue.
 
 ## Table of Contents
 - [PyDESeq2](#pydeseq2)
   - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
     - [Requirements](#requirements)
@@ -137,16 +138,17 @@
 
 - [x] Integration to the [scverse](https://scverse.org/) ecosystem:
   * [x] Refactoring to use the [AnnData](https://anndata.readthedocs.io/) data structure
   * [x] Submitting a PR to be listed as an [scverse ecosystem](https://github.com/scverse/ecosystem-packages/) package
 - [x] Variance-stabilizing transformation
 - [ ] Improving multi-factor analysis:
   * [x] Allowing n-level factors
+  * [x] Support for continuous covariates
   * [ ] Implementing interaction terms
-  * [ ] Support for continuous covariates
+
 
 ## Citing this work
 
 ```
 @article{muzellec2022pydeseq2,
   title={PyDESeq2: a python package for bulk RNA-seq differential expression analysis},
   author={Muzellec, Boris and Telenczuk, Maria and Cabeli, Vincent and Andreux, Mathieu},
```

### Comparing `pydeseq2-0.3.6/setup.py` & `pydeseq2-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.6/tests/test_docstring.py` & `pydeseq2-0.4.0/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `pydeseq2-0.3.6/tests/test_edge_cases.py` & `pydeseq2-0.4.0/tests/test_edge_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,52 @@
     )
     metadata = pd.DataFrame({"condition": [0, np.NaN]}, index=["sample1", "sample2"])
 
     with pytest.raises(ValueError):
         DeseqDataSet(counts=counts_df, metadata=metadata, design_factors="condition")
 
 
+def test_underscores_in_factors():
+    """Test that underscores in factor and variable names don't cause bugs."""
+    counts_df = load_example_data(
+        modality="raw_counts",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    metadata = load_example_data(
+        modality="metadata",
+        dataset="synthetic",
+        debug=False,
+    )
+
+    # Rename metadata's columns and variables to add underscores
+    metadata.rename(
+        columns={"condition": "some_variable_with_underscores"}, inplace=True
+    )
+    metadata.replace(
+        {"A": "level_with_underscores", "B": "level_with_even_more_underscores"},
+        inplace=True,
+    )
+
+    # Run the pipeline. This should raise a warning, but not cause bugs.
+    with pytest.warns(UserWarning):
+        dds = DeseqDataSet(
+            counts=counts_df,
+            metadata=metadata,
+            design_factors="some_variable_with_underscores",
+            ref_level=["some_variable_with_underscores", "level_with_underscores"],
+        )
+    dds.deseq2()
+
+    stat_res = DeseqStats(dds)
+    stat_res.summary()
+    stat_res.lfc_shrink()
+
+
 def test_one_factor():
     """Test that a ValueError is thrown when the design factor takes only one value."""
     counts_df = pd.DataFrame(
         {"gene1": [0, 1], "gene2": [4, 12]}, index=["sample1", "sample2"]
     )
     metadata = pd.DataFrame({"condition": [0, 0]}, index=["sample1", "sample2"])
```

### Comparing `pydeseq2-0.3.6/tests/test_pydeseq2.py` & `pydeseq2-0.4.0/tests/test_pydeseq2.py`

 * *Files 12% similar despite different names*

```diff
@@ -289,14 +289,115 @@
     # Check that the same LFC found (up to tol)
     assert (
         abs(r_shrunk_res.log2FoldChange - shrunk_res.log2FoldChange)
         / abs(r_shrunk_res.log2FoldChange)
     ).max() < tol
 
 
+# Continuous tests
+def test_continuous_deseq(tol=0.02):
+    """Test that the outputs of the DESeq2 function match those of the original R
+    package, up to a tolerance in relative error, with a continuous factor.
+    """
+
+    test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
+
+    counts_df = pd.read_csv(
+        os.path.join(test_path, "data/continuous/test_counts.csv"), index_col=0
+    ).T
+
+    metadata = pd.read_csv(
+        os.path.join(test_path, "data/continuous/test_metadata.csv"), index_col=0
+    )
+
+    r_res = pd.read_csv(
+        os.path.join(test_path, "data/continuous/r_test_res.csv"), index_col=0
+    )
+
+    dds = DeseqDataSet(
+        counts=counts_df,
+        metadata=metadata,
+        design_factors=["group", "condition", "measurement"],
+        continuous_factors=["measurement"],
+    )
+    dds.deseq2()
+
+    res = DeseqStats(dds)
+    res.summary()
+    res_df = res.results_df
+
+    # check that the same p-values are NaN
+    assert (res_df.pvalue.isna() == r_res.pvalue.isna()).all()
+    assert (res_df.padj.isna() == r_res.padj.isna()).all()
+
+    # Check that the same LFC, p-values and adjusted p-values are found (up to tol)
+    assert (
+        abs(r_res.log2FoldChange - res_df.log2FoldChange) / abs(r_res.log2FoldChange)
+    ).max() < tol
+    assert (abs(r_res.pvalue - res_df.pvalue) / r_res.pvalue).max() < tol
+    assert (abs(r_res.padj - res_df.padj) / r_res.padj).max() < tol
+
+
+def test_continuous_lfc_shrinkage(tol=0.02):
+    """Test that the outputs of the lfc_shrink function match those of the original
+    R package (starting from the same inputs), up to a tolerance in relative error.
+    """
+
+    test_path = str(Path(os.path.realpath(tests.__file__)).parent.resolve())
+
+    r_res = pd.read_csv(
+        os.path.join(test_path, "data/continuous/r_test_res.csv"), index_col=0
+    )
+    r_shrunk_res = pd.read_csv(
+        os.path.join(test_path, "data/continuous/r_test_lfc_shrink_res.csv"),
+        index_col=0,
+    )
+
+    counts_df = pd.read_csv(
+        os.path.join(test_path, "data/continuous/test_counts.csv"), index_col=0
+    ).T
+
+    metadata = pd.read_csv(
+        os.path.join(test_path, "data/continuous/test_metadata.csv"), index_col=0
+    )
+
+    r_size_factors = pd.read_csv(
+        os.path.join(test_path, "data/continuous/r_test_size_factors.csv"),
+        index_col=0,
+    ).squeeze()
+
+    r_dispersions = pd.read_csv(
+        os.path.join(test_path, "data/continuous/r_test_dispersions.csv"), index_col=0
+    ).squeeze()
+
+    dds = DeseqDataSet(
+        counts=counts_df,
+        metadata=metadata,
+        design_factors=["group", "condition", "measurement"],
+        continuous_factors=["measurement"],
+    )
+
+    dds.deseq2()
+    dds.obsm["size_factors"] = r_size_factors.values
+    dds.varm["dispersions"] = r_dispersions.values
+    dds.varm["LFC"].iloc[:, 1] = r_res.log2FoldChange.values * np.log(2)
+
+    res = DeseqStats(dds)
+    res.summary()
+    res.SE = r_res.lfcSE * np.log(2)
+    res.lfc_shrink(coeff="measurement")
+    shrunk_res = res.results_df
+
+    # Check that the same LFC found (up to tol)
+    assert (
+        abs(r_shrunk_res.log2FoldChange - shrunk_res.log2FoldChange)
+        / abs(r_shrunk_res.log2FoldChange)
+    ).max() < tol
+
+
 def test_contrast():
     """
     Check that the contrasts ['condition', 'B', 'A'] and ['condition', 'A', 'B'] give
     coherent results (change of sign in LFCs and Wald stats, same (adjusted p-values).
     """
 
     counts_df = load_example_data(
```

### Comparing `pydeseq2-0.3.6/tests/test_utils.py` & `pydeseq2-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

