# Comparing `tmp/pertpy-0.4.0.tar.gz` & `tmp/pertpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pertpy-0.4.0.tar", max compression
+gzip compressed data, was "pertpy-0.5.0.tar", max compression
```

## Comparing `pertpy-0.4.0.tar` & `pertpy-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0     1070 2023-04-16 11:27:06.116299 pertpy-0.4.0/LICENSE
--rw-r--r--   0        0        0     1860 2023-04-16 11:27:06.116299 pertpy-0.4.0/README.md
--rw-r--r--   0        0        0      363 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/__init__.py
--rw-r--r--   0        0        0     1206 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/data/__init__.py
--rw-r--r--   0        0        0     2279 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/data/_dataloader.py
--rw-r--r--   0        0        0    62405 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/data/_datasets.py
--rw-r--r--   0        0        0      434 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/__init__.py
--rw-r--r--   0        0        0     6539 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_augurpy.py
--rw-r--r--   0        0        0    38991 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_coda.py
--rw-r--r--   0        0        0     2779 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_guide_rna.py
--rw-r--r--   0        0        0     9257 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_milopy.py
--rw-r--r--   0        0        0    25129 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_mixscape.py
--rw-r--r--   0        0        0    13118 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_scgen.py
--rw-r--r--   0        0        0       54 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/preprocessing/__init__.py
--rw-r--r--   0        0        0     3493 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/preprocessing/_guide_rna.py
--rw-r--r--   0        0        0        0 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/py.typed
--rw-r--r--   0        0        0      818 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/__init__.py
--rw-r--r--   0        0        0    40607 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_augur.py
--rw-r--r--   0        0        0        0 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/__init__.py
--rw-r--r--   0        0        0    61298 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/_base_coda.py
--rw-r--r--   0        0        0    21639 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/_sccoda.py
--rw-r--r--   0        0        0    29152 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/_tasccoda.py
--rw-r--r--   0        0        0    35411 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_dialogue.py
--rw-r--r--   0        0        0     3618 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_differential_gene_expression.py
--rw-r--r--   0        0        0        0 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_distances/__init__.py
--rw-r--r--   0        0        0    11814 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_distances/_distance_tests.py
--rw-r--r--   0        0        0    12562 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_distances/_distances.py
--rw-r--r--   0        0        0     1521 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_kernel_pca.py
--rw-r--r--   0        0        0       63 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_metadata/__init__.py
--rw-r--r--   0        0        0    25517 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_metadata/_cell_line.py
--rw-r--r--   0        0        0    27081 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_milo.py
--rw-r--r--   0        0        0    22105 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_mixscape.py
--rw-r--r--   0        0        0       49 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/__init__.py
--rw-r--r--   0        0        0     2880 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_base_components.py
--rw-r--r--   0        0        0    12990 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_jax_scgen.py
--rw-r--r--   0        0        0     3902 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_jax_scgenvae.py
--rw-r--r--   0        0        0     2807 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_utils.py
--rw-r--r--   0        0        0     1069 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/transferlearning_MMD_LICENSE
--rw-r--r--   0        0        0     3037 2023-04-16 11:27:06.144299 pertpy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 pertpy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-07 10:47:37.171862 pertpy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1856 2023-08-07 10:47:37.171862 pertpy-0.5.0/README.md
+-rw-r--r--   0        0        0      490 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/__init__.py
+-rw-r--r--   0        0        0     1206 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/data/__init__.py
+-rw-r--r--   0        0        0     2393 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/data/_dataloader.py
+-rw-r--r--   0        0        0    62414 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/data/_datasets.py
+-rw-r--r--   0        0        0      434 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/__init__.py
+-rw-r--r--   0        0        0     6569 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/_augurpy.py
+-rw-r--r--   0        0        0    38882 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/_coda.py
+-rw-r--r--   0        0        0     2779 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/_guide_rna.py
+-rw-r--r--   0        0        0     9257 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/_milopy.py
+-rw-r--r--   0        0        0    25108 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/_mixscape.py
+-rw-r--r--   0        0        0    13069 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/plot/_scgen.py
+-rw-r--r--   0        0        0       54 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3493 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/preprocessing/_guide_rna.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/py.typed
+-rw-r--r--   0        0        0     1064 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/__init__.py
+-rw-r--r--   0        0        0    40607 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_augur.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_coda/__init__.py
+-rw-r--r--   0        0        0    61737 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_coda/_base_coda.py
+-rw-r--r--   0        0        0    22216 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_coda/_sccoda.py
+-rw-r--r--   0        0        0    29929 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_coda/_tasccoda.py
+-rw-r--r--   0        0        0    35411 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_dialogue.py
+-rw-r--r--   0        0        0     3639 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_differential_gene_expression.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_distances/__init__.py
+-rw-r--r--   0        0        0    11745 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_distances/_distance_tests.py
+-rw-r--r--   0        0        0    12601 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_distances/_distances.py
+-rw-r--r--   0        0        0     1521 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_kernel_pca.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_metadata/__init__.py
+-rw-r--r--   0        0        0    25519 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_metadata/_cell_line.py
+-rw-r--r--   0        0        0    27184 2023-08-07 10:47:37.199862 pertpy-0.5.0/pertpy/tools/_milo.py
+-rw-r--r--   0        0        0    22148 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_mixscape.py
+-rw-r--r--   0        0        0        0 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_perturbation_space/__init__.py
+-rw-r--r--   0        0        0     2811 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_perturbation_space/_clustering.py
+-rw-r--r--   0        0        0    12975 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_perturbation_space/_discriminator_classifier.py
+-rw-r--r--   0        0        0     3169 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_perturbation_space/_metrics.py
+-rw-r--r--   0        0        0    12669 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_perturbation_space/_perturbation_space.py
+-rw-r--r--   0        0        0     9232 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_perturbation_space/_simple.py
+-rw-r--r--   0        0        0       49 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_scgen/__init__.py
+-rw-r--r--   0        0        0     2879 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_scgen/_base_components.py
+-rw-r--r--   0        0        0    13009 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_scgen/_jax_scgen.py
+-rw-r--r--   0        0        0     3937 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_scgen/_jax_scgenvae.py
+-rw-r--r--   0        0        0     2807 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/_scgen/_utils.py
+-rw-r--r--   0        0        0     1069 2023-08-07 10:47:37.203862 pertpy-0.5.0/pertpy/tools/transferlearning_MMD_LICENSE
+-rw-r--r--   0        0        0     2735 2023-08-07 10:47:37.207862 pertpy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 pertpy-0.5.0/PKG-INFO
```

### Comparing `pertpy-0.4.0/LICENSE` & `pertpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/README.md` & `pertpy-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,28 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/pertpy)](https://pypi.org/project/pertpy)
 [![Read the Docs](https://img.shields.io/readthedocs/pertpy/latest.svg?label=Read%20the%20Docs)](https://pertpy.readthedocs.io/)
 [![Test](https://github.com/theislab/pertpy/workflows/Run%20pertpy%20Tests/badge.svg)](https://github.com/theislab/pertpy/actions?workflow=Tests)
 [![PyPI](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # pertpy
 
-## Features
+![pertpy-wide1](https://user-images.githubusercontent.com/21954664/235677503-0c72f90d-3f6d-4a16-a1ff-ff8c11a540fb.png)
 
--   Differential cell type perturbation analysis with Augurpy
--   Analysis of CRISPR-KO screens with Mixscape
--   Compositional analysis with Milo and tascCODA
+## Documentation
+
+Please read the [documentation](https://pertpy.readthedocs.io/en/latest).
 
 ## Installation
 
 You can install _pertpy_ via [pip] from [PyPI]:
 
 ```console
 $ pip install pertpy
 ```
 
-## Usage
-
-Please see [Usage] for details.
-
 ## Credits
 
 This package was created with [cookietemple] using [Cookiecutter] based on [Hypermodern_Python_Cookiecutter].
 
 [cookiecutter]: https://github.com/audreyr/cookiecutter
 [cookietemple]: https://cookietemple.com
 [hypermodern_python_cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
```

### Comparing `pertpy-0.4.0/pertpy/data/__init__.py` & `pertpy-0.5.0/pertpy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/data/_dataloader.py` & `pertpy-0.5.0/pertpy/data/_dataloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,13 +53,16 @@
         task = progress.add_task("[red]Downloading...", total=total)
         Path(output_path).mkdir(parents=True, exist_ok=True)
         with open(download_to_path, "wb") as file:
             for data in response.iter_content(block_size):
                 file.write(data)
                 progress.update(task, advance=block_size)
 
+        # force the progress bar to 100% at the end
+        progress.update(task, completed=total, refresh=True)
+
     if is_zip:
         output_path = output_path or tempfile.gettempdir()
         with ZipFile(download_to_path, "r") as zip_obj:
             zip_obj.extractall(path=output_path)
             extracted = zip_obj.namelist()
             print(extracted)
```

### Comparing `pertpy-0.4.0/pertpy/data/_datasets.py` & `pertpy-0.5.0/pertpy/data/_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
 
-import muon as mu
 import scanpy as sc
 from anndata import AnnData
 from mudata import MuData
 from scanpy import settings
 
 from pertpy.data._dataloader import _download
 
@@ -34,14 +33,16 @@
         Papalexi, E., Mimitou, E.P., Butler, A.W. et al. Characterizing the molecular regulation
         of inhibitory immune checkpoints with multimodal single-cell screens.
         Nat Genet 53, 322–331 (2021). https://doi.org/10.1038/s41588-021-00778-2
 
     Returns:
         :class:`~anndata.AnnData` object of the ECCITE-seq dataset
     """
+    import muon as mu
+
     output_file_name = "papalexi_2021.h5mu"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/36509460",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
@@ -207,15 +208,15 @@
         Frangieh, C.J., Melms, J.C., Thakore, P.I. et al. Multimodal pooled Perturb-CITE-seq
         screens in patient models define mechanisms of cancer immune evasion.
         Nat Genet 53, 332–341 (2021). https://doi.org/10.1038/s41588-021-00779-1
 
     Returns:
         :class:`~anndata.AnnData` object of raw Perturb-CITE-seq data
     """
-    output_file_name = "frangieh_2021.h5ad"
+    output_file_name = "frangieh_2021_raw.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34012565",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
```

### Comparing `pertpy-0.4.0/pertpy/plot/_augurpy.py` & `pertpy-0.5.0/pertpy/plot/_augurpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         Args:
             results: Results after running differential prioritization.
             top_n: optionally, the number of top prioritized cell types to label in the plot
             ax: optionally, axes used to draw plot
             return_figure: if `True` returns figure of the plot
 
         Returns:
+            Axes of the plot.
         """
         x = results["mean_augur_score1"]
         y = results["mean_augur_score2"]
 
         if ax is None:
             fig, ax = plt.subplots()
         scatter = ax.scatter(x, y, c=results.z, cmap="Greens")
```

### Comparing `pertpy-0.4.0/pertpy/plot/_coda.py` & `pertpy-0.5.0/pertpy/plot/_coda.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,18 @@
         title: str,
         level_names: List[str],
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[int] = 100,
         cmap: Optional[ListedColormap] = cm.tab20,
         show_legend: Optional[bool] = True,
     ) -> plt.Axes:
-        """Plots a stacked barplot for one (discrete) covariate
+        """Plots a stacked barplot for one (discrete) covariate.
 
         Typical use (only inside stacked_barplot): plot_one_stackbar(data.X, data.var.index, "xyz", data.obs.index)
 
-
         Args:
             y: The count data, collapsed onto the level of interest. i.e. a binary covariate has two rows, one for each group, containing the count mean of each cell type
             type_names: The names of all cell types
             title: Plot title, usually the covariate's name
             level_names: Names of the covariate's levels
             figsize: Figure size. Defaults to None.
             dpi: Dpi setting. Defaults to 100.
@@ -95,15 +94,14 @@
         show_legend: Optional[bool] = True,
         level_order: List[str] = None,
     ) -> plt.Axes:
         """Plots a stacked barplot for all levels of a covariate or all samples (if feature_name=="samples").
 
         Usage: plot_feature_stackbars(data, ["cov1", "cov2", "cov3"])
 
-
         Args:
             data: AnnData object or MuData object.
             feature_name: The name of the covariate to plot. If feature_name=="samples", one bar for every sample will be plotted
             modality_key: If data is a MuData object, specify which modality to use. Defaults to "coda".
             figsize: Figure size. Defaults to None.
             dpi: Dpi setting. Defaults to 100.
             cmap: The matplotlib color map for the barplot. Defaults to cm.tab20.
@@ -114,16 +112,15 @@
             A :class:`~matplotlib.axes.Axes` object
         """
         if isinstance(data, MuData):
             data = data[modality_key]
         if isinstance(data, AnnData):
             data = data
 
-        # cell type names
-        type_names = data.var.index
+        ct_names = data.var.index
 
         # option to plot one stacked barplot per sample
         if feature_name == "samples":
             if level_order:
                 assert set(level_order) == set(data.obs.index), "level order is inconsistent with levels"
                 data = data[level_order]
             ax = CodaPlot.__stackbar(
@@ -150,15 +147,15 @@
 
             for level in range(n_levels):
                 l_indices = np.where(data.obs[feature_name] == levels[level])
                 feature_totals[level] = np.sum(data.X[l_indices], axis=0)
 
             ax = CodaPlot.__stackbar(
                 feature_totals,
-                type_names=type_names,
+                type_names=ct_names,
                 title=feature_name,
                 level_names=levels,
                 figsize=figsize,
                 dpi=dpi,
                 cmap=cmap,
                 show_legend=show_legend,
             )
@@ -192,15 +189,15 @@
             plot_facets: If False, plot cell types on the x-axis. If True, plot as facets. Defaults to True.
             plot_zero_covariate: If True, plot covariate that have all zero effects. If False, do not plot. Defaults to True.
             plot_zero_cell_type: If True, plot cell type that have zero effect. If False, do not plot. Defaults to False.
             figsize: Figure size. Defaults to None.
             dpi: Figure size. Defaults to 100.
             cmap: The seaborn color map for the barplot. Defaults to cm.tab20.
             level_order: Custom ordering of bars on the x-axis. Defaults to None.
-            args_barplot: Arguments passed to sns.barplot. Defaults to {}.
+            args_barplot: Arguments passed to sns.barplot. Defaults to None.
 
         Returns:
             Depending on `plot_facets`, returns a :class:`~matplotlib.axes.Axes` (`plot_facets = False`) or :class:`~sns.axisgrid.FacetGrid` (`plot_facets = True`) object
         """
         if args_barplot is None:
             args_barplot = {}
         if isinstance(data, MuData):
@@ -243,15 +240,15 @@
                     plot_df = plot_df[plot_df["value"] != 0]
                     for covariate_name_zero in covariate_names_zero:
                         new_row = {
                             "Covariate": covariate_name_zero,
                             "Cell Type": "zero",
                             "value": 0,
                         }
-                        plot_df = plot_df.append(new_row, ignore_index=True)
+                        plot_df = pd.concat([plot_df, pd.DataFrame([new_row])], ignore_index=True)
                     plot_df["covariate_"] = pd.Categorical(plot_df["Covariate"], covariate_names)
                     plot_df = plot_df.sort_values(["covariate_"])
         if not plot_zero_cell_type:
             cell_type_names_zero = [
                 name
                 for name in plot_df["Cell Type"].unique()
                 if (plot_df[plot_df["Cell Type"] == name]["value"] == 0).all()
@@ -742,33 +739,25 @@
             print("Tree leaves and leaf effect bars won't be aligned when legend is shown!")
 
         if isinstance(tree, str):
             tree = data.uns[tree]
         # Collapse tree singularities
         tree2 = collapse_singularities_2(tree)
 
-        node_effs = (
-            data.uns["scCODA_params"]["node_df"]
-            .loc[
-                (covariate + "_node",),
-            ]
-            .copy()
-        )
+        node_effs = data.uns["scCODA_params"]["node_df"].loc[(covariate + "_node",),].copy()
         node_effs.index = node_effs.index.get_level_values("Node")
 
         covariates = data.uns["scCODA_params"]["covariate_names"]
         effect_dfs = [data.varm[f"effect_df_{cov}"] for cov in covariates]
         eff_df = pd.concat(effect_dfs)
         eff_df.index = pd.MultiIndex.from_product(
             (covariates, data.var.index.tolist()),
             names=["Covariate", "Cell Type"],
         )
-        leaf_effs = eff_df.loc[
-            (covariate,),
-        ].copy()
+        leaf_effs = eff_df.loc[(covariate,),].copy()
         leaf_effs.index = leaf_effs.index.get_level_values("Cell Type")
 
         # Add effect values
         for n in tree2.traverse():
             nstyle = NodeStyle()
             nstyle["size"] = 0
             n.set_style(nstyle)
```

### Comparing `pertpy-0.4.0/pertpy/plot/_guide_rna.py` & `pertpy-0.5.0/pertpy/plot/_guide_rna.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/plot/_milopy.py` & `pertpy-0.5.0/pertpy/plot/_milopy.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/plot/_mixscape.py` & `pertpy-0.5.0/pertpy/plot/_mixscape.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     ylab,
 )
 from scanpy import get
 from scanpy._settings import settings
 from scanpy._utils import _check_use_raw, sanitize_anndata
 from scanpy.plotting import _utils
 
-import pertpy as pt
-
 
 class MixscapePlot:
     """Plotting functions for Mixscape."""
 
     @staticmethod
     def barplot(  # pragma: no cover
         adata: AnnData,
```

### Comparing `pertpy-0.4.0/pertpy/plot/_scgen.py` & `pertpy-0.5.0/pertpy/plot/_scgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,14 @@
             dot_sal[ind] = np.dot(delta, vec)
         pyplot.hist(
             dot_cd,
             label=ctrl_key,
             bins=50,
         )
         pyplot.hist(dot_sal, label=stim_key, bins=50)
-        # pyplot.legend(loc=1, prop={'size': 7})
         pyplot.axvline(0, color="k", linestyle="dashed", linewidth=1)
         pyplot.title("  ", fontsize=fontsize)
         pyplot.xlabel("  ", fontsize=fontsize)
         pyplot.ylabel("  ", fontsize=fontsize)
         pyplot.xticks(fontsize=fontsize)
         pyplot.yticks(fontsize=fontsize)
         ax = pyplot.gca()
```

### Comparing `pertpy-0.4.0/pertpy/preprocessing/_guide_rna.py` & `pertpy-0.5.0/pertpy/preprocessing/_guide_rna.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/tools/__init__.py` & `pertpy-0.5.0/pertpy/tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from rich import print
 
 from pertpy.tools._augur import Augur
 from pertpy.tools._dialogue import Dialogue
 from pertpy.tools._differential_gene_expression import DifferentialGeneExpression
 from pertpy.tools._distances._distance_tests import DistanceTest
 from pertpy.tools._distances._distances import Distance
-from pertpy.tools._kernel_pca import kernel_pca
-from pertpy.tools._metadata import CellLineMetaData
+from pertpy.tools._metadata._cell_line import CellLineMetaData
 from pertpy.tools._milo import Milo
 from pertpy.tools._mixscape import Mixscape
+from pertpy.tools._perturbation_space._clustering import ClusteringSpace
+from pertpy.tools._perturbation_space._discriminator_classifier import DiscriminatorClassifierSpace
+from pertpy.tools._perturbation_space._simple import CentroidSpace, DBSCANSpace, KMeansSpace, PseudobulkSpace
 from pertpy.tools._scgen import SCGEN
 
 try:
     from pertpy.tools._coda._sccoda import Sccoda
     from pertpy.tools._coda._tasccoda import Tasccoda
 except ImportError as e:
     if "ete3" in str(e):
```

### Comparing `pertpy-0.4.0/pertpy/tools/_augur.py` & `pertpy-0.5.0/pertpy/tools/_augur.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/tools/_coda/_base_coda.py` & `pertpy-0.5.0/pertpy/tools/_coda/_base_coda.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 import toytree as tt
 from anndata import AnnData
 from jax import random
 from jax._src.prng import PRNGKeyArray
 from jax._src.typing import Array
 from jax.config import config
 from mudata import MuData
-from numpyro.infer import HMC, MCMC, NUTS
+from numpyro.infer import HMC, MCMC, NUTS, initialization
 from rich import box, print
 from rich.console import Console
 from rich.table import Table
 from scipy.cluster import hierarchy as sp_hierarchy
 
 config.update("jax_enable_x64", True)
 
 
 class CompositionalModel2(ABC):
-    """
-    General compositional model framework for scCODA-type models
+    """General compositional model framework for scCODA-type models.
 
     This class serves as a template for scCODA-style models. It handles:
 
     - General data preprocessing
 
     - Inference
 
@@ -57,14 +56,16 @@
     - `sample_adata.uns["scCODA_params"]["select_type"]`:
     String indicating the type of spike_and_slab selection ("spikeslab" or "sslasso")
 
     Additionally, a subclass must implement at least these functions (see subclasses for examples):
 
     - `model`: The model formulation
 
+    - `set_init_mcmc_states`: A function to set the initial state of the MCMC algorithm
+
     - `make_arviz`: A function to generate an arviz result object
     """
 
     @abstractmethod
     def __init__(self):
         pass
 
@@ -72,14 +73,18 @@
     def make_arviz(self, *args, **kwargs):
         pass
 
     @abstractmethod
     def model(self, *args, **kwargs):
         pass
 
+    @abstractmethod
+    def set_init_mcmc_states(self, *args, **kwargs):
+        pass
+
     def prepare(
         self,
         sample_adata: AnnData,
         formula: str,
         reference_cell_type: str = "automatic",
         automatic_reference_absence_threshold: float = 0.05,
     ) -> AnnData:
@@ -92,15 +97,15 @@
                 To set a different level as the base category for a categorical covariate, use "C(<CovariateName>, Treatment('<ReferenceLevelName>'))"
             reference_cell_type: Column name that sets the reference cell type.
                 Reference the name of a column. If "automatic", the cell type with the lowest dispersion in relative abundance that is present in at least 90% of samlpes will be chosen. Defaults to "automatic".
             automatic_reference_absence_threshold: If using reference_cell_type = "automatic", determine the maximum fraction of zero entries for a cell type
                 to be considered as a possible reference cell type. Defaults to 0.05.
 
         Returns:
-            AnnData
+            AnnData object that is ready for CODA models.
         """
         dtype = "float64"
 
         # Convert count data to float64 (needed for correct inference)
         sample_adata.X = sample_adata.X.astype(dtype)
 
         # Build covariate matrix from R-like formula, save in obsm
@@ -209,15 +214,14 @@
         self.mcmc.run(
             rng_key,
             numpyro_counts,
             numpyro_covariates,
             numpyro_n_total,
             jnp.array(sample_adata.uns["scCODA_params"]["reference_index"]),
             sample_adata,
-            init_params=sample_adata.uns["scCODA_params"]["mcmc"]["init_params"],
             extra_fields=extra_fields,
         )
 
         # Set acceptance rate and save sampled values to `sample_adata.uns`
         sample_adata.uns["scCODA_params"]["mcmc"]["acceptance_rate"] = np.array(self.mcmc.last_state.mean_accept_prob)
         samples = self.mcmc.get_samples()
         for k, v in samples.items():
@@ -280,15 +284,19 @@
         if rng_key is None:
             rng_key_array = random.PRNGKey(np.random.randint(0, 10000))
         else:
             rng_key_array = random.PRNGKey(rng_key)
         sample_adata.uns["scCODA_params"]["mcmc"]["rng_key"] = np.array(rng_key_array)
 
         # Set up NUTS kernel
-        nuts_kernel = NUTS(self.model, *args, **kwargs)
+        sample_adata = self.set_init_mcmc_states(
+            rng_key, sample_adata.uns["scCODA_params"]["reference_index"], sample_adata
+        )
+        init_params = sample_adata.uns["scCODA_params"]["mcmc"]["init_params"]
+        nuts_kernel = NUTS(self.model, *args, init_strategy=initialization.init_to_value(values=init_params), **kwargs)
         # Save important parameters in `sample_adata.uns`
         sample_adata.uns["scCODA_params"]["mcmc"]["num_samples"] = num_samples
         sample_adata.uns["scCODA_params"]["mcmc"]["num_warmup"] = num_warmup
         sample_adata.uns["scCODA_params"]["mcmc"]["algorithm"] = "NUTS"
 
         return self.__run_mcmc(
             sample_adata, nuts_kernel, num_samples=num_samples, num_warmup=num_warmup, rng_key=rng_key_array, copy=copy
@@ -330,15 +338,19 @@
         if rng_key is None:
             rng_key = random.PRNGKey(np.random.randint(0, 10000))
             sample_adata.uns["scCODA_params"]["mcmc"]["rng_key"] = rng_key
         else:
             rng_key = random.PRNGKey(rng_key)
 
         # Set up HMC kernel
-        hmc_kernel = HMC(self.model, *args, **kwargs)
+        sample_adata = self.set_init_mcmc_states(
+            rng_key, sample_adata.uns["scCODA_params"]["reference_index"], sample_adata
+        )
+        init_params = sample_adata.uns["scCODA_params"]["mcmc"]["init_params"]
+        hmc_kernel = HMC(self.model, *args, init_strategy=initialization.init_to_value(values=init_params), **kwargs)
 
         # Save important parameters in `sample_adata.uns`
         sample_adata.uns["scCODA_params"]["mcmc"]["num_samples"] = num_samples
         sample_adata.uns["scCODA_params"]["mcmc"]["num_warmup"] = num_warmup
         sample_adata.uns["scCODA_params"]["mcmc"]["algorithm"] = "HMC"
 
         return self.__run_mcmc(
@@ -460,21 +472,17 @@
             ref_index = sample_adata.uns["scCODA_params"]["reference_index"]
             n_conditions = len(covariates)
             n_cell_types = len(cell_types)
 
             def insert_row(idx, df, df_insert):
                 return pd.concat(
                     [
-                        df.iloc[
-                            :idx,
-                        ],
+                        df.iloc[:idx,],
                         df_insert,
-                        df.iloc[
-                            idx:,
-                        ],
+                        df.iloc[idx:,],
                     ]
                 ).reset_index(drop=True)
 
             for i in range(n_conditions):
                 summary_sel = insert_row(
                     (i * n_cell_types) + ref_index,
                     summary_sel,
@@ -552,15 +560,16 @@
         effect_df: pd.DataFrame,
         model_type: str,
         select_type: str,
         target_fdr: float = 0.05,
         node_df: pd.DataFrame = None,
     ) -> pd.DataFrame:
         """Evaluation of MCMC results for effect parameters. This function is only used within self.summary_prepare.
-            This function also calculates the posterior inclusion probability for each effect and decides whether effects are significant.
+
+        This function also calculates the posterior inclusion probability for each effect and decides whether effects are significant.
 
         Args:
             sample_adata: Anndata object with cell counts as sample_adata.X and covariates saved in sample_adata.obs.
             intercept_df: Intercept summary, see ``summary_prepare``
             effect_df: Effect summary, see ``summary_prepare``
             model_type: String indicating the model type ("classic" or "tree_agg")
             select_type:  String indicating the type of spike_and_slab selection ("spikeslab" or "sslasso")
@@ -973,15 +982,15 @@
             sample_adata = data
 
         # Get model and effect selection types
         select_type = sample_adata.uns["scCODA_params"]["select_type"]
         model_type = sample_adata.uns["scCODA_params"]["model_type"]
 
         # If other than None for est_fdr is specified, recalculate intercept and effect DataFrames
-        if type(est_fdr) == float:
+        if isinstance(est_fdr, float):
             if est_fdr < 0 or est_fdr > 1:
                 raise ValueError("est_fdr must be between 0 and 1!")
             else:
                 _, eff_df = self.summary_prepare(sample_adata, est_fdr=est_fdr)  # type: ignore
         # otherwise, get pre-calculated DataFrames. Effect DataFrame is stitched together from varm
         else:
             if model_type == "tree_agg" and select_type == "sslasso":
@@ -999,33 +1008,27 @@
 
         return out
 
 
 def get_a(
     tree: tt.tree,
 ) -> tuple[np.ndarray, int]:
-    """
-    Calculate ancestor matrix from a toytree tree
+    """Calculate ancestor matrix from a toytree tree
+
+    Args:
+        tree: A toytree tree object.
 
-    Parameters
-    ----------
-    tree
-        A toytree tree object
-
-    Returns
-    -------
-    Ancestor matrix and number of nodes without root node
-
-    A
-        Ancestor matrix (numpy array)
-    T
-        number of nodes in the tree, excluding the root node
+    Returns:
+        Ancestor matrix and number of nodes without root node
+        A
+            Ancestor matrix (numpy array)
+        T
+            number of nodes in the tree, excluding the root node
     """
     # Builds ancestor matrix
-
     n_tips = tree.ntips
     n_nodes = tree.nnodes
 
     A_ = np.zeros((n_tips, n_nodes))
 
     for i in np.arange(n_nodes):
         leaves_i = list(set(tree.get_node_descendant_idxs(i)) & set(np.arange(n_tips)))
@@ -1043,30 +1046,25 @@
         A[scrambled_leaves[r], :] = A_[r, :]
     A = A[:, :-1]
 
     return A, n_nodes - 1
 
 
 def collapse_singularities(tree: tt.tree) -> tt.tree:
-    """
-    Collapses (deletes) nodes in a toytree tree that are singularities (have only one child).
+    """Collapses (deletes) nodes in a toytree tree that are singularities (have only one child).
 
-    Parameters
-    ----------
-    tree
-        A toytree tree object
-
-    Returns
-    -------
-    A toytree tree without singularities
+    Args:
+        tree: A toytree tree object
 
-    tree_new
-        A toytree tree
-    """
+    Returns:
+        A toytree tree without singularities
 
+        tree_new
+            A toytree tree
+    """
     A, _ = get_a(tree)
     A_T = A.T
     unq, count = np.unique(A_T, axis=0, return_counts=True)
 
     repeated_idx = []
     for repeated_group in unq[count > 1]:
         repeated_idx.append(np.argwhere(np.all(A_T == repeated_group, axis=1)).ravel())
@@ -1111,33 +1109,25 @@
     else:
         out = a
 
     return out
 
 
 def df2newick(df: pd.DataFrame, levels: list[str], inner_label: bool = True) -> str:
-    """
-    Converts a pandas DataFrame with hierarchical information into a newick string.
+    """Converts a pandas DataFrame with hierarchical information into a newick string.
+
     Adapted from https://stackoverflow.com/questions/15343338/how-to-convert-a-data-frame-to-tree-structure-object-such-as-dendrogram
 
-    Parameters
-    ----------
-    df
-        Pandas DataFrame that has one row for each leaf of the tree and columns that indicate a hierarchical ordering. See the tascCODA tutorial for an example.
-    levels
-        list that indicates how the columns in df are ordered as tree levels. Begins with the root level, ends with the leaf level
-    inner_label
-        Indicator whether labels for inner nodes should be included in the newick string
-
-    Returns
-    -------
-    Newick string describing the tree structure from df
+    Args:
+        df: Pandas DataFrame that has one row for each leaf of the tree and columns that indicate a hierarchical ordering. See the tascCODA tutorial for an example.
+        levels: List that indicates how the columns in df are ordered as tree levels. Begins with the root level, ends with the leaf level
+        inner_label: Indicator whether labels for inner nodes should be included in the newick string
 
-    newick
-        A newick string
+    Returns:
+        Newick string describing the tree structure from df
     """
     df_tax = df.loc[:, [x for x in levels if x in df.columns]]
 
     alevel = pd.unique(df_tax.iloc[:, 0])
     strs = []
     for a in alevel:
         strs.append(traverse(df_tax, a, 0, inner_label))
@@ -1147,36 +1137,30 @@
 
 
 def get_a_2(
     tree: ete.Tree,
     leaf_order: list[str] = None,
     node_order: list[str] = None,
 ) -> tuple[np.ndarray, int]:
-    """
-    Calculate ancestor matrix from a ete3 tree
+    """Calculate ancestor matrix from a ete3 tree.
 
-    Parameters
-    ----------
-    tree
-        A ete3 tree object
-    leaf_order
-        List of leaf names how they should appear as the rows of the ancestor matrix.
-        If None, the ordering will be as in `tree.iter_leaves()`
-    node_order
-        List of node names how they should appear as the columns of the ancestor matrix
-        If None, the ordering will be as in `tree.iter_descendants()`
-
-    Returns
-    -------
-    Ancestor matrix and number of nodes without root node
-
-    A
-        Ancestor matrix (numpy array)
-    T
-        number of nodes in the tree, excluding the root node
+    Args:
+        tree: A ete3 tree object.
+        leaf_order: List of leaf names how they should appear as the rows of the ancestor matrix.
+                    If None, the ordering will be as in `tree.iter_leaves()`
+        node_order: List of node names how they should appear as the columns of the ancestor matrix
+                    If None, the ordering will be as in `tree.iter_descendants()`
+
+    Returns:
+            Ancestor matrix and number of nodes without root node
+
+        A
+            Ancestor matrix (numpy array)
+        T
+            number of nodes in the tree, excluding the root node
     """
     n_tips = len(tree.get_leaves())
     n_nodes = len(tree.get_descendants())
 
     node_names = [n.name for n in tree.iter_descendants()]
     duplicates = [x for x in node_names if node_names.count(x) > 1]
     if len(duplicates) > 0:
@@ -1200,41 +1184,35 @@
         A_ = A_[node_order]
     A_ = np.array(A_)
 
     return A_, n_nodes
 
 
 def collapse_singularities_2(tree: ete.Tree) -> ete.Tree:
-    """
-    Collapses (deletes) nodes in a ete3 tree that are singularities (have only one child).
+    """Collapses (deletes) nodes in a ete3 tree that are singularities (have only one child).
 
-    Parameters
-    ----------
-    tree
-        A ete3 tree object
-
-    Returns
-    -------
-    A ete3 tree without singularities
+    Args:
+        tree: A ete3 tree object
 
-    tree
-        A ete3 tree
+    Returns:
+        A ete3 tree without singularities.
     """
     for node in tree.iter_descendants():
         if len(node.get_children()) == 1:
             node.delete()
 
     return tree
 
 
 def linkage_to_newick(
     Z: np.ndarray,
     labels: list[str],
 ) -> str:
     """Convert a linkage matrix to newick tree string.
+
     Adapted from https://stackoverflow.com/a/31878514/20299702.
 
     Args:
         Z: linkage matrix
         labels: leaf labels
 
     Returns:
@@ -1265,14 +1243,15 @@
     dendrogram_key: str = None,
     levels_orig: list[str] = None,
     levels_agg: list[str] = None,
     add_level_name: bool = True,
     key_added: str = "tree",
 ):
     """Generate ete tree for tascCODA models from dendrogram information or cell-level observations.
+
     Trees can either be generated from scipy dendrogram information e.g. from scanpy.tl.dendrogram,
     or from hierarchical information for each cell type - either saved in `.obs` of the cell-level data object, or in `.var` of the aggregated data.
 
     Notes:
     - Either `dendrogram_key`, `levels_orig` or `levels_agg` must be not None. Priority is `dendrogram_key` -> `levels_orig` -> `levels_agg`
     - If `data` is a MuData object, `modality_1` and `modality_2` must be specified
     - The node names of the generated tree must be unique. Often, setting `add_level_name=True` is enough to achieve that.
@@ -1351,16 +1330,15 @@
     adata: AnnData,
     cell_type_identifier: str,
     sample_identifier: str | list[str],
     covariate_uns: str | None = None,
     covariate_obs: list[str] | None = None,
     covariate_df: pd.DataFrame | None = None,
 ) -> AnnData:
-    """
-    Creates a compositional analysis dataset from a single anndata object, as it is produced by e.g. scanpy.
+    """Creates a compositional analysis dataset from a single AnnData object, as it is produced by e.g. scanpy.
 
     The anndata object needs to have a column in adata.obs that contains the cell type assignment.
     Further, it must contain one column or a set of columns (e.g. subject id, treatment, disease status) that uniquely identify each (statistical) sample.
     Further covariates (e.g. subject age) can either be specified via addidional column names in adata.obs, a key in adata.uns, or as a separate DataFrame.
 
     NOTE: The order of samples in the returned dataset is determined by the first occurence of cells from each sample in `adata`
 
@@ -1370,27 +1348,25 @@
         sample_identifier: column name or list of column names in adata.obs that uniquely identify each sample
         covariate_uns: key for adata.uns, where covariate values are stored
         covariate_obs: list of column names in adata.obs, where covariate values are stored. Note: If covariate values are not unique for a value of sample_identifier, this covaariate will be skipped.
         covariate_df: DataFrame with covariates
 
     Returns:
         AnnData: A data set with cells aggregated to the (sample x cell type) level
-
     """
-
-    if type(sample_identifier) == str:
+    if isinstance(sample_identifier, str):
         sample_identifier = [sample_identifier]
 
     if covariate_obs:
         covariate_obs += [i for i in sample_identifier if i not in covariate_obs]
     else:
         covariate_obs = sample_identifier  # type: ignore
 
     # join sample identifiers
-    if type(sample_identifier) == list:
+    if isinstance(sample_identifier, list):
         adata.obs["scCODA_sample_id"] = adata.obs[sample_identifier].agg("-".join, axis=1)
         sample_identifier = "scCODA_sample_id"
 
     # get cell type counts
     groups = adata.obs.value_counts([sample_identifier, cell_type_identifier])
     count_data = groups.unstack(level=cell_type_identifier)
     count_data = count_data.fillna(0)
```

### Comparing `pertpy-0.4.0/pertpy/tools/_coda/_sccoda.py` & `pertpy-0.5.0/pertpy/tools/_coda/_sccoda.py`

 * *Files 21% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def load(
         self,
         adata: AnnData,
         type: Literal["cell_level", "sample_level"],
-        generate_sample_level: bool = False,
+        generate_sample_level: bool = True,
         cell_type_identifier: str = None,
         sample_identifier: str = None,
         covariate_uns: str | None = None,
         covariate_obs: list[str] | None = None,
         covariate_df: pd.DataFrame | None = None,
         modality_key_1: str = "rna",
         modality_key_2: str = "coda",
@@ -68,42 +68,39 @@
         When using ``type="cell_level"``, ``adata`` needs to have a column in ``adata.obs`` that contains the cell type assignment.
         Further, it must contain one column or a set of columns (e.g. subject id, treatment, disease status) that uniquely identify each (statistical) sample.
         Further covariates (e.g. subject age) can either be specified via addidional column names in ``adata.obs``, a key in ``adata.uns``, or as a separate DataFrame.
 
         Args:
             adata: AnnData object.
             type : Specify the input adata type, which could be either a cell-level AnnData or an aggregated sample-level AnnData.
+            generate_sample_level: Whether to generate an AnnData object on the sample level or create an empty AnnData object.
             cell_type_identifier: If type is "cell_level", specify column name in adata.obs that specifies the cell types. Defaults to None.
             sample_identifier: If type is "cell_level", specify column name in adata.obs that specifies the sample. Defaults to None.
             covariate_uns: If type is "cell_level", specify key for adata.uns, where covariate values are stored. Defaults to None.
             covariate_obs: If type is "cell_level", specify list of keys for adata.obs, where covariate values are stored. Defaults to None.
             covariate_df: If type is "cell_level", specify dataFrame with covariates. Defaults to None.
             modality_key_1: Key to the cell-level AnnData in the MuData object. Defaults to "rna".
             modality_key_2: Key to the aggregated sample-level AnnData object in the MuData object. Defaults to "coda".
 
         Returns:
             MuData: MuData object with cell-level AnnData (`mudata[modality_key_1]`) and aggregated sample-level AnnData (`mudata[modality_key_2]`).
 
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                mdata = sccoda.load(
-                    adata,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> mdata = sccoda.load(
+            >>>     adata,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
         """
-
         if type == "cell_level":
             if generate_sample_level:
                 adata_coda = from_scanpy(
                     adata=adata,
                     cell_type_identifier=cell_type_identifier,
                     sample_identifier=sample_identifier,
                     covariate_uns=covariate_uns,
@@ -143,30 +140,28 @@
 
             Specifically, parameters have been set:
 
             - `adata.uns["param_names"]` or `data[modality_key].uns["param_names"]`: List with the names of all tracked latent model parameters (through `npy.sample` or `npy.deterministic`)
             - `adata.uns["scCODA_params"]["model_type"]` or `data[modality_key].uns["scCODA_params"]["model_type"]`: String indicating the model type ("classic")
             - `adata.uns["scCODA_params"]["select_type"]` or `data[modality_key].uns["scCODA_params"]["select_type"]`: String indicating the type of spike_and_slab selection ("spikeslab")
 
-        Example:
-            .. code-block:: python
+        Examples:
+            >>> import pertpy as pt
 
-                import pertpy as pt
-
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                mdata = sccoda.load(
-                    adata,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
-                mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> mdata = sccoda.load(
+            >>>     adata,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
+            >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
         """
         if isinstance(data, MuData):
             adata = data[modality_key]
             is_MuData = True
         if isinstance(data, AnnData):
             adata = data
             is_MuData = False
@@ -189,52 +184,73 @@
 
         if is_MuData:
             data.mod[modality_key] = adata
             return data
         else:
             return adata
 
-    def model(  # type: ignore
-        self,
-        counts: np.ndarray,
-        covariates: np.ndarray,
-        n_total: np.ndarray,
-        ref_index,
-        sample_adata: AnnData,
-    ):
+    def set_init_mcmc_states(self, rng_key: None, ref_index: np.ndarray, sample_adata: AnnData) -> AnnData:  # type: ignore
         """
-        Implements scCODA model in numpyro
+        Sets initial MCMC state values for scCODA model
 
         Args:
-            counts: Count data array
-            covariates: Covariate matrix
-            n_total: Number of counts per sample
+            rng_key: RNG value to be set
             ref_index: Index of reference feature
             sample_adata: Anndata object with cell counts as sample_adata.X and covariates saved in sample_adata.obs.
 
         Returns:
-            predictions (see numpyro documentation for details on models)
+            Return AnnData object.
         """
         # data dimensions
         N, D = sample_adata.obsm["covariate_matrix"].shape
         P = sample_adata.X.shape[1]
 
         # Sizes of different parameter matrices
         alpha_size = [P]
         sigma_size = [D, 1]
         beta_nobl_size = [D, P - 1]
 
         # Initial MCMC states
+        if rng_key is not None:
+            np.random.seed(rng_key)
+
         sample_adata.uns["scCODA_params"]["mcmc"]["init_params"] = {
             "sigma_d": np.ones(dtype=np.float64, shape=sigma_size),
             "b_offset": np.random.normal(0.0, 1.0, beta_nobl_size),
             "ind_raw": np.zeros(dtype=np.float64, shape=beta_nobl_size),
             "alpha": np.random.normal(0.0, 1.0, alpha_size),
         }
 
+        return sample_adata
+
+    def model(  # type: ignore
+        self,
+        counts: np.ndarray,
+        covariates: np.ndarray,
+        n_total: np.ndarray,
+        ref_index,
+        sample_adata: AnnData,
+    ):
+        """
+        Implements scCODA model in numpyro
+
+        Args:
+            counts: Count data array
+            covariates: Covariate matrix
+            n_total: Number of counts per sample
+            ref_index: Index of reference feature
+            sample_adata: Anndata object with cell counts as sample_adata.X and covariates saved in sample_adata.obs.
+
+        Returns:
+            predictions (see numpyro documentation for details on models)
+        """
+        # data dimensions
+        N, D = sample_adata.obsm["covariate_matrix"].shape
+        P = sample_adata.X.shape[1]
+
         # numpyro plates for all dimensions
         covariate_axis = npy.plate("covs", D, dim=-2)
         cell_type_axis = npy.plate("ct", P, dim=-1)
         cell_type_axis_nobl = npy.plate("ctnb", P - 1, dim=-1)
         sample_axis = npy.plate("sample", N, dim=-2)
 
         # Effect priors
@@ -291,35 +307,32 @@
             rng_key: The rng state used for the prior simulation. If None, a random state will be selected. Defaults to None.
             num_prior_samples: Number of prior samples calculated. Defaults to 500.
             use_posterior_predictive: If True, the posterior predictive will be calculated. Defaults to True.
 
         Returns:
             az.InferenceData: arviz_data with all MCMC information
 
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
-                mdata_salm = sccoda.load(
-                    adata_salm,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
-                mdata_salm = sccoda.prepare(
-                    mdata_salm, formula="condition", reference_cell_type="Goblet"
-                )
-                sccoda.run_nuts(mdata_salm)
-                sccoda.make_arviz(mdata_salm, num_prior_samples=100)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
+            >>> mdata_salm = sccoda.load(
+            >>>     adata_salm,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
+            >>> mdata_salm = sccoda.prepare(
+            >>>     mdata_salm, formula="condition", reference_cell_type="Goblet"
+            >>> )
+            >>> sccoda.run_nuts(mdata_salm)
+            >>> sccoda.make_arviz(mdata_salm, num_prior_samples=100)
         """
         if isinstance(data, MuData):
             try:
                 sample_adata = data[modality_key]
             except IndexError:
                 print("When data is a MuData object, modality_key must be specified!")
                 raise
@@ -404,113 +417,102 @@
         num_warmup: int = 1000,
         rng_key: int = None,
         copy: bool = False,
         *args,
         **kwargs,
     ):
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                mdata = sccoda.load(
-                    adata,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
-                mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
-                sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> mdata = sccoda.load(
+            >>>     adata,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
+            >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
+            >>> sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000)
         """
         return super().run_nuts(data, modality_key, num_samples, num_warmup, rng_key, copy, *args, **kwargs)
 
     run_nuts.__doc__ = CompositionalModel2.run_nuts.__doc__ + run_nuts.__doc__
 
     def credible_effects(self, data: AnnData | MuData, modality_key: str = "coda", est_fdr: float = None) -> pd.Series:
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
-                mdata_salm = sccoda.load(
-                    adata_salm,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
-                mdata_salm = sccoda.prepare(
-                    mdata_salm, formula="condition", reference_cell_type="Goblet"
-                )
-                sccoda.run_nuts(mdata_salm)
-                sccoda.credible_effects(mdata_salm)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
+            >>> mdata_salm = sccoda.load(
+            >>>     adata_salm,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
+            >>> mdata_salm = sccoda.prepare(
+            >>>     mdata_salm, formula="condition", reference_cell_type="Goblet"
+            >>> )
+            >>> sccoda.run_nuts(mdata_salm)
+            >>> sccoda.credible_effects(mdata_salm)
         """
         return super().credible_effects(data, modality_key, est_fdr)
 
     credible_effects.__doc__ = CompositionalModel2.credible_effects.__doc__ + credible_effects.__doc__
 
     def summary(self, data: AnnData | MuData, extended: bool = False, modality_key: str = "coda", *args, **kwargs):
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
-                mdata_salm = sccoda.load(
-                    adata_salm,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
-                mdata_salm = sccoda.prepare(
-                    mdata_salm, formula="condition", reference_cell_type="Goblet"
-                )
-                sccoda.run_nuts(mdata_salm)
-                sccoda.summary(mdata_salm)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
+            >>> mdata_salm = sccoda.load(
+            >>>     adata_salm,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
+            >>> mdata_salm = sccoda.prepare(
+            >>>     mdata_salm, formula="condition", reference_cell_type="Goblet"
+            >>> )
+            >>> sccoda.run_nuts(mdata_salm)
+            >>> sccoda.summary(mdata_salm)
         """
         return super().summary(data, extended, modality_key, *args, **kwargs)
 
     summary.__doc__ = CompositionalModel2.summary.__doc__ + summary.__doc__
 
     def set_fdr(self, data: AnnData | MuData, est_fdr: float, modality_key: str = "coda", *args, **kwargs):
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
+        Examples:
+            >>> import pertpy as pt
 
-                adata = pt.dt.haber_2017_regions()
-                sccoda = pt.tl.Sccoda()
-                adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
-                mdata_salm = sccoda.load(
-                    adata_salm,
-                    type="cell_level",
-                    generate_sample_level=True,
-                    cell_type_identifier="cell_label",
-                    sample_identifier="batch",
-                    covariate_obs=["condition"],
-                )
-                mdata_salm = sccoda.prepare(
-                    mdata_salm, formula="condition", reference_cell_type="Goblet"
-                )
-                sccoda.run_nuts(mdata_salm)
-                sccoda.set_fdr(mdata_salm, est_fdr=0.4)
-                sccoda.summary(mdata_salm)
+            >>> adata = pt.dt.haber_2017_regions()
+            >>> sccoda = pt.tl.Sccoda()
+            >>> adata_salm = adata[adata.obs["condition"].isin(["Control", "Salmonella"])]
+            >>> mdata_salm = sccoda.load(
+            >>>     adata_salm,
+            >>>     type="cell_level",
+            >>>     generate_sample_level=True,
+            >>>     cell_type_identifier="cell_label",
+            >>>     sample_identifier="batch",
+            >>>     covariate_obs=["condition"],
+            >>> )
+            >>> mdata_salm = sccoda.prepare(
+            >>>     mdata_salm, formula="condition", reference_cell_type="Goblet"
+            >>> )
+            >>> sccoda.run_nuts(mdata_salm)
+            >>> sccoda.set_fdr(mdata_salm, est_fdr=0.4)
+            >>> sccoda.summary(mdata_salm)
         """
         return super().set_fdr(data, est_fdr, modality_key, *args, **kwargs)
 
     set_fdr.__doc__ = CompositionalModel2.set_fdr.__doc__ + set_fdr.__doc__
```

### Comparing `pertpy-0.4.0/pertpy/tools/_coda/_tasccoda.py` & `pertpy-0.5.0/pertpy/tools/_coda/_tasccoda.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,26 +97,23 @@
             key_added: If not specified, the tree is stored in .uns[‘tree’]. If `data` is AnnData, save tree in `data`. If `data` is MuData, save tree in data[modality_2]. Defaults to "tree".
             modality_key_1: Key to the cell-level AnnData in the MuData object. Defaults to "rna".
             modality_key_2: Key to the aggregated sample-level AnnData object in the MuData object. Defaults to "coda".
 
         Returns:
             MuData: MuData object with cell-level AnnData (`mudata[modality_key_1]`) and aggregated sample-level AnnData (`mudata[modality_key_2]`).
 
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
         """
 
         if type == "cell_level":
             adata_coda = from_scanpy(
                 adata=adata,
                 cell_type_identifier=cell_type_identifier,
                 sample_identifier=sample_identifier,
@@ -170,29 +167,26 @@
 
             Specifically, parameters have been set:
 
             - `adata.uns["param_names"]` or `data[modality_key].uns["param_names"]`: List with the names of all tracked latent model parameters (through `npy.sample` or `npy.deterministic`)
             - `adata.uns["scCODA_params"]["model_type"]` or `data[modality_key].uns["scCODA_params"]["model_type"]`: String indicating the model type ("classic")
             - `adata.uns["scCODA_params"]["select_type"]` or `data[modality_key].uns["scCODA_params"]["select_type"]`: String indicating the type of spike_and_slab selection ("spikeslab")
 
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
-                mdata = tasccoda.prepare(
-                    mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
-                )
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
+            >>> mdata = tasccoda.prepare(
+            >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
+            >>> )
         """
         if pen_args is None:
             pen_args = {"lambda_1": 5}
         if isinstance(data, MuData):
             adata = data[modality_key]
             is_MuData = True
         if isinstance(data, AnnData):
@@ -200,15 +194,15 @@
             is_MuData = False
         adata = super().prepare(adata, formula, reference_cell_type, automatic_reference_absence_threshold)
 
         if tree_key is None:
             raise ValueError("Please specify the key in .uns that contains the tree structure!")
 
         # toytree tree - only for legacy reasons, can be removed in the final version
-        if type(adata.uns[tree_key]) == tt.tree:
+        if isinstance(adata.uns[tree_key], tt.tree):
             # Collapse singularities in the tree
             phy_tree = collapse_singularities(adata.uns[tree_key])
 
             # Get ancestor matrix
             A, T = get_a(phy_tree)
             adata.uns["scCODA_params"]["ancestor_matrix"] = A
             adata.uns["scCODA_params"]["T"] = T
@@ -234,15 +228,15 @@
             # number of leaves for each internal node (important for aggregation penalty lambda_1)
             if "node_leaves" not in pen_args:
                 node_leaves = [len(n.get_leaves()) for n in phy_tree.idx_dict.values()]
                 node_leaves.reverse()
                 pen_args["node_leaves"] = np.delete(np.array(node_leaves[:-1]), refs)
 
         # ete tree
-        elif type(adata.uns[tree_key]) == ete.Tree:
+        elif isinstance(adata.uns[tree_key], ete.Tree):
             # Collapse singularities in the tree
             phy_tree = collapse_singularities_2(adata.uns[tree_key])
 
             node_names = [n.name for n in phy_tree.iter_descendants()]
 
             # Get ancestor matrix
             A, T = get_a_2(phy_tree, leaf_order=adata.var.index.tolist(), node_order=node_names)
@@ -301,41 +295,38 @@
         adata.uns["scCODA_params"]["select_type"] = "sslasso"
         if is_MuData:
             data.mod[modality_key] = adata
             return data
         else:
             return adata
 
-    def model(  # type: ignore
-        self,
-        counts: np.ndarray,
-        covariates: np.ndarray,
-        n_total: int,
-        ref_index: np.ndarray,
-        sample_adata: AnnData,
-    ):
-        """Implements tascCODA model in numpyro
+    def set_init_mcmc_states(self, rng_key: None, ref_index: np.ndarray, sample_adata: AnnData) -> AnnData:  # type: ignore
+        """
+        Sets initial MCMC state values for scCODA model
 
         Args:
-            counts: Count data array
-            covariates: Covariate matrix
-            n_total: Number of counts per sample
+            rng_key: RNG value to be set
             ref_index: Index of reference feature
             sample_adata: Anndata object with cell counts as sample_adata.X and covariates saved in sample_adata.obs.
 
         Returns:
-            predictions (see numpyro documentation for details on models)
+            Return AnnData
         """
-        # data dimensions
-        dtype = "float64"
-
         N, D = sample_adata.obsm["covariate_matrix"].shape
         P = sample_adata.X.shape[1]
         T = sample_adata.uns["scCODA_params"]["T"]
 
+        # Reference nodes must be sorted by index
+        ref_index = np.sort(ref_index)
+        num_ref_nodes = len(ref_index)
+
+        # Sizes of different parameter matrices
+        alpha_size = [P]
+        beta_nobl_size = [D, T - num_ref_nodes]
+
         # spike-and-slab LASSO parameters
         lambda_0 = sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["lambda_0"]
         # tree-based scaled penalty
         penalty_scale_factor = np.array(
             (
                 1
                 / (
@@ -343,40 +334,69 @@
                     + np.exp(
                         -1
                         * sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["phi"]
                         * (sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["node_leaves"] / P - 0.5)
                     )
                 )
             ),
-            dtype,
         )
         lambda_1 = 2 * sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["lambda_1"] * penalty_scale_factor
         sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["lambda_1_scaled"] = lambda_1
 
-        # Reference nodes must be sorted by index
-        ref_index = jnp.sort(ref_index)
-        num_ref_nodes = len(ref_index)
-
-        # Sizes of different parameter matrices
-        alpha_size = [P]
-        beta_nobl_size = [D, T - num_ref_nodes]
-
-        # Size of inferred parameter matrix
-        d = D * (T - num_ref_nodes)
-
         # Initial MCMC states
+        if rng_key is not None:
+            np.random.seed(rng_key)
+
         sample_adata.uns["scCODA_params"]["mcmc"]["init_params"] = {
             "a_0": np.ones(dtype=np.float64, shape=beta_nobl_size) * 1 / lambda_0,
             "b_raw_0": np.random.normal(0.0, 1.0, beta_nobl_size),
             "a_1": np.ones(dtype=np.float64, shape=beta_nobl_size) * 1 / lambda_1,
             "b_raw_1": np.random.normal(0.0, 1.0, beta_nobl_size),
             "theta": np.ones(dtype=np.float64, shape=1) * 0.5,
             "alpha": np.random.normal(0.0, 1.0, alpha_size),
         }
 
+        return sample_adata
+
+    def model(  # type: ignore
+        self,
+        counts: np.ndarray,
+        covariates: np.ndarray,
+        n_total: int,
+        ref_index: np.ndarray,
+        sample_adata: AnnData,
+    ):
+        """Implements tascCODA model in numpyro
+
+        Args:
+            counts: Count data array
+            covariates: Covariate matrix
+            n_total: Number of counts per sample
+            ref_index: Index of reference feature
+            sample_adata: Anndata object with cell counts as sample_adata.X and covariates saved in sample_adata.obs.
+
+        Returns:
+            predictions (see numpyro documentation for details on models)
+        """
+        # data dimensions
+        N, D = sample_adata.obsm["covariate_matrix"].shape
+        P = sample_adata.X.shape[1]
+        T = sample_adata.uns["scCODA_params"]["T"]
+
+        # spike-and-slab LASSO parameters
+        lambda_0 = sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["lambda_0"]
+        lambda_1 = sample_adata.uns["scCODA_params"]["sslasso_pen_args"]["lambda_1_scaled"]
+
+        # Reference nodes must be sorted by index
+        ref_index = jnp.sort(ref_index)
+        num_ref_nodes = len(ref_index)
+
+        # Size of inferred parameter matrix
+        d = D * (T - num_ref_nodes)
+
         # numpyro plates for all dimensions
         covariate_axis = npy.plate("covs", D, dim=-2)
         node_axis = npy.plate("ct", T, dim=-1)
         node_axis_nobl = npy.plate("ctnb", T - num_ref_nodes, dim=-1)
         cell_type_axis = npy.plate("ct", P, dim=-1)
         sample_axis = npy.plate("sample", N, dim=-2)
 
@@ -438,31 +458,28 @@
             rng_key: The rng state used for the prior simulation. If None, a random state will be selected. Defaults to None.
             num_prior_samples: Number of prior samples calculated. Defaults to 500.
             use_posterior_predictive: If True, the posterior predictive will be calculated. Defaults to True.
 
         Returns:
             arviz.InferenceData: arviz_data
 
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
-                mdata = tasccoda.prepare(
-                    mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
-                )
-                tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
-                tasccoda.make_arviz(mdata)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
+            >>> mdata = tasccoda.prepare(
+            >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
+            >>> )
+            >>> tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
+            >>> tasccoda.make_arviz(mdata)
         """
         if isinstance(data, MuData):
             try:
                 sample_adata = data[modality_key]
             except IndexError:
                 print("When data is a MuData object, modality_key must be specified!")
                 raise
@@ -551,99 +568,87 @@
         num_warmup: int = 1000,
         rng_key: int = None,
         copy: bool = False,
         *args,
         **kwargs,
     ):
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
-                mdata = tasccoda.prepare(
-                    mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
-                )
-                tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
+            >>> mdata = tasccoda.prepare(
+            >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
+            >>> )
+            >>> tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
         """
         return super().run_nuts(data, modality_key, num_samples, num_warmup, rng_key, copy, *args, **kwargs)
 
     run_nuts.__doc__ = CompositionalModel2.run_nuts.__doc__ + run_nuts.__doc__
 
     def summary(self, data: AnnData | MuData, extended: bool = False, modality_key: str = "coda", *args, **kwargs):
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
-                mdata = tasccoda.prepare(
-                    mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
-                )
-                tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
-                tasccoda.summary(mdata)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
+            >>> mdata = tasccoda.prepare(
+            >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
+            >>> )
+            >>> tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
+            >>> tasccoda.summary(mdata)
         """
         return super().summary(data, extended, modality_key, *args, **kwargs)
 
     summary.__doc__ = CompositionalModel2.summary.__doc__ + summary.__doc__
 
     def credible_effects(self, data: AnnData | MuData, modality_key: str = "coda", est_fdr: float = None) -> pd.Series:
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
-                mdata = tasccoda.prepare(
-                    mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
-                )
-                tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
-                tasccoda.credible_effects(mdata)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
+            >>> mdata = tasccoda.prepare(
+            >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
+            >>> )
+            >>> tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
+            >>> tasccoda.credible_effects(mdata)
         """
         return super().credible_effects(data, modality_key, est_fdr)
 
     credible_effects.__doc__ = CompositionalModel2.credible_effects.__doc__ + credible_effects.__doc__
 
     def set_fdr(self, data: AnnData | MuData, est_fdr: float, modality_key: str = "coda", *args, **kwargs):
         """
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.smillie()
-                tasccoda = pt.tl.Tasccoda()
-                mdata = tasccoda.load(
-                    adata, type="sample_level",
-                    levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
-                    key_added="lineage", add_level_name=True
-                )
-                mdata = tasccoda.prepare(
-                    mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
-                )
-                tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
-                tasccoda.set_fdr(mdata_salm, est_fdr=0.4)
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.smillie()
+            >>> tasccoda = pt.tl.Tasccoda()
+            >>> mdata = tasccoda.load(
+            >>>     adata, type="sample_level",
+            >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
+            >>>     key_added="lineage", add_level_name=True
+            >>> )
+            >>> mdata = tasccoda.prepare(
+            >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
+            >>> )
+            >>> tasccoda.run_nuts(mdata, num_samples=1000, num_warmup=100)
+            >>> tasccoda.set_fdr(mdata_salm, est_fdr=0.4)
         """
         return super().set_fdr(data, est_fdr, modality_key, *args, **kwargs)
 
     set_fdr.__doc__ = CompositionalModel2.set_fdr.__doc__ + set_fdr.__doc__
```

### Comparing `pertpy-0.4.0/pertpy/tools/_dialogue.py` & `pertpy-0.5.0/pertpy/tools/_dialogue.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/tools/_differential_gene_expression.py` & `pertpy-0.5.0/pertpy/tools/_differential_gene_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,8 +90,8 @@
             Depending on the method a Pandas DataFrame containing at least:
             * gene_id
             * log2 fold change
             * mean expression
             * unadjusted p-value
             * adjusted p-value
         """
-        pass
+        raise NotImplementedError
```

### Comparing `pertpy-0.4.0/pertpy/tools/_distances/_distance_tests.py` & `pertpy-0.5.0/pertpy/tools/_distances/_distance_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,19 @@
     Args:
         metric: Distance metric to use.
         n_perms: Number of permutations to run. Defaults to 1000.
         obsm_key: Name of embedding to use for distance computation. Defaults to 'X_pca'.
         alpha: Significance level. Defaults to 0.05.
         correction: Multiple testing correction method. Defaults to 'holm-sidak'.
 
-    Example:
-        .. code-block:: python
-
-            import pertpy as pt
-
-            adata = pt.dt.distance_example_data()
-            etest = pt.tl.DistanceTest('edistance', n_perms=1000)
-            tab = etest(adata, groupby='perturbation', contrast='control')
+    Examples:
+        >>> import pertpy as pt
+        >>> adata = pt.dt.distance_example_data()
+        >>> etest = pt.tl.DistanceTest('edistance', n_perms=1000)
+        >>> tab = etest(adata, groupby='perturbation', contrast='control')
     """
 
     def __init__(
         self,
         metric: str,
         n_perms: int = 1000,
         obsm_key: str = "X_pca",
@@ -64,22 +61,19 @@
             pandas.DataFrame: Results of the permutation test, with columns:
                 - distance: distance between the contrast group and the group
                 - pvalue: p-value of the permutation test
                 - significant: whether the group is significantly different from the contrast group
                 - pvalue_adj: p-value after multiple testing correction
                 - significant_adj: whether the group is significantly different from the contrast group after multiple testing correction
 
-        Example:
-            .. code-block:: python
-
-                import pertpy as pt
-
-                adata = pt.dt.distance_example_data()
-                etest = pt.tl.DistanceTest('edistance', n_perms=1000)
-                tab = etest(adata, groupby='perturbation', contrast='control')
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.distance_example_data()
+            >>> etest = pt.tl.DistanceTest('edistance', n_perms=1000)
+            >>> tab = etest(adata, groupby='perturbation', contrast='control')
         """
         if Distance(self.metric, self.obsm_key).metric_fct.accepts_precomputed:
             # Much faster if the metric can be called on the precomputed
             # distance matrix, but not all metrics can do that.
             return self.test_precomputed(adata, groupby, contrast, cell_wise_metric, verbose)
         else:
             return self.test_xy(adata, groupby, contrast, verbose)
@@ -190,15 +184,14 @@
             pandas.DataFrame: Results of the permutation test, with columns:
                 - distance: distance between the contrast group and the group
                 - pvalue: p-value of the permutation test
                 - significant: whether the group is significantly different from the contrast group
                 - pvalue_adj: p-value after multiple testing correction
                 - significant_adj: whether the group is significantly different from the contrast group after multiple testing correction
         """
-
         distance = Distance(self.metric, self.obsm_key)
         if not distance.metric_fct.accepts_precomputed:
             raise ValueError(f"Metric {self.metric} does not accept precomputed distances.")
 
         groups = adata.obs[groupby].unique()
         if contrast not in groups:
             raise ValueError(f"Contrast group {contrast} not found in {groupby} of adata.obs.")
```

### Comparing `pertpy-0.4.0/pertpy/tools/_distances/_distances.py` & `pertpy-0.5.0/pertpy/tools/_distances/_distances.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             D = Distance(X, Y)
     """
 
     def __init__(
         self,
         metric: str = "edistance",
         obsm_key: str = "X_pca",
-    ) -> None:
+    ):
         """Initialize Distance class.
 
         Args:
             metric: Distance metric to use. Defaults to "edistance".
             obsm_key: Name of embedding in adata.obsm to use. Defaults to "X_pca".
         """
         metric_fct: AbstractDistance = None
@@ -113,14 +113,15 @@
 
     def pairwise(
         self,
         adata: AnnData,
         groupby: str,
         groups: list[str] | None = None,
         verbose: bool = True,
+        n_jobs: int = 1,
         **kwargs,
     ) -> pd.DataFrame:
         """Get pairwise distances between groups of cells.
 
         Args:
             adata: Annotated data matrix.
             groupby: Column name in adata.obs.
@@ -144,15 +145,15 @@
         grouping = adata.obs[groupby].copy()
         df = pd.DataFrame(index=groups, columns=groups, dtype=float)
         fct = track if verbose else lambda iterable: iterable
 
         if self.metric_fct.accepts_precomputed:
             # Precompute the pairwise distances if needed
             if f"{self.obsm_key}_predistances" not in adata.obsp.keys():
-                self.precompute_distances(adata, **kwargs)
+                self.precompute_distances(adata, n_jobs=n_jobs, **kwargs)
             pwd = adata.obsp[f"{self.obsm_key}_predistances"]
             for index_x, group_x in enumerate(fct(groups)):
                 idx_x = grouping == group_x
                 for group_y in groups[index_x:]:
                     if group_x == group_y:
                         dist = 0.0
                     else:
@@ -175,28 +176,28 @@
                     df.loc[group_x, group_y] = dist
                     df.loc[group_y, group_x] = dist
         df.index.name = groupby
         df.columns.name = groupby
         df.name = f"pairwise {self.metric}"
         return df
 
-    def precompute_distances(self, adata: AnnData, cell_wise_metric: str = "euclidean") -> None:
+    def precompute_distances(self, adata: AnnData, cell_wise_metric: str = "euclidean", n_jobs: int = None) -> None:
         """Precompute pairwise distances between all cells, writes to adata.obsp.
 
         The precomputed distances are stored in adata.obsp under the key
         '{self.obsm_key}_predistances', as they depend on the embedding used.
 
         Args:
             adata: Annotated data matrix.
             obs_key: Column name in adata.obs.
             cell_wise_metric: Metric to use for pairwise distances.
         """
         # Precompute the pairwise distances
         cells = adata.obsm[self.obsm_key].copy()
-        pwd = pairwise_distances(cells, cells, metric=cell_wise_metric)
+        pwd = pairwise_distances(cells, cells, metric=cell_wise_metric, n_jobs=n_jobs)
         # Write to adata.obsp
         adata.obsp[f"{self.obsm_key}_predistances"] = pwd
 
 
 class AbstractDistance(ABC):
     """Abstract class of distance metrics between two sets of vectors."""
 
@@ -229,15 +230,14 @@
 
         Returns:
             float: Distance between X and Y.
         """
         raise NotImplementedError("Metric class is abstract.")
 
 
-# Specific distance metrics
 class Edistance(AbstractDistance):
     """Edistance metric."""
 
     def __init__(self) -> None:
         super().__init__()
         self.accepts_precomputed = True
```

### Comparing `pertpy-0.4.0/pertpy/tools/_kernel_pca.py` & `pertpy-0.5.0/pertpy/tools/_kernel_pca.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/tools/_metadata/_cell_line.py` & `pertpy-0.5.0/pertpy/tools/_metadata/_cell_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
                 "Please choose either broad or sanger."
             )
 
     def getinfo_annotate_cell_lines(self, cell_line_source: str = "DepMap") -> None:
         """A brief summary of cell line metadata.
 
         Args:
-            cell_line_source: the source of cell line annotation: DepMap or Cancerrxgene. (default: "DepMap")
+            cell_line_source: the source of cell line annotation: DepMap or Cancerrxgene. Defaults to "DepMap".
         """
         if cell_line_source == "DepMap":
             print(
                 "Current available information in the DepMap cell line annotation: ",
                 *list(self.cell_line_meta.columns.values),
                 sep="\n- ",
             )
```

### Comparing `pertpy-0.4.0/pertpy/tools/_milo.py` & `pertpy-0.5.0/pertpy/tools/_milo.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,17 @@
         if pd.api.types.is_numeric_dtype(adata.obs[anno_col]):
             raise ValueError(
                 "adata.obs[anno_col] is not of categorical type - please use milopy.utils.annotate_nhoods_continuous for continuous variables"
             )
 
         anno_dummies = pd.get_dummies(adata.obs[anno_col])
         anno_count = adata.obsm["nhoods"].T.dot(csr_matrix(anno_dummies.values))
-        anno_frac = np.array(anno_count / anno_count.sum(1))
+        anno_count_dense = anno_count.toarray()
+        anno_sum = anno_count_dense.sum(1)
+        anno_frac = np.divide(anno_count_dense, anno_sum[:, np.newaxis])
 
         anno_frac_dataframe = pd.DataFrame(anno_frac, columns=anno_dummies.columns, index=sample_adata.var_names)
         sample_adata.varm["frac_annotation"] = anno_frac_dataframe.values
         sample_adata.uns["annotation_labels"] = anno_frac_dataframe.columns
         sample_adata.uns["annotation_obs"] = anno_col
         sample_adata.var["nhood_annotation"] = anno_frac_dataframe.idxmax(1)
         sample_adata.var["nhood_annotation_frac"] = anno_frac_dataframe.max(1)
```

### Comparing `pertpy-0.4.0/pertpy/tools/_mixscape.py` & `pertpy-0.5.0/pertpy/tools/_mixscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import warnings
 
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from anndata import AnnData
-from pynndescent import NNDescent
 from rich import print
 from scanpy.tools._utils import _choose_representation
 from scipy import sparse
 from scipy.sparse import csr_matrix, issparse, spmatrix
 from sklearn.mixture import GaussianMixture
 
 import pertpy as pt
@@ -83,14 +82,16 @@
 
         for split_mask in split_masks:
             control_mask_split = control_mask & split_mask
 
             R_split = R[split_mask]
             R_control = R[control_mask_split]
 
+            from pynndescent import NNDescent  # saves a lot of import time
+
             eps = kwargs.pop("epsilon", 0.1)
             nn_index = NNDescent(R_control, **kwargs)
             indices, _ = nn_index.query(R_split, k=n_neighbors, epsilon=eps)
 
             X_control = np.expm1(adata.X[control_mask_split])
 
             n_split = split_mask.sum()
```

### Comparing `pertpy-0.4.0/pertpy/tools/_scgen/_base_components.py` & `pertpy-0.5.0/pertpy/tools/_scgen/_base_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         mean_x = nn.Dense(self.n_latent)(x)
         logvar_x = nn.Dense(self.n_latent)(x)
 
         return mean_x, self.var_activation(logvar_x)
 
 
 class FlaxDecoder(nn.Module):
-
     n_output: int
     n_layers: int = 1
     n_hidden: int = 128
     dropout_rate: float = 0.2
     use_batch_norm: bool = False
     use_layer_norm: bool = False
     activation_fn: nn.activation = nn.activation.leaky_relu  # type: ignore
```

### Comparing `pertpy-0.4.0/pertpy/tools/_scgen/_jax_scgen.py` & `pertpy-0.5.0/pertpy/tools/_scgen/_jax_scgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import Any, Sequence
 
 import jax.numpy as jnp
 import numpy as np
 from anndata import AnnData
+from jax import Array
 from scvi import REGISTRY_KEYS
 from scvi.data import AnnDataManager
 from scvi.data.fields import CategoricalObsField, LayerField
 from scvi.model.base import BaseModelClass, JaxTrainingMixin
 from scvi.utils import setup_anndata_dsp
 
 from ._jax_scgenvae import JaxSCGENVAE
@@ -133,15 +134,15 @@
         return np.mean(self.get_latent_representation(adata), axis=0)
 
     def get_decoded_expression(
         self,
         adata: AnnData | None = None,
         indices: Sequence[int] | None = None,
         batch_size: int | None = None,
-    ) -> np.ndarray:
+    ) -> Array:
         """Get decoded expression."""
         if self.is_trained_ is False:
             raise RuntimeError("Please train the model first.")
 
         adata = self._validate_anndata(adata)
         scdl = self._make_data_loader(adata=adata, indices=indices, batch_size=batch_size)
         decoded = []
@@ -198,14 +199,15 @@
                 batch_ind[i] = temp_ind
             max_batch_ann = batch_list[max_batch_ind]
             for study in batch_list:
                 delta = np.average(max_batch_ann.X, axis=0) - np.average(batch_list[study].X, axis=0)
                 batch_list[study].X = delta + batch_list[study].X
                 temp_cell[batch_ind[study]].X = batch_list[study].X
             shared_ct.append(temp_cell)
+
         all_shared_ann = AnnData.concatenate(*shared_ct, batch_key="concat_batch", index_unique=None)
         if "concat_batch" in all_shared_ann.obs.columns:
             del all_shared_ann.obs["concat_batch"]
         if len(not_shared_ct) < 1:
             corrected = AnnData(
                 np.array(self.module.as_bound().generative(all_shared_ann.X)["px"]),
                 obs=all_shared_ann.obs,
@@ -237,14 +239,15 @@
             corrected = corrected[adata.obs_names]
             if adata.raw is not None:
                 adata_raw = AnnData(X=adata.raw.X, var=adata.raw.var)
                 adata_raw.obs_names = adata.obs_names
                 corrected.raw = adata_raw
             corrected.obsm["latent"] = all_corrected_data.X
             corrected.obsm["corrected_latent"] = self.get_latent_representation(corrected)
+
             return corrected
 
     @classmethod
     @setup_anndata_dsp.dedent
     def setup_anndata(
         cls,
         adata: AnnData,
```

### Comparing `pertpy-0.4.0/pertpy/tools/_scgen/_jax_scgenvae.py` & `pertpy-0.5.0/pertpy/tools/_scgen/_jax_scgenvae.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
             z=z,
             # batch_index=batch_index,
         )
         return input_dict
 
     # def generative(self, x, z, batch_index) -> dict:
     def generative(self, z) -> dict:
-
         px = self.decoder(z)
         return dict(px=px)
 
     def loss(self, tensors, inference_outputs, generative_outputs):
         x = tensors[REGISTRY_KEYS.X_KEY]
         px = generative_outputs["px"]
         qz = inference_outputs["qz"]
@@ -112,15 +111,18 @@
 
     def sample(
         self,
         tensors,
         n_samples=1,
     ):
         inference_kwargs = dict(n_samples=n_samples)
-        inference_outputs, generative_outputs, = self.forward(
+        (
+            inference_outputs,
+            generative_outputs,
+        ) = self.forward(
             tensors,
             inference_kwargs=inference_kwargs,
             compute_loss=False,
         )
         px = dist.Normal(generative_outputs["px"], 1).sample()
         return px
```

### Comparing `pertpy-0.4.0/pertpy/tools/_scgen/_utils.py` & `pertpy-0.5.0/pertpy/tools/_scgen/_utils.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pertpy/tools/transferlearning_MMD_LICENSE` & `pertpy-0.5.0/pertpy/tools/transferlearning_MMD_LICENSE`

 * *Files identical despite different names*

### Comparing `pertpy-0.4.0/pyproject.toml` & `pertpy-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,75 @@
 [tool.poetry]
 name = "pertpy"
-version = "0.4.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.5.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Perturbation Analysis in the scverse ecosystem."
 authors = ["Lukas Heumos <lukas.heumos@posteo.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/theislab/pertpy"
 repository = "https://github.com/theislab/pertpy"
 documentation = "https://pertpy.readthedocs.io"
 packages = [
     { include = "pertpy" },
 ]
 classifiers = [
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.0,<3.11"
+python = ">=3.9.0,<3.11"
 rich = ">=10.11.0"
 PyYAML = ">=5.4.1"
-scanpy = ">=1.8.1"
-pypi-latest = ">=0.1.1"
+scanpy = {extras = ["leiden"], version = "^1.9.3"}
 muon = ">=0.1.2"
 requests = ">=2.27.1"
 ipywidgets = ">=7.6.5"
-switchlang = "^0.1.0"
-scikit-misc = "^0.1.4"
-plotnine = "^0.10.1"
-leidenalg = "^0.9.0"
-scipy = "^1.9.3"
-scvi-tools = "^0.19.0"
-adjusttext = "^0.7.3"
+switchlang = ">=0.1.0"
+scikit-misc = ">=0.1.4"
+plotnine = ">=0.10.1"
+scipy = ">=1.9.3"
+scvi-tools = ">=0.20.3"
+adjusttext = ">=0.7.3"
 toytree = "^2.0.1"
-arviz = ">=0.14,<0.16"
-numpyro = ">=0.10.1,<0.12.0"
+arviz = ">=0.14"
+numpyro = ">=0.10.1"
 statannotations = "^0.5.0"
-protobuf = "3.20.1"
-numba = "^0.56.4"
-decoupler = "^1.3.3"
+decoupler = "^1.3.4"
 ete3 = {version = "^3.1.2", optional = true}
 pyqt5 = {version = "^5.15.9", optional = true}
 ott-jax = "^0.4.0"
-pandas = "<=2.0.0"
-sparsecca = "^0.3.0"
+sparsecca = ">=0.3.0"
+numba = "^0.57.1"
 
 [tool.poetry.dev-dependencies]
+black = ">=22.12.0"
 pytest = ">=6.2.5"
 coverage = {extras = ["toml"], version = ">=6.2"}
-safety = ">=1.9.0"
 mypy = ">=0.930"
-typeguard = ">=2.13.3"
-xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 pre-commit = ">=2.16.0"
 flake8 = ">=4.0.1"
-black = ">=21.12b0"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.11.29"
 flake8-docstrings = ">=1.5.0"
 flake8-rst-docstrings = ">=0.2.5"
 pep8-naming = ">=0.12.1"
-reorder-python-imports = ">=2.6.0"
 pre-commit-hooks = ">=4.1.0"
 Pygments = ">=2.11.1"
 types-pkg-resources = ">=0.1.3"
 types-requests = ">=2.27.4"
 types-attrs = ">=19.1.0"
-Jinja2 = ">=3.0.3"
 pyenchant = ">=3.2.1"
 nbsphinx = ">=0.8.8"
-sphinx-gallery = ">0.6,<0.11"
+sphinx-gallery = ">0.6"
 sphinx-autodoc-typehints = ">=1.12.0"
 sphinx-last-updated-by-git = ">=0.3.0"
-sphinxcontrib-bibtex = ">=2.4.1"
 sphinx-automodapi = ">=0.14"
 nbsphinx-link = ">=1.3.0"
 sphinx-copybutton = ">=0.4.0"
 pyupgrade = ">=2.31.0"
 furo = ">=2022.3.4"
 myst-parser = ">=0.17.0"
 sphinx-remove-toctrees = ">=0.0.3"
@@ -89,16 +78,14 @@
 
 [tool.poetry.extras]
 ete3 = ["ete3"]
 
 [tool.poetry.scripts]
 pertpy = "pertpy.__main__:main"
 
-[tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
 strict = false
 pretty = true
@@ -110,14 +97,17 @@
 
 [tool.isort]
 multi_line_output=3
 include_trailing_comma=true
 balanced_wrapping=true
 line_length=120
 
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+
 [tool.coverage.paths]
 source = ["pertpy", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["pertpy"]
```

### Comparing `pertpy-0.4.0/PKG-INFO` & `pertpy-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 Metadata-Version: 2.1
 Name: pertpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Perturbation Analysis in the scverse ecosystem.
 Home-page: https://github.com/theislab/pertpy
 License: MIT
 Author: Lukas Heumos
 Author-email: lukas.heumos@posteo.net
-Requires-Python: >=3.8.0,<3.11
+Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: ete3
 Requires-Dist: PyYAML (>=5.4.1)
-Requires-Dist: adjusttext (>=0.7.3,<0.8.0)
-Requires-Dist: arviz (>=0.14,<0.16)
-Requires-Dist: decoupler (>=1.3.3,<2.0.0)
+Requires-Dist: adjusttext (>=0.7.3)
+Requires-Dist: arviz (>=0.14)
+Requires-Dist: decoupler (>=1.3.4,<2.0.0)
 Requires-Dist: ete3 (>=3.1.2,<4.0.0) ; extra == "ete3"
 Requires-Dist: ipywidgets (>=7.6.5)
-Requires-Dist: leidenalg (>=0.9.0,<0.10.0)
 Requires-Dist: muon (>=0.1.2)
-Requires-Dist: numba (>=0.56.4,<0.57.0)
-Requires-Dist: numpyro (>=0.10.1,<0.12.0)
+Requires-Dist: numba (>=0.57.1,<0.58.0)
+Requires-Dist: numpyro (>=0.10.1)
 Requires-Dist: ott-jax (>=0.4.0,<0.5.0)
-Requires-Dist: pandas (<=2.0.0)
-Requires-Dist: plotnine (>=0.10.1,<0.11.0)
-Requires-Dist: protobuf (==3.20.1)
-Requires-Dist: pypi-latest (>=0.1.1)
+Requires-Dist: plotnine (>=0.10.1)
 Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: rich (>=10.11.0)
-Requires-Dist: scanpy (>=1.8.1)
-Requires-Dist: scikit-misc (>=0.1.4,<0.2.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
-Requires-Dist: scvi-tools (>=0.19.0,<0.20.0)
-Requires-Dist: sparsecca (>=0.3.0,<0.4.0)
+Requires-Dist: scanpy[leiden] (>=1.9.3,<2.0.0)
+Requires-Dist: scikit-misc (>=0.1.4)
+Requires-Dist: scipy (>=1.9.3)
+Requires-Dist: scvi-tools (>=0.20.3)
+Requires-Dist: sparsecca (>=0.3.0)
 Requires-Dist: statannotations (>=0.5.0,<0.6.0)
-Requires-Dist: switchlang (>=0.1.0,<0.2.0)
+Requires-Dist: switchlang (>=0.1.0)
 Requires-Dist: toytree (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://pertpy.readthedocs.io
 Project-URL: Repository, https://github.com/theislab/pertpy
 Description-Content-Type: text/markdown
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Build](https://github.com/theislab/pertpy/workflows/Build%20pertpy%20Package/badge.svg)](https://github.com/theislab/pertpy/actions?workflow=Package)
@@ -54,32 +46,28 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/pertpy)](https://pypi.org/project/pertpy)
 [![Read the Docs](https://img.shields.io/readthedocs/pertpy/latest.svg?label=Read%20the%20Docs)](https://pertpy.readthedocs.io/)
 [![Test](https://github.com/theislab/pertpy/workflows/Run%20pertpy%20Tests/badge.svg)](https://github.com/theislab/pertpy/actions?workflow=Tests)
 [![PyPI](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # pertpy
 
-## Features
+![pertpy-wide1](https://user-images.githubusercontent.com/21954664/235677503-0c72f90d-3f6d-4a16-a1ff-ff8c11a540fb.png)
+
+## Documentation
 
--   Differential cell type perturbation analysis with Augurpy
--   Analysis of CRISPR-KO screens with Mixscape
--   Compositional analysis with Milo and tascCODA
+Please read the [documentation](https://pertpy.readthedocs.io/en/latest).
 
 ## Installation
 
 You can install _pertpy_ via [pip] from [PyPI]:
 
 ```console
 $ pip install pertpy
 ```
 
-## Usage
-
-Please see [Usage] for details.
-
 ## Credits
 
 This package was created with [cookietemple] using [Cookiecutter] based on [Hypermodern_Python_Cookiecutter].
 
 [cookiecutter]: https://github.com/audreyr/cookiecutter
 [cookietemple]: https://cookietemple.com
 [hypermodern_python_cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
```

